---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973930"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso controlScore

Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   String  |   Controlar o nome exclusivo |
|   score   |   Duplo  |  A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle). |
|   controlCategory |   String  |  Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura). |
|   descrição |   String  |  Descrição do controle. |

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
