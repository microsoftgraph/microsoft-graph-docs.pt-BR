---
title: Tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de longa duração, disparada por uma chamada para a API de convite para participantes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9aa707a68cccb7424cb6a2eabaa455ece784730478ce2469b3e2f70c40e5297e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196975"
---
# <a name="inviteparticipantsoperation-resource-type"></a>Tipo de recurso inviteParticipantsOperation

Namespace: microsoft.graph

Representa o status de uma operação de convite de participante de longa duração, disparada por uma chamada para a API de convite para participantes.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | Cadeia de caracteres                      | O contexto do cliente.                                                                                                                               |
| id                             | Cadeia de caracteres                      | A id da operação do servidor. Somente leitura.                                                                                              |
| participants | conjunto [invitationParticipantInfo](invitationParticipantInfo.md) | Os participantes a convidar. |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Apenas leitura.                                                                                             |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                  |

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
  "id": "String (identifier)",
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

