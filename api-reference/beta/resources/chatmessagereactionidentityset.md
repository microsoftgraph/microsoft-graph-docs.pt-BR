---
title: Tipo de recurso chatMessageReactionIdentitySet
description: Representa um usuário que reagia a uma mensagem em um chat ou canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 032b335656d768f505cdb673b56ef0955cf9ed58
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211195"
---
# <a name="chatmessagereactionidentityset-resource-type"></a>Tipo de recurso chatMessageReactionIdentitySet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um **usuário** que reagia a [uma mensagem](../resources/chatmessage.md) em um chat ou canal. Somente a `user` propriedade tem um valor.


Herda de [identitySet](../resources/identityset.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não definido porque os aplicativos não podem reagir às mensagens.|
|device|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não definido porque os dispositivos não podem reagir às mensagens.|
|user|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Detalhes sobre o usuário que reagia à mensagem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
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

