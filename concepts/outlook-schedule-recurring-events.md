---
title: Agendar compromissos repetidos como eventos recorrentes no Outlook
description: Os eventos recorrentes são uma parte importante do calendário do Outlook. Quer seja uma reunião individual semanal com seu gerente ou uma reunião de revisão de toda a divisão que acontece na segunda terça-feira de cada mês, os eventos recorrentes tornam mais fácil criar o evento uma vez e deixar o servidor preencher o resto da série.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 29aeef98cbc0e9d33df26a0c54bb568317ebb790
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071781"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a>Agendar compromissos repetidos como eventos recorrentes no Outlook

Os eventos recorrentes são uma parte importante do calendário do Outlook. Quer seja uma reunião individual semanal com seu gerente ou uma reunião de revisão de toda a divisão que acontece na segunda terça-feira de cada mês, os eventos recorrentes tornam mais fácil criar o evento uma vez e deixar o servidor preencher o resto da série.

O principal dado que permite que os eventos recorrentes sejam "expandidos" em ocorrências individuais é a regra de recorrência. A regra especifica a frequência de repetição do evento e sua duração. As regras de recorrência modelam as APIs REST do Outlook na propriedade **recorrência** do [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0). 

Cada recorrência é composta de duas partes: o padrão de recorrência (frequência) e o intervalo de recorrência (duração).

## <a name="recurrence-patterns"></a>Padrões de recorrência

A primeira parte de uma recorrência é o padrão. Ele especifica a frequência com que o evento se repete. Por exemplo, um evento poderia repetir "a cada 3 dias", "toda quinta-feira" ou "em 22 de julho de cada ano". Um padrão é representado na API pelo [recurso recurrencePattern](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).

Dependendo do tipo de padrão, determinados campos do **recurrencePattern** são obrigatórios, opcionais ou ignorados.

> **Observação**: Mesmo que um campo seja ignorado, ele ainda é validado. Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.

Vamos dar uma olhada em cada um dos tipos de possíveis de padrão.

### <a name="daily"></a>Diariamente

O padrão de recorrência diária faz com que um evento se repita com base em um número de dias entre cada ocorrência.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **intervalo** | Obrigatório | Especifica o número de dias entre cada ocorrência. |
| **type** | Obrigatório | Tem que ser definida como `daily`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento todos os dias

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- Repita esse evento a cada 3 dias

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a>Semanalmente

O padrão de recorrência semanal faz com que um evento se repita no mesmo dia ou dias da semana, com base no número de semanas entre cada conjunto de ocorrências.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **daysOfWeek** | Obrigatório | Especifica em quais dias da semana o evento ocorre. |
| **firstDayOfWeek** | Opcional | Especifica qual dia é considerado o primeiro dia da semana. Valor padrão: `Sunday`. |
| **intervalo** | Obrigatório | Especifica o número de semanas entre cada conjunto de ocorrências. |
| **type** | Obrigatório | Tem que ser definida como `weekly`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento toda quinta-feira

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- Repita esse evento em segundas e terças alternadas

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a>Mensal absoluto

O padrão mensal absoluto faz com que um evento se repita no mesmo dia do mês (por exemplo, dia 15), com base no número de meses entre cada ocorrência.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **dayOfMonth** | Obrigatório | Especifica em quais dias do mês o evento ocorre. |
| **intervalo** | Obrigatório | Especifica o número de meses entre cada ocorrência. |
| **type** | Obrigatório | Tem que ser definida como `absoluteMonthly`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento no 15º dia de cada mês

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- Repita esse evento trimestralmente (a cada 3 meses) no dia 7

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a>Mensal relativo

O padrão mensal relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa do mês, com base no número de meses entre cada ocorrência. Por exemplo, "toda segunda quarta-feira do mês".

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **daysOfWeek** | Obrigatório | Especifica em quais dias da semana o evento pode ocorrer. Os eventos mensais relativos ocorrem apenas uma vez por mês, portanto, se mais de um valor for especificado, o evento cairá no primeiro dia que satisfaça o padrão. |
| **índice** | Opcional | Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês. Valores possíveis: `first`, `second`, `third`, `fourth` e `last`. Valor padrão: `first`. |
| **intervalo** | Obrigatório | Especifica o número de meses entre cada ocorrência. |
| **type** | Obrigatório | Tem que ser definida como `relativeMonthly`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento na segunda quarta-feira de cada mês

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- Repita esse evento na primeira quinta ou sexta-feira de cada mês

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a>Anual absoluto

O padrão anual absoluto faz com que um evento se repita no mesmo mês e dia (por exemplo, dia 15 de abril), com base no número de anos entre cada ocorrência.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **dayOfMonth** | Obrigatório | Especifica em quais dias do mês o evento ocorre. |
| **Mês** | Obrigatório | Especifica em qual mês o evento ocorre. |
| **intervalo** | Obrigatório | Especifica o número de anos entre cada ocorrência. |
| **type** | Obrigatório | Tem que ser definida como `absoluteYearly`. |

#### <a name="example"></a>Exemplo

- Repita esse evento em 15 de abril todo ano

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a>Anual relativo

O padrão anual relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa em um mês específico, com base no número de anos entre cada ocorrência. Por exemplo, "toda última quarta-feira de novembro".

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **daysOfWeek** | Obrigatório | Especifica em quais dias da semana o evento pode ocorrer. Os eventos anuais relativos ocorrem apenas uma vez por ano, portanto, se mais de um valor for especificado, o evento cairá no primeiro dia que satisfaça o padrão. |
| **índice** | Opcional | Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês. Valores possíveis: `first`, `second`, `third`, `fourth` e `last`. Valor padrão: `first`. |
| **Mês** | Obrigatório | Especifica em qual mês o evento ocorre. |
| **intervalo** | Obrigatório | Especifica o número de anos entre cada ocorrência. |
| **type** | Obrigatório | Tem que ser definida como `relativeYearly`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento na última quarta-feira de novembro a cada ano

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a>Intervalos de recorrência

A segunda parte de uma recorrência é o intervalo. Especifica por quanto tempo o padrão se repete. Por exemplo, um evento poderia terminar após 10 ocorrências, em uma data específica ou poderia não ter fim. Um intervalo é representado na API pelo [recurso recurrenceRange](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).

Dependendo do tipo de intervalo, determinados campos do **recurrenceRange** são obrigatórios ou ignorados.

> **Observação**: Mesmo que um campo seja ignorado, ele ainda é validado. Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.

Vamos dar uma olhada em cada um dos tipos de possíveis de intervalo.

### <a name="numbered-range"></a>Intervalo numerado

O intervalo numerado faz com que um evento ocorra um número fixo de vezes (com base no padrão) de uma data de início.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **numberOfOccurences** | Obrigatório | Especifica o número de ocorrências. Deve ser um número inteiro positivo. |
| **recurrenceTimeZone** | Opcional | Especifica o fuso horário para a propriedade **startDate**. Se a propriedade não for especificada, será usado o fuso horário do evento. |
| **startDate** | Obrigatório | Especifica a data para começar a aplicar o padrão. O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0). Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão. |
| **type** | Obrigatório | Tem que ser definida como `numbered`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento 10 vezes

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a>Intervalo de datas de término

O intervalo de datas de término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável entre uma data de início e uma data de término.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **endDate** | Obrigatório | Especifica a data para parar de aplicar o padrão. Observe que a última ocorrência da reunião pode não ocorrer nesta data se não se enquadrar no padrão. |
| **recurrenceTimeZone** | Opcional | Especifica o fuso horário das propriedades **startDate** e **endDate**. Se a propriedade não for especificada, será usado o fuso horário do evento. |
| **startDate** | Obrigatório | Especifica a data para começar a aplicar o padrão. O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0). Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão. |
| **type** | Obrigatório | Tem que ser definida como **endDate**. |

#### <a name="examples"></a>Exemplos

- Repita esse evento de 1.º de julho de 2017 a 31 de julho de 2017

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a>Intervalo sem término

O intervalo sem término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável após uma data de início.

#### <a name="relevant-properties"></a>Propriedades relevantes

| Propriedade | Relevância | Descrição |
|----------|-----------|-------------|
| **recurrenceTimeZone** | Opcional | Especifica o fuso horário para a propriedade **startDate**. Se a propriedade não for especificada, será usado o fuso horário do evento. |
| **startDate** | Obrigatório | Especifica a data para começar a aplicar o padrão. O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0). Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão. |
| **type** | Obrigatório | Tem que ser definida como `noEnd`. |

#### <a name="examples"></a>Exemplos

- Repita esse evento de 15 de maio de 2017 para sempre

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a>Usando padrões e intervalos para criar eventos recorrentes

Agora que já vimos padrões e intervalos separadamente, vamos analisar como eles funcionam juntos e como eles interagem com as propriedades **iniciar** e **encerrar** do evento.

### <a name="creating-a-recurrence-rule"></a>Criando uma regra de recorrência

Para criar uma regra de recorrência, você deve especificar um padrão e um intervalo. Qualquer tipo de padrão pode funcionar com qualquer tipo de intervalo. Eis alguns exemplos.

#### <a name="examples"></a>Exemplos

- **Reunião das 13h às 13h30 toda segunda-feira a partir de 4 de setembro de 2017 até o final do ano**

  - O requisito "toda segunda-feira" requisito é atendido facilmente pelo tipo de padrão de recorrência `weekly`.
  - O requisito "até o final do ano" indica um tipo de intervalo de recorrência `endDate`.

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  Como 31 de dezembro de 2017 é um domingo, a última ocorrência dessa série será na segunda-feira, dia 25 de dezembro.

- **Reunião das 14h às 15h na primeira quinta-feira de cada mês a partir de 29 de agosto de 2017**

  - O requisito "primeira quinta-feira de cada mês" pode ser cumprido usando um padrão mensal relativo. A parte "cada mês" indica que o **intervalo** deve ser definido como `2`.
  - Por não existir um requisito de data de término, um tipo de intervalo `noEnd` pode ser usado.

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  Como o valor de **starDate** é após a primeira quinta-feira de agosto, a primeira ocorrência dessa série será em setembro.

## <a name="next-steps"></a>Próximas etapas
    
- Veja mais detalhes em [integração com o calendário do Outlook](outlook-calendar-concept-overview.md).
- Visualize outros exemplos de eventos recorrentes na referência da API do calendário:
  - [Crie um evento recorrente que ocorra uma vez por semana](/graph/api/user-post-events?view=graph-rest-1.0#request-3)
  - [Crie um evento recorrente diário](/graph/api/user-post-events?view=graph-rest-1.0#request-4)

