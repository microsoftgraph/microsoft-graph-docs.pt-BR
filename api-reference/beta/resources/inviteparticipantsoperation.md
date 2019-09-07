---
title: tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793017"
---
# <a name="inviteparticipantsoperation-resource-type"></a>tipo de recurso inviteParticipantsOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | O contexto do cliente.                                                                                                                               |
| createdDateTime                | DateTimeOffset              | A hora em que a gravação foi criada.                                                                                                          |
| id                             | Cadeia de caracteres                      | A ID da operação do servidor. Somente leitura. Servidor gerado.                                                                                             |
| lastActionDateTime             | DateTimeOffset              | A hora da última ação da operação.                                                                                                     |
| participants | coleção [invitationParticipantInfo](invitationParticipantInfo.md) | Os participantes a serem convidados. |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura. Servidor gerado.                                                                                             |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura. Servidor gerado.                                                 |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
