---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543375"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso controlScore

Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   String  |   Controlar o nome exclusivo |
|   score   |   Duplo  |  A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle). |
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
  "score": "String",
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
