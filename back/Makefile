# Define o programa Go usado nas tarefas deste backend.
GO := go

# Identifica o pacote que contém o ponto de entrada da API.
APP := ./cmd/api

# Define o caminho local para o executável compilado.
BINARY := bin/sisdeve-agro-api

# Declara alvos que representam ações e não arquivos de saída.
.PHONY: help run test fmt vet check build clean

# Exibe a lista de comandos disponíveis ao desenvolvedor.
help:
	@echo "Comandos do backend Sisdeve Agro:"
	@echo "  make run    - Executa o programa Go"
	@echo "  make test   - Executa todos os testes Go"
	@echo "  make fmt    - Formata o código Go"
	@echo "  make vet    - Analisa problemas suspeitos no código"
	@echo "  make build  - Compila o executável em bin/"
	@echo "  make clean  - Remove o executável compilado"

# Executa o pacote principal da aplicação sem criar um binário permanente.
run:
	$(GO) run $(APP)

# Executa os testes de todos os pacotes do módulo.
test:
	$(GO) test ./...

# Aplica a formatação padrão a todos os pacotes Go.
fmt:
	$(GO) fmt ./...

# Executa a análise estática oferecida pela ferramenta Go.
vet:
	$(GO) vet ./...

check: fmt vet test

# Cria a pasta de saída antes de compilar a aplicação.
build:
	mkdir -p bin
	$(GO) build -o $(BINARY) $(APP)

# Remove somente o binário produzido por este Makefile.
clean:
	rm -f $(BINARY)