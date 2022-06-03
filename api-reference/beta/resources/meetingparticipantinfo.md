---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2222c32db1f4dcee27fb4e3c88100d5e32788f60
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883863"
---
# <a name="meetingparticipantinfo-resource-type"></a>Tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um participante em uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo             | Descrição                 |
| :------- | :-------------------- | :------------------------------ |
| Identidade | [identitySet](identityset.md) | Informações de identidade do participante.           |
| Upn      | String                        | Nome principal do usuário do participante.             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | Especifica a função do participante na reunião.|

### <a name="onlinemeetingrole-values"></a>Valores onlineMeetingRole

A tabela a seguir lista os membros de [uma enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter `coorganizer` o valor nessa enumeração evolvável.

| Valor              | Descrição                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | A função do participante é participante. Esse valor se aplica a todas as reuniões.   |
| Apresentador           | A função do participante é apresentador. Esse valor se aplica a reuniões com **allowedPresenter** definido como `roleIsPresenter`ou a um evento ao vivo do Teams. |
| Produtor            | A função do participante é produtor. Esse valor se aplica somente ao evento ao vivo do Teams.  |
| coorganizador | A função do participante é co-organizador. Esse valor se aplica a todas as reuniões, exceto ao evento ao vivo do Teams. |
| unknownFutureValue | Valor de sentinel de enumeração evolvável. Não usar. |

> [!TIP]
>
> Para definir a **função de apresentador** de um participante da reunião ao criar ou atualizar um [onlineMeeting](onlinemeeting.md), o valor de **allowedPresenters** também deve ser definido como `roleIsPresenter`.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


