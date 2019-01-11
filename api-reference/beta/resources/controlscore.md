---
title: " tipo de recurso de controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891466"
---
#  <a name="controlscore-resource-type"></a>tipo de recurso de controlScore

Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   Cadeia de caracteres  |   Nome exclusivo do controle |
|   score   |   Duplo  |  Locatário alcançado e pontuação para o controle (ele diariamente varia dependendo de operações de Inquilino no controle). |
|   controlCategory |   Cadeia de caracteres  |  Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura). |
|   description |   Cadeia de caracteres  |  Descrição do controle. |

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
