---
title: Tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: db525d4d3a4f2999dd637745532789043b4f68df
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884164"
---
# <a name="lobbybypasssettings-resource-type"></a>Tipo de recurso lobbyBypassSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais participantes podem ignorar o lobby da reunião.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo    | Descrição                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | Especifica o tipo de participantes que são admitidos automaticamente em uma reunião, ignorando o lobby. Opcional.|
| isDialInBypassEnabled | Booliano | Especifica se os chamadores de discagem sempre devem ou não ignorar o lobby. Opcional. |

### <a name="lobbybypassscope-values"></a>valores de lobbyBypassScope

A tabela a seguir lista os membros de [uma enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta enumeração evolvável: `invited`, `organizationExcludingGuests`.

| Valor                    | Descrição     |
| ------------------------ | --------------------------------------------------- |
| organizer | Somente o organizador é admitido na reunião e ignora o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organization | Somente os participantes da mesma empresa e **convidados** são admitidos na reunião e ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organizationAndFederated | Somente os participantes da mesma empresa ou organização confiável e convidados são admitidos na reunião e ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| Todos | Todos são admitidos na reunião. Nenhum participante é colocado no lobby da reunião. |
| Convidado | Somente as pessoas que o organizador convida são admitidos na reunião e ignoram o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organizationExcludingGuests |  Somente os participantes da mesma empresa são admitidos na reunião e ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| unknownFutureValue | Valor de sentinel de enumeração evolvável. Não usar. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
