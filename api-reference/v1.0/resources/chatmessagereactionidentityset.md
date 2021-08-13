---
title: Tipo de recurso chatMessageReactionIdentitySet
description: Representa um usuário que reagia a uma mensagem em um chat ou canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59b1e110f5d74fdf4883cf7e59adfe5aacdf8b88fcd6e5e6da5728cc2e948f9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189876"
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

