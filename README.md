[MANUAL_UTILIZADOR_ANGOLA.md](https://github.com/user-attachments/files/22553147/MANUAL_UTILIZADOR_ANGOLA.md)
# Manual do Utilizador - Sistema de Fluxo de Caixa Angola

## Índice

1. [Introdução](#introdução)
2. [Instalação](#instalação)
3. [Configuração Inicial](#configuração-inicial)
4. [Funcionalidades Principais](#funcionalidades-principais)
5. [Gestão de Contas](#gestão-de-contas)
6. [Registo de Movimentos](#registo-de-movimentos)
7. [Relatórios](#relatórios)
8. [Backup e Manutenção](#backup-e-manutenção)
9. [Resolução de Problemas](#resolução-de-problemas)
10. [Suporte Técnico](#suporte-técnico)

---

## Introdução

O **Sistema de Fluxo de Caixa Angola** é uma aplicação web desenvolvida especificamente para facilitar a gestão financeira diária de empresas angolanas. O sistema foi concebido para ser simples de usar, mesmo para utilizadores com poucos conhecimentos de contabilidade, e está totalmente adaptado ao contexto empresarial angolano.

### Características Principais

- **Interface Web Simples**: Acesso através de qualquer navegador
- **Adaptado para Angola**: Moeda em Kwanzas (Kz), categorias locais
- **Multi-empresa**: Suporte para diferentes empresas numa única instalação
- **Gestão de Contas**: Controlo de caixas e contas bancárias
- **Categorização Angolana**: Categorias adaptadas ao contexto local
- **Relatórios Profissionais**: Relatórios mensais prontos para aprovação
- **Backup Automático**: Sistema de backup integrado
- **Instalação Simples**: Instalador automático para Windows

---

## Instalação

### Requisitos do Sistema

- **Sistema Operativo**: Windows 7 ou superior
- **Python**: Versão 3.7 ou superior
- **Navegador Web**: Chrome, Firefox, Edge ou Safari
- **Espaço em Disco**: Mínimo 100 MB

### Processo de Instalação

1. **Descarregar o Sistema**
   - Extrair todos os ficheiros para uma pasta (ex: `C:\FluxoCaixaAngola`)

2. **Executar o Instalador**
   - Fazer duplo clique no ficheiro `instalar.bat`
   - Seguir as instruções no ecrã

3. **Configurar a Empresa**
   - Inserir o nome da empresa
   - Inserir o NIF (aceita formatos angolanos de 8-15 dígitos)

4. **Aguardar a Instalação**
   - O sistema instalará automaticamente todas as dependências
   - Criará a base de dados
   - Configurará os ficheiros necessários

---

## Configuração Inicial

### Primeiro Acesso

1. **Iniciar o Sistema**
   - Executar `iniciar_sistema.bat`
   - Aguardar a mensagem "Sistema iniciado"

2. **Aceder à Interface Web**
   - Abrir o navegador
   - Navegar para `http://localhost:5000`

3. **Configurar Contas Iniciais**
   - Criar pelo menos uma conta (caixa ou banco)
   - Definir o saldo inicial de cada conta em Kwanzas

### Categorias Pré-definidas para Angola

O sistema vem com categorias adaptadas ao contexto angolano:

- **Rendas**: Pagamento de rendas e alugueres
- **Condomínios**: Taxas de condomínio e manutenção predial
- **Água**: Conta de água - EPAL Angola
- **Luz**: Conta de eletricidade - ENE Angola
- **Combustível**: Gasóleo, gasolina e gás doméstico
- **Produtos de Limpeza**: Detergentes e material de limpeza
- **Manutenção**: Manutenção de equipamentos e instalações
- **Alimentação**: Cafés, chás, águas e alimentação
- **Material de Escritório**: Papel, canetas, tinteiros e consumíveis
- **Seguros**: Seguros diversos
- **Telecomunicações**: Internet, telefone e comunicações
- **Transporte**: Combustível, manutenção de viaturas e transportes
- **Impostos e Taxas**: Impostos, taxas e contribuições
- **Outras Despesas**: Despesas diversas não categorizadas

---

## Funcionalidades Principais

### Dashboard

O dashboard apresenta uma visão geral do estado financeiro em Kwanzas:

- **Resumo das Contas**: Saldos atuais de todas as contas
- **Movimentos Recentes**: Últimas transações registadas
- **Estatísticas Rápidas**: Totais e contadores
- **Ações Rápidas**: Acesso direto às funcionalidades principais

### Navegação

A navegação é feita através do menu principal:

- **Dashboard**: Página inicial com resumo
- **Contas**: Gestão de caixas e bancos
- **Movimentos**: Histórico de transações
- **Novo Movimento**: Registo de entradas e saídas
- **Relatórios**: Geração de relatórios mensais

---

## Gestão de Contas

### Tipos de Contas

**Caixas**
- Dinheiro físico em Kwanzas
- Exemplos: "Caixa Principal", "Fundo de Maneio", "Caixa Pequeno"

**Bancos**
- Contas bancárias angolanas
- Exemplos: "BFA Conta Corrente", "BAI Poupança", "BIC Empresa"

### Criar Nova Conta

1. Aceder ao menu **Contas**
2. Clicar em **Nova Conta**
3. Preencher os campos:
   - **Nome**: Nome descritivo da conta
   - **Tipo**: Caixa ou Banco
   - **Saldo Inicial**: Valor atual da conta em Kwanzas
4. Clicar em **Criar Conta**

---

## Registo de Movimentos

### Tipos de Movimentos

**Entradas (Recebimentos)**
- Dinheiro que entra na conta
- Exemplos: Vendas, recebimentos de clientes, prestação de serviços

**Saídas (Pagamentos)**
- Dinheiro que sai da conta
- Exemplos: Pagamentos a fornecedores, despesas operacionais

### Registar Novo Movimento

1. Aceder ao menu **Novo Movimento**
2. Preencher os campos obrigatórios:
   - **Data**: Data do movimento
   - **Tipo**: Entrada ou Saída
   - **Descrição**: Descrição clara do movimento
   - **Valor**: Montante em Kwanzas (sempre positivo)
   - **Conta**: Conta onde registar o movimento
3. Para saídas, selecionar a **Categoria** apropriada
4. **Informações do Documento** (opcional):
   - **Tipo de Documento**: Fatura, Recibo, Nota de Débito, etc.
   - **Número do Documento**: Número da fatura ou recibo
5. **Informações do Fornecedor/Cliente** (obrigatório):
   - **Tipo**: Formal, Informal ou Movimento Interno
   - **Nome**: Nome da empresa ou pessoa
   - **NIF**: Obrigatório apenas para fornecedores formais
6. Clicar em **Registar Movimento**

### Tipos de Fornecedores

**Fornecedor Formal**
- Empresas registadas com NIF
- Emitem documentos fiscais (faturas, recibos)
- NIF é obrigatório
- Exemplos: Fornecedores de equipamentos, prestadores de serviços registados

**Fornecedor Informal**
- Mercado paralelo/informal
- Sem NIF ou documentos fiscais
- Apenas nome é obrigatório
- Exemplos: Vendedores de rua, pequenos comerciantes informais

**Movimento Interno**
- Transferências entre contas da própria empresa
- Não requer NIF
- Exemplos: Transferência de caixa para banco

### Boas Práticas para Angola

- Registar movimentos no mesmo dia em que ocorrem
- Usar descrições claras em português
- Sempre associar saídas a uma categoria
- Para pagamentos de impostos, usar a categoria "Impostos e Taxas"
- Para combustível de viaturas, usar "Transporte"
- Para contas de serviços públicos, usar as categorias específicas (Água, Luz)

---

## Relatórios

### Relatório Mensal

O relatório mensal é formatado para o contexto empresarial angolano.

#### Conteúdo do Relatório

1. **Cabeçalho**
   - Nome da empresa e NIF
   - Período do relatório
   - Data de geração

2. **Resumo Executivo em Kwanzas**
   - Total de entradas
   - Total de saídas
   - Resultado líquido

3. **Análise de Despesas por Categoria**
   - Breakdown detalhado por categoria angolana
   - Identificação da maior despesa

4. **Posição das Contas**
   - Saldo atual de cada conta em Kwanzas
   - Saldo total consolidado

5. **Indicadores de Performance**
   - Taxa de crescimento
   - Eficiência de gastos

6. **Seção de Aprovação**
   - Espaços para assinaturas da direção
   - Data de aprovação

---

## Backup e Manutenção

### Criar Backup

1. **Automático**: Executar `criar_backup.bat`
2. **Manual**: Copiar o ficheiro `database/fluxo_caixa.db`

### Manutenção Regular

- **Backup Semanal**: Recomendado para empresas ativas
- **Verificação Mensal**: Executar `corrigir_sistema.py`
- **Limpeza**: Manter apenas os últimos 10 backups

---

## Resolução de Problemas

### Problemas Específicos de Angola

#### Formatação de Números

**Problema**: Valores não aparecem corretamente
**Solução**: O sistema usa formatação angolana (Kz) automaticamente

#### Categorias em Falta

**Problema**: Não encontra categoria específica
**Solução**: Usar "Outras Despesas" ou contactar administrador para adicionar

### Script de Correção Automática

O ficheiro `corrigir_sistema.py` resolve automaticamente:
- Problemas de formatação de moeda
- Categorias em falta
- Estrutura de base de dados
- Permissões de ficheiros

---

## Suporte Técnico

### Informações do Sistema

- **Versão**: 1.0 Angola
- **Moeda**: Kwanza Angolano (Kz)
- **Localização**: pt-AO
- **Tecnologia**: Python Flask + SQLite

### Estrutura de Ficheiros

```
fluxo_caixa/
├── app.py                          # Aplicação principal
├── instalar.bat                    # Instalador Windows
├── iniciar_sistema.bat             # Script de arranque
├── criar_backup.bat                # Script de backup
├── corrigir_sistema.py             # Script de correção
├── MANUAL_UTILIZADOR_ANGOLA.md     # Este manual
├── database/
│   └── fluxo_caixa.db             # Base de dados SQLite
├── src/
│   ├── models/                     # Modelos adaptados para Angola
│   └── static/
│       ├── css/                    # Estilos
│       ├── js/                     # JavaScript com formatação Kz
│       └── templates/              # Interface em português angolano
```

### Contacto para Suporte

Para suporte específico para Angola:
1. Consultar este manual
2. Executar script de correção
3. Contactar o administrador local do sistema

---

**© 2024 Sistema de Fluxo de Caixa Angola - Desenvolvido para facilitar a gestão financeira empresarial em Angola**

**Adaptado para**: Empresas angolanas, moeda Kwanza, categorias locais, regulamentação angolana
