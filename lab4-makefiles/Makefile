# ============================================================
# Makefile - Simulação de Pipeline com Kaniko
# Autor: Deivide Souza
# Objetivo: Automatizar build, push e limpeza de imagens
# ============================================================

# Variáveis Globais
IMAGE_NAME := docker.io/deividesouza12/lab4-make-kaniko
TAG := v1.0.0
WORKDIR := $(shell pwd)
CONFIG := $(WORKDIR)/config-kaniko.json
KANIKO_IMAGE := gcr.io/kaniko-project/executor:latest

#================================
# Tagets Principais
#================================

build:
	@echo "Iniciando build da imagem com Kaniko..."
	docker run \
	-v $(WORKDIR):/workspace \
	-v ${CONFIG}:/kaniko/.docker/config.json:ro \
	$(KANIKO_IMAGE) \
	--context /workspace \
	--dockerfile /workspace/Dockerfile \
	--destination $(IMAGE_NAME):$(TAG) \
	--cleanup
	@echo "Build concluído."

## make push  →  Faz push manual (caso build local seja usado)
push:
	@echo "Kaniko já fez o push da imagem. Nenhuma ação necessária."

## make clean  →  Remove imagens locais
clean:
	@echo "Removendo imagens locais..."
	docker system prune -f
	@echo "Imagens removidas."

## make pipeline  →  Executa o fluxo completo
pipeline: build push clean
	@echo " Pipeline finalizada com sucesso!"