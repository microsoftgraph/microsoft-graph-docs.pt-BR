---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma coleção de objetos userConsentRequest para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9c01fd4e752bca0fe9518553f52312e523da3a3
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697898"
---
# <a name="appconsentrequest-resource-type"></a>Tipo de recurso appConsentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) para um aplicativo específico.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appConsentRequests](../api/appconsentrequest-list.md)|[Coleção appConsentRequest](../resources/appconsentrequest.md)|Recupere uma coleção de [objetos appConsentRequest](appconsentrequest.md) e suas propriedades.|
|[Obter appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)|
|[filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appDisplayName|String|O nome de exibição do aplicativo para o qual o consentimento é solicitado. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
|appId|String|O identificador do aplicativo. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
|consentType|String|O tipo de consentimento da solicitação. Os valores possíveis são: `Static`   e  `Dynamic` . Elas representam permissões estáticas e dinâmicas, respectivamente, solicitadas no fluxo de trabalho de consentimento. Suporta `$filter` ( `eq` somente) e `$orderby` . Obrigatório.|
|id|String|O identificador da solicitação de consentimento do aplicativo. Obrigatório.|
|pendingScopes|[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)|Uma lista de escopos pendentes aguardando aprovação. Isso será vazio se o consentType for `Static` . Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|userConsentRequests|[Coleção userConsentRequest](../resources/userconsentrequest.md)|Uma lista de solicitações pendentes de consentimento do usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

