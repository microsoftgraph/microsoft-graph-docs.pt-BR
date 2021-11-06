---
title: Tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5fa0fac27d8dfaacb27572476ab49e80cb3832e
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805543"
---
# <a name="lobbybypasssettings-resource-type"></a>Tipo de recurso lobbyBypassSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais participantes podem ignorar o lobby da reunião.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo    | Descrição                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby. Opcional.|
| isDialInBypassEnabled | Booliano | Especifica se os chamadores de discagem sempre podem ou não ignorar o lobby. Opcional. |

### <a name="lobbybypassscope-values"></a>valores lobbyBypassScope

| Valor                    | Descrição     |
| ------------------------ | --------------------------------------------------- |
| organizer | Somente o organizador é admitido na reunião e ignora o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organização | Somente os participantes da mesma empresa e **convidados** são admitidos na reunião e ignoram o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organizationAndFederated | Somente os participantes da mesma empresa ou organização confiável e convidados são admitidos na reunião e ignoram o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| everyone | Todos são admitidos na reunião. Nenhum participante é colocado no lobby da reunião. |
| invited | Somente as pessoas convidadas pelo organizador são internadas na reunião e ignoram o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| organizationExcludingGuests |  Somente os participantes da mesma empresa são admitidos na reunião e ignoram o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

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
