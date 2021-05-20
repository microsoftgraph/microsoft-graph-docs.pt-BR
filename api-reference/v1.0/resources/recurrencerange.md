---
title: Tipo de recurso recurrenceRange
description: 'Descreve um intervalo de datas sobre o qual um event recorrente se repete. '
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0b7aa184981549f45c9c5d00e5c32cd5431123c2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547257"
---
# <a name="recurrencerange-resource-type"></a>Tipo de recurso recurrenceRange

Namespace: microsoft.graph

Descreve um intervalo de datas sobre o qual um [event](event.md) recorrente se repete.

É possível especificar o intervalo de datas para um evento recorrente de uma de três maneiras, dependendo do seu cenário. Como você deve sempre especificar um valor de **startDate** para o intervalo de datas, é possível especificar um evento recorrente que termina em uma data específica, que não termina ou que termina após um número específico de ocorrências. As ocorrências reais dentro do intervalo de datas sempre seguem o padrão de recorrência que você especifica para o evento recorrente. Um evento recorrente é sempre definido por seu [recurrencePattern](recurrencepattern.md) (com que frequência o evento se repete) e seu **recurrenceRange** (por quanto tempo o evento se repete).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|endDate|Data|A data para parar de aplicar o padrão de recorrência. Dependendo do padrão de recorrência do evento, a última ocorrência da reunião pode não ser essa data. Obrigatório se **type** for `endDate`.|
|numberOfOccurrences|Int32|O número de vezes para repetir o evento. Obrigatório e deve ser positivo se **type** for `numbered`.|
|recurrenceTimeZone|Cadeia de caracteres |Fuso horário das propriedades **startDate** e **endDate**. Opcional. Se a propriedade não for especificada, será usado o fuso horário do evento.|
|startDate|Data|A data para começar a aplicar o padrão de recorrência. A primeira ocorrência da reunião pode ser essa data ou posterior, dependendo do padrão de recorrência do evento. Deve ser o mesmo valor da propriedade **start** do [event](event.md) recorrente. Obrigatório.|
|type|recorrênciaRangeType|O intervalo de recorrência. Os valores possíveis são: `endDate`, `noEnd`, `numbered`. Obrigatório.|

Use a propriedade **type** para especificar os diferentes tipos de **recorrenceRange**. Observe as propriedades necessárias para cada tipo, conforme descrito na tabela a seguir.

| propriedade tipo  | Tipo de intervalo de recorrência | Descrição | Exemplo | Propriedades necessárias |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |Intervalo com data final | O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente entre **startDate** e **endDate**, incluindo essas datas. | Repita o evento no período entre 1º de junho de 2017 e 15 de junho de 2017. | **type**, **startDate**, **endDate** |
|`noEnd`  |Intervalo sem uma data final | O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente começando em **startDate**. | Repita o evento no intervalo de datas que começa em 1º de junho de 2017, indefinidamente. | **type**, **startDate** |
|`numbered`|Intervalo com número específico de ocorrências | O evento se repete para **numberOfOccurrences** com base no padrão de recorrência começando em **startDate**. | Repita o evento no período que começa em 1º de junho de 2017, para dez ocorrências.  | **type**, **startDate**, **numberOfOccurrences** |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->

