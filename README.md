# Sistema de Conferência de Conversão de Dados

Sistema desenvolvido em **Python** para automatizar a conferência de dados em processos de conversão entre sistemas de folha de pagamento.

A aplicação realiza a extração, comparação e validação de informações entre diferentes bases de dados, identificando divergências e gerando relatórios técnicos para auxiliar equipes durante processos de migração de sistemas.

> ⚠️ Este repositório representa uma versão de portfólio. Algumas regras de negócio, consultas SQL e informações específicas foram omitidas por questões de confidencialidade.

---

# Interface

## Menu Principal

![Tela Principal](images/tela_principal.png)

Tela inicial da aplicação, onde o usuário escolhe o sistema de origem dos dados (SAGE ou Consisanet) e inicia o processo de conferência.

---

## Extração de Dados

![Extração](images/conexao&extracao.png)

Nesta etapa o sistema:

- Lê o arquivo de relacionamento das empresas
- Conecta aos bancos de dados
- Executa dezenas de consultas SQL
- Gera automaticamente os arquivos utilizados na comparação

---

## Processamento

![Processamento](images/processamento.png)

Após a extração, a aplicação executa automaticamente todas as fases da conferência, gerando:

- Comparações
- Divergências
- Relatórios
- Resumo final do processamento

---

## Estrutura dos Resultados

![Resultados](images/estrutura.png)

Todos os arquivos gerados são organizados automaticamente em pastas, facilitando a análise dos resultados.

---

# Funcionalidades

- Comparação de Empresas
- Comparação de Empregados
- Comparação de Férias
- Comparação de Alterações Salariais
- Comparação de Horários
- Comparação de Eventos do eSocial
- Comparação de Responsáveis Legais
- Comparação de Serviços e Obras
- Geração automática de relatórios em Excel
- Dashboard com indicadores de processamento
- Organização automática dos arquivos por empresa
- Tratamento de divergências entre sistemas

---

# Fluxo do Processo

```text
Sistema de Origem
        │
        ▼
Extração dos Dados
        │
        ▼
Tratamento
        │
        ▼
Comparação
        │
        ▼
Relatórios
        │
        ▼
Resumo Final
```

---

# Tecnologias Utilizadas

- Python
- SQL
- Firebird
- SQL Anywhere (Sybase)
- Pandas
- OpenPyXL
- Tkinter
- Git
- GitHub

---

# Estrutura do Projeto

```text
app/
├── banco/
├── comum/
├── consisanet/
├── interface/
├── sage/
└── servico/

scripts/
├── FASE1_EMPRESA
├── FASE2_EMPREGADOS
├── FASE3_FERIAS
├── FASE4_ALTERACOES_SALARIAIS
└── FASE5_HORARIOS

images/

requirements.txt
README.md
```

---

# Objetivo

Automatizar processos de conferência de dados durante migrações entre sistemas, reduzindo o tempo de análise manual e aumentando a confiabilidade das validações realizadas.

---

# Diferenciais do Projeto

- Interface gráfica intuitiva
- Arquitetura modular
- Automatização de processos repetitivos
- Comparação entre múltiplos sistemas
- Geração automática de relatórios
- Organização dos resultados por empresa
- Projeto desenvolvido para utilização em ambiente corporativo

---

# Observações

Por questões de confidencialidade, este repositório não contém:

- Bases de dados utilizadas em produção
- Consultas SQL proprietárias
- Informações de clientes
- Regras de negócio específicas

O objetivo é demonstrar a arquitetura, a organização do projeto e as tecnologias utilizadas durante o desenvolvimento.

---

# Autor

## Higor Batista de Souza

Analista de Sistemas | Desenvolvedor Python | SQL | Automação de Processos | Banco de Dados

LinkedIn: https://www.linkedin.com/in/higorsouza-analistadedados/

GitHub: https://github.com/HigorSouzaBatista