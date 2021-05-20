---
title: Tipo de recurso invokeUserFlowListener
description: Um ouvinte usado para invocar um fluxo de usuário durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89f990ab4692ec7fd4d6ce3b94ee4c4d4846c6c4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547208"
---
# <a name="invokeuserflowlistener-resource-type"></a>Tipo de recurso invokeUserFlowListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode criar [um invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart. Isso associa um aplicativo a um fluxo de usuário, que permite que identidades externas [se inscrevam](/azure/active-directory/external-identities/self-service-sign-up-overview) no aplicativo. Depois que um aplicativo é associado a um fluxo de usuários, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.

Herda da autenticação de tipo base [abstrataListener](../resources/authenticationlistener.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da ação. Herdado de [authenticationListener](../resources/authenticationlistener.md).|
|prioridade|Int32|A prioridade da ação usada para determinar uma de várias ações aplicáveis. Herdado de [authenticationListener](../resources/authenticationlistener.md).|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtrar com base na origem da autenticação usada para determinar se o ouvinte é executado. Herdado de [authenticationListener](../resources/authenticationlistener.md).|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|O fluxo do usuário que é invocado quando essa ação é executada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```
