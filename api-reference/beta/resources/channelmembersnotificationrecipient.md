---
title: Tipo de recurso channelMembersNotificationRecipient
description: Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade. O destinatário consiste nos membros do canal.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211211"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a>Tipo de recurso channelMembersNotificationRecipient

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade. O destinatário consiste nos membros do canal.

Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo   | Descrição                                            |
| :-------- | :----- | :----------------------------------------------------- |
| teamId    | String | O identificador da equipe no qual o canal reside. |
| channelId | String | O identificador do canal.                              |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
