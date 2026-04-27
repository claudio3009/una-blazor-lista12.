# EcoMonitor - Lista 12

## Identificação

**Aluno:** Claudio Martins Camilo Júnior

**Curso:** (Análise e Desenvolvimento de Sistemas)

**Disciplina:** Interação Humano Computador e UX

**Professor:** Daniel Henrique Matos de Paiva

---

## Descrição do Projeto

O EcoMonitor é uma prova de conceito (PoC) em Blazor para registrar ações sustentáveis e acompanhar o impacto ambiental em tempo real.

O sistema possui três ações:

* Reciclagem de Plástico (1 ponto por ação)
* Descarte de Eletrônicos (5 pontos por ação)
* Plantio de Árvores (10 pontos por ação)

Cada atividade acumula pontos individualmente e permite visualizar o progresso do usuário.

---

## Heurísticas de Nielsen Aplicadas

### 1. Visibilidade do Status do Sistema

O sistema fornece feedback imediato ao usuário por meio:

* Atualização do contador
* Barra de progresso
* Mensagem ao atingir a meta

Isso permite acompanhar o estado atual do sistema em tempo real.

---

### 2. Feedback Imediato

Ao clicar em **Registrar Atividade**, o sistema responde instantaneamente:

* Soma os pontos
* Atualiza o progresso
* Exibe mensagem de conquista quando a meta é atingida

---

## Explicação Técnica

O componente `EcoStatus.razor` utiliza parâmetros com `[Parameter]` para torná-lo reutilizável:

* `Titulo`
* `PesoAcao`

Isso permite reutilizar o mesmo componente para diferentes ações sem duplicar código.

Cada instância possui seu próprio estado (`Total`) independente das demais.

---

## Guia de Execução

Clone o projeto e execute:

```bash
dotnet restore
dotnet run --launch-profile https
```

Abra no navegador:

```text
https://localhost:7025
```

---

## Funcionalidades Implementadas

✔ Componente reutilizável
✔ Estado dinâmico com contador
✔ Incremento por clique
✔ Barra de progresso
✔ Meta de 100 pontos
✔ Mensagem de conquista ("Herói do Planeta")

---

## Repositório

Nome do repositório solicitado:

```text
una-blazor-lista12
```
