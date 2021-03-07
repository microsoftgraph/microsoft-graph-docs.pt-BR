---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9462971d1c2694b3443c9b3a4e799a24362eee80
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515636"
---
# <a name="audioconferencing-resource-type"></a>Tipo de recurso audioConferencing

Namespace: microsoft.graph

Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Cadeia de caracteres  | Uma URL para a página da Web externamente acessível que contém informações de discagem. |
| conferenceId        | Cadeia de caracteres  | A ID da conferência da reunião online.      |
| tollFreeNumber      | Cadeia de caracteres  | O número gratuito que se conecta ao Provedor de Conferência de Áudio.              |
| tollNumber          | Cadeia de caracteres  | O número de telefone que se conecta ao Provedor de Conferência de Áudio.                   |

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
  "conferenceId": "String",
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

