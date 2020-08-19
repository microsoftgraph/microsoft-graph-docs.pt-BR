---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2b718851d1a27c3317a0ce77554be7ea3f8906a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811494"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso controlScore

Namespace: microsoft.graph

Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   String  |   Controlar o nome exclusivo |
|   Pontuação   |   Duplo  |  A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle). |
|   controlCategory |   String  |  Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura). |
|   description |   String  |  Descrição do controle. |

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
