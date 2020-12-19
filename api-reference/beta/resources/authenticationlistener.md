---
title: tipo de recurso authenticationListener
description: Define o ouvinte a ser avaliado durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d89d7660fc2580b8fad185633b6b819df1a41aaf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720061"
---
# <a name="authenticationlistener-resource-type"></a>tipo de recurso authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um ouvinte a ser avaliado quando um evento de autenticação ocorrer em uma experiência de autenticação. Um authenticationListener é abstrato e é a classe base dos vários tipos de ouvintes que você pode avaliar durante um evento de autenticação. 

Você pode criar um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart.. Isso associa um aplicativo a um fluxo de usuário, habilitando, portanto, o processo de [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) . Depois que um aplicativo é associado a um fluxo de usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que Provisione uma conta de convidado.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|coleção [authenticationListener](../resources/authenticationlistener.md)|Obtenha a coleção de recursos authenticationListener com suporte pelo evento onSignupStart.|
|[Criar authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Criar um novo objeto authenticationListener para o evento onSignupStart.|
|[Atualizar authenticationListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|Atualize o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Colocar authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|Substitua as propriedades de um objeto authenticationListener.|
|[Obter authenticationListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|Obtenha o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Excluir authenticationListener](../api/authenticationlistener-delete.md)|Nenhum|Exclua o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da ação.|
|prioridade|Int32|A prioridade do ouvinte. Determina a ordem de avaliação quando um evento tem vários ouvintes. A prioridade é avaliada de baixo para alto.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado. No momento, isso está limitado a avaliações com base no aplicativo para o qual o usuário está se Autenticando.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
