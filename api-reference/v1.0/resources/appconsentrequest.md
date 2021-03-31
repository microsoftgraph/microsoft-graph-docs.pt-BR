---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma agregação de userConsentRequests para um aplicativo específico.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac7e9f2ea8e727a285016641bac10ea3d2e38f9b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469504"
---
# <a name="appconsentrequest-resource-type"></a>Tipo de recurso appConsentRequest

Namespace: microsoft.graph

Uma agregação de [userConsentRequests](../resources/userconsentrequest.md) para um aplicativo específico.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appConsentRequests](../api/appconsentrequest-list.md)|[Coleção appConsentRequest](../resources/appconsentrequest.md)|Obter uma lista dos [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.|
|[Obter appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)|
|[appConsentRequests: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Uma lista do [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appDisplayName|String|O nome de exibição do aplicativo para o qual o consentimento é solicitado. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
|appId|String|O identificador do aplicativo. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
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
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
