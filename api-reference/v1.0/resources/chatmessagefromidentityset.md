---
title: Tipo de recurso chatMessageFromIdentitySet
description: Representa o remetente de uma mensagem em um chat ou canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30b8c8add62c94ff16fe5e560a78ec5c9c95627d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211059"
---
# <a name="chatmessagefromidentityset-resource-type"></a>Tipo de recurso chatMessageFromIdentitySet

Namespace: microsoft.graph

Representa o remetente de uma [mensagem em](../resources/chatmessage.md) um chat ou canal. Esse objeto pode ser para uma mensagem que foi excluída ou enviada pelo sistema Microsoft Teams interno; por exemplo, mensagens de evento para adição `null` de membros.


Herda de [identitySet](../resources/identityset.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa o aplicativo (por exemplo, bot) que enviou a mensagem.|
|device|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não usado.|
|user|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa o usuário que enviou a mensagem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

