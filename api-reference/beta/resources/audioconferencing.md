---
title: tipo de recurso de audioConferencing
description: Representa as informações de acesso telefônicas de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9bd8343f29a797a24044f02aa2a00bd098c35007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843621"
---
# <a name="audioconferencing-resource-type"></a>tipo de recurso de audioConferencing

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as informações de acesso telefônicas de um [onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Cadeia de caracteres  | Uma URL para a página da web acessível externamente que contém informações de discagem. |
| leaderPasscode      | Cadeia de caracteres  | A senha de líder necessária para conectar ao provedor de conferência de áudio.      |
| participantPasscode | Cadeia de caracteres  | A senha de participante necessária para conectar ao provedor de conferência de áudio. |
| tollFreeNumber      | Cadeia de caracteres  | O número de chamada gratuito para conectar ao provedor de conferência de áudio.              |
| tollNumber          | Cadeia de caracteres  | O número de Chamada Tarifada para conectar ao provedor de conferência de áudio.                   |

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
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
