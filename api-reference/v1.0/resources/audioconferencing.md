---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 36a21359c4c336b122856417021c5291de01d2c1c3fd704420cd2f234831136c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124581"
---
# <a name="audioconferencing-resource-type"></a>Tipo de recurso audioConferencing

Namespace: microsoft.graph

Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Cadeia de caracteres  | Uma URL para a página da Web externamente acessível que contém informações de discagem. |
| conferenceId        | String  | A ID da conferência da reunião online.      |
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

