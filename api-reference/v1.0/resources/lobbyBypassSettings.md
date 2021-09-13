---
title: Tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d850b6335d3a3446516c4fccad1e1dd81518a189
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134735"
---
# <a name="lobbybypasssettings-resource-type"></a>Tipo de recurso lobbyBypassSettings

Namespace: microsoft.graph

Especifica quais participantes podem ignorar o lobby da reunião.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo             | Descrição                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values) | Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby. Os valores possíveis são listados na tabela a seguir. Opcional. |
| isDialInBypassEnabled | Booliano          | Especifica se os chamadores de discagem sempre podem ou não ignorar o lobby. Opcional.                                                                                   |

### <a name="lobbybypassscope-values"></a>valores lobbyBypassScope

| Valor                    | Descrição                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | Somente o organizador é admitido na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião.                                                   |
| organização             | Somente os participantes da mesma empresa são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião.                         |
| organizationAndFederated | Somente os participantes da mesma empresa ou organização confiável são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| everyone                 | Todos são admitidos na reunião. Nenhum participante é colocado no lobby da reunião.                                                                                         |
| unknownFutureValue       | Valor futuro desconhecido.                                                                                                                                                            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "String",
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
