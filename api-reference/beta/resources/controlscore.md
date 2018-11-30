---
title: " tipo de recurso de controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034472"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso de controlScore

Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   String  |   Nome exclusivo do controle |
|   score   |   Duplo  |  Locatário alcançado e pontuação para o controle (ele diariamente varia dependendo de operações de Inquilino no controle). |
|   controlCategory |   String  |  Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura). |
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
