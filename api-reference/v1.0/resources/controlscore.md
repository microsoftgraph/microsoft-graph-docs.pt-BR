---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc3de6363784f62792d7c4e56906c79ed1be0c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531768"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso controlScore

Namespace: microsoft.graph

Contém uma pontuação de locatário e uma descrição para um controle individual.

## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|controlName|String|Controlar o nome exclusivo.|
|score|Duplo|A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).|
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
