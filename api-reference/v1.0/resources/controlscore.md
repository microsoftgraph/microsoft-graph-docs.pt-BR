---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e4470d1ce22f5ffbf3c805adc5328398d57d9fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056921"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso controlScore

Namespace: microsoft.graph

Contém uma pontuação de locatário e uma descrição para um controle individual.

## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|controlName|String|Controlar o nome exclusivo.|
|Pontuação|Duplo|A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).|
|controlCategory|String|Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).|
|description|String| Descrição do controle.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

