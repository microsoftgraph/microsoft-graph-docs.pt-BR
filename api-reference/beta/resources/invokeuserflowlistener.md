---
title: tipo de recurso invokeUserFlowListener
description: Um ouvinte usado para invocar um fluxo de usuário durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720089"
---
# <a name="invokeuserflowlistener-resource-type"></a>tipo de recurso invokeUserFlowListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode criar um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart. Isso associa um aplicativo a um fluxo de usuário, que permite a [inscrição de autoatendimento de identidade externa](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) para o aplicativo. Depois que um aplicativo é associado a um fluxo de usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que Provisione uma conta de convidado.

Herda do tipo de base abstrato [authenticationListener](../resources/authenticationlistener.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da ação. Herdado de [authenticationListener](../resources/authenticationlistener.md).|
|prioridade|Int32|A prioridade da ação que é usada para determinar uma de várias ações aplicáveis. Herdado de [authenticationListener](../resources/authenticationlistener.md).|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é executado. Herdado de [authenticationListener](../resources/authenticationlistener.md).|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|userflow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|O fluxo do usuário que é chamado quando esta ação é executada.|

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
