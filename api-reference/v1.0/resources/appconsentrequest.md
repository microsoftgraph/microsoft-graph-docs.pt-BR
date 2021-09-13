---
title: Tipo de recurso appConsentRequest
description: Uma solicitação que representa uma coleção de objetos userConsentRequest para um aplicativo específico.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef5eed15ad094e35d4db49ee4e34def6de5f2861
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094433"
---
# <a name="appconsentrequest-resource-type"></a>Tipo de recurso appConsentRequest

Namespace: microsoft.graph

Uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) para um aplicativo específico.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appConsentRequests](../api/appconsentrequest-list.md)|[Coleção appConsentRequest](../resources/appconsentrequest.md)|Recupere uma coleção de [objetos appConsentRequest](appconsentrequest.md) e suas propriedades.|
|[Obter appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)|
|[filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Leia as propriedades dos [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status da solicitação de consentimento do usuário é `InProgress` . |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appDisplayName|Cadeia de caracteres|O nome de exibição do aplicativo para o qual o consentimento é solicitado. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
|appId|String|O identificador do aplicativo. Obrigatório. Suporta `$filter` ( `eq` somente) e `$orderby` . |
|id|String|O identificador da solicitação de consentimento do aplicativo. Obrigatório.|
|pendingScopes|[Coleção appConsentRequestScope](../resources/appconsentrequestscope.md)|Uma lista de escopos pendentes aguardando aprovação. Obrigatório.|

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
