---
title: Tipo de recurso chatViewpoint
description: Representa propriedades específicas do usuário de um chat.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d9efb70dec447bf2f3c504a05245f67944783f6
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131921"
---
# <a name="chatviewpoint-resource-type"></a>Tipo de recurso chatViewpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades específicas do usuário de um [chat](../resources/chat.md). Essas propriedades podem mudar com base em quem é o chamador da API.

> **Observação:** Atualmente, somente a [operação de chats](../api/chat-list.md) lista suporta **chatViewpoint**.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|IsHidden|Booleano|Indica se o chat está oculto para o usuário atual.|
|lastMessageReadDateTime|DateTimeOffset|Representa a dateTime up até a qual o usuário atual leu [chatMessages](../resources/chatmessage.md) em um chat específico.|

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
  "isHidden": "Boolean",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

