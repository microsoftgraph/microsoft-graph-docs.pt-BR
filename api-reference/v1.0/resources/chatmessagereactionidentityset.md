---
title: Tipo de recurso chatMessageReactionIdentitySet
description: Representa um usuário que reagia a uma mensagem em um chat ou canal.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35b97d1b7fe470beced8daca4b92f5e1c167b467
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109392"
---
# <a name="chatmessagereactionidentityset-resource-type"></a>Tipo de recurso chatMessageReactionIdentitySet

Namespace: microsoft.graph

Representa um **usuário** que reagia a [uma mensagem](../resources/chatmessage.md) em um chat ou canal. Somente a `user` propriedade tem um valor.


Herda de [identitySet](../resources/identityset.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não definido porque os aplicativos não podem reagir às mensagens.|
|device|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não definido porque os dispositivos não podem reagir às mensagens.|
|usuário|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Detalhes sobre o usuário que reagia à mensagem.|

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

