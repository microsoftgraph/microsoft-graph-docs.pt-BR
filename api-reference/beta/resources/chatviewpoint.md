---
title: Tipo de recurso chatViewpoint
description: Representa propriedades específicas do usuário de um chat.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236289"
---
# <a name="chatviewpoint-resource-type"></a>Tipo de recurso chatViewpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades específicas do usuário de um [chat](../resources/chat.md). Essas propriedades podem mudar com base em quem é o chamador da API.

> **Observação:** Atualmente, somente a operação [de chats de lista](../api/chat-list.md) suporta **chatViewpoint**.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastMessageReadDateTime|DateTimeOffset|Representa a dateTime up até a qual o usuário de chamada leu [chatMessages](../resources/chatmessage.md) em um chat específico.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

