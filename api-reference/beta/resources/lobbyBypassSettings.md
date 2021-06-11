---
title: Tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c6d530765e1bc356486f0b8893c69c445c07181f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896680"
---
# <a name="lobbybypasssettings-resource-type"></a>Tipo de recurso lobbyBypassSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais participantes podem ignorar o lobby da reunião.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo    | Descrição                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby. Os valores possíveis são listados na tabela a seguir. Opcional.|
| isDialInBypassEnabled | Boolean | Especifica se os chamadores de discagem sempre podem ou não ignorar o lobby. Opcional. | 

### <a name="lobbybypassscope-values"></a>valores lobbyBypassScope

| Valor                    | Descrição                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | Somente o organizador é admitido na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião.                                                                                                         |
| organization             | Somente os participantes da mesma empresa são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião.                                                                              |
| organizationAndFederated | Somente os participantes da mesma empresa ou organização confiável são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados no lobby da reunião. |
| everyone                 | Todos são admitidos na reunião. Nenhum participante é colocado no lobby da reunião.                                                                                                                   |
| unknownFutureValue       | Valor futuro desconhecido.                                                                                                                                     |

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
