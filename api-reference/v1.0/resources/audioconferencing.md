---
title: tipo de recurso audioConferencing
description: Representa informações de acesso de telefone de uma reunião online.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d2eab9732660f53c7e003b49f6c6ca780c8a4610
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865667"
---
# <a name="audioconferencing-resource-type"></a>tipo de recurso audioConferencing

Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | Uma URL para a página da Web acessível externamente que contém informações de discagem. |
| ID        | String  | A ID de conferência da reunião online.      |
| tollFreeNumber      | String  | O número de chamada gratuita que se conecta ao provedor de conferência de áudio.              |
| tollNumber          | String  | O número de chamada tarifada que se conecta ao provedor de conferência de áudio.                   |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "ConferenceId": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
