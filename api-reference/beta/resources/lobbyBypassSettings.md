---
title: tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3723f6593547b75c60a82b8436995c931d64e436
ms.sourcegitcommit: 7dcae492d8b4707d068adca3a74732e25a8198e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2020
ms.locfileid: "47423678"
---
# <a name="lobbybypasssettings-resource-type"></a>tipo de recurso lobbyBypassSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais participantes podem ignorar o lobby da reunião.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo    | Descrição                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| scope                 | lobbyBypassScope  | Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby. Os valores possíveis estão listados na tabela a seguir. Opcional.|
| isDialInBypassEnabled | Boolean | Especifica se você deseja ou não permitir que chamadores de discagem ignorem o lobby. Opcional. | 

### <a name="lobbybypassscope-values"></a>valores de lobbyBypassScope

| Valor                    | Descrição                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | Somente o organizador é admitido na reunião, ignorando o lobby. Todos os outros participantes são colocados na sala de reunião.                                                                                                         |
| organization             | Somente os participantes da mesma empresa são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados na sala de reunião.                                                                              |
| organizationAndFederated | Somente os participantes da mesma empresa ou organização confiável são admitidos na reunião, ignorando o lobby. Todos os outros participantes são colocados na sala de reunião. |
| têm                 | Todos são admitidos na reunião. Nenhum participante é colocado na sala de reunião.                                                                                                                   |
| unknownFutureValue       | Valor de futuro desconhecido.                                                                                                                                     |

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
