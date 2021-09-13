---
title: Tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de longa duração, disparada por uma chamada para a API de convite para participantes.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 24fb78d2c2dee1bcf902849f10eaf3d11a167426
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084388"
---
# <a name="inviteparticipantsoperation-resource-type"></a>Tipo de recurso inviteParticipantsOperation

Namespace: microsoft.graph

Representa o status de uma operação de convite de participante de longa duração, disparada por uma chamada para a API de convite para participantes.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | O contexto do cliente.                                                                                                                               |
| id                             | Cadeia de caracteres                      | A id da operação do servidor. Somente leitura.                                                                                              |
| participants | conjunto [invitationParticipantInfo](invitationParticipantInfo.md) | Os participantes a convidar. |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                                                                             |
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

