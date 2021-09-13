---
title: Tipo de recurso recurrencePattern
description: 'Descreve a frequência com que um event recorrente se repete. '
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 89e8c29f2e18259db0496fbe2cb93a4c70b086ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078641"
---
# <a name="recurrencepattern-resource-type"></a>Tipo de recurso recurrencePattern

Namespace: microsoft.graph

Descreve a frequência com que um [event](event.md) recorrente se repete.

É possível especificar o padrão de recorrência de um evento recorrente de uma de seis maneiras, dependendo do seu cenário. Para cada tipo de padrão, especifique a quantidade de tempo entre as ocorrências. As ocorrências reais do evento recorrente sempre seguem esse padrão dentro do intervalo de datas que você especifica para o evento. Um evento recorrente é sempre definido por seu **recurrencePattern** (com que frequência o evento se repete) e seu [recurrenceRange](recurrencerange.md) (por quanto tempo o evento se repete).

Use a propriedade **type** para especificar os diferentes tipos de **recurrencePattern** e a propriedade **interval** para especificar o tempo entre as ocorrências, que pode ser em número de dias, semanas, meses ou anos, dependendo do **type**. Observe quais propriedades são necessárias para cada tipo, conforme descrito na tabela a seguir.

> **Observação** Inclua apenas as propriedades necessárias para um padrão de recorrência. Qualquer propriedade que você incluir que não tenha um valor compatível resultará em erro.

| Tipo de padrão de recorrência | Valor da propriedade type | Descrição | Exemplo | Propriedades necessárias |
|:---------------|:--------|:--------|:--------|:----------|
| Diariamente | `daily` | O evento se repete com base no número de dias especificado pelo **interval** entre ocorrências. | Repita o evento a cada três dias. | **type**, **interval** |
| Semanalmente | `weekly` | O evento se repete no mesmo dia ou dias da semana, com base no número de semanas entre cada conjunto de ocorrências. | Repita o evento nas segundas e terças-feiras a cada duas semanas. | **type**, **interval**, **daysOfWeek**, **firstDayOfWeek** |
| Mensal absoluto | `absoluteMonthly` | O evento se repete no dia especificado do mês (por exemplo, o dia 15), com base no número de meses entre as ocorrências. | Repita o evento trimestralmente (a cada três meses) no dia 15. | **type**, **interval**, **dayOfMonth** |
| Mensal relativo | `relativeMonthly` | O evento se repete no dia ou dias específicos da semana, na mesma posição relativa no mês, com base no número de meses entre as ocorrências. | Repita o evento na segunda quinta-feira ou sexta-feira a cada três meses. | **type**, **interval**, **daysOfWeek** |
| Anual absoluto | `absoluteYearly` | O evento se repete no dia e mês específicos, com base no número de anos entre as ocorrências. | Repita o evento no dia 15 de março a cada três anos. | **type**, **interval**, **dayOfMonth**, **month** |
| Anual relativo | `relativeYearly` | O evento se repete no dia ou dias específicos da semana, na mesma posição relativa em um mês específico do ano, com base no número de anos entre as ocorrências. | Repita o evento na segunda quinta-feira ou sexta-feira de novembro a cada três anos. | **type**, **interval**, **daysOfWeek**, **month** |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|O dia do mês em que ocorre o evento. Obrigatório se **type** for `absoluteMonthly` ou `absoluteYearly`. |
|daysOfWeek|Coleção dayOfWeek|Uma coleção dos dias da semana em que o evento ocorre. Os valores possíveis são `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. <br>Se **type** for `relativeMonthly` ou `relativeYearly` e **daysOfWeek** especificar mais de um dia, o evento cairá no primeiro dia que satisfizer o padrão. <br> Obrigatório se **type** for `weekly`, `relativeMonthly` ou `relativeYearly`.|
|firstDayOfWeek|dayOfWeek|O primeiro dia da semana. Os valores possíveis são `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. O padrão é `sunday`. Obrigatório se **type** for `weekly`. |
|index|weekIndex|Especifica em qual instância dos dias permitidos especificados em **daysOfWeek** ocorre o evento, contado da primeira instância do mês. Os valores possíveis são: `first`, `second`, `third`, `fourth`, `last`. O padrão é `first`. Opcional e usado se **type** for `relativeMonthly` ou `relativeYearly`. |
|interval|Int32|O número de unidades entre ocorrências, onde as unidades podem ser em dias, semanas, meses ou anos, dependendo de **type**. Obrigatório. |
|month|Int32|O mês em que o evento ocorre.  É um número entre 1 e 12.|
|type|recurrencePatternType|O tipo de padrão da recorrência: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly` e `relativeYearly`. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/recurrencepattern.md/microsoft.graph.recurrencePattern/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->

