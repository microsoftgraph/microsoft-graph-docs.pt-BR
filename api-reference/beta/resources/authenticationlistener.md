---
title: Tipo de recurso authenticationListener
description: Define o ouvinte a ser avaliada durante um evento de autenticação.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5528dda667d225d8963ac476542122e2ec8c48c3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766492"
---
# <a name="authenticationlistener-resource-type"></a>Tipo de recurso authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um ouvinte a ser avaliada quando um evento de autenticação acontece em uma experiência de autenticação. Um authenticationListener é abstrato e é a classe base dos vários tipos de ouvintes que você pode avaliar durante um evento de autenticação. 

Você pode criar [um invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart.. Isso associa um aplicativo a um fluxo de usuário, portanto, habilitando um processo de [inscrição de autoatendenciamento.](/azure/active-directory/external-identities/self-service-sign-up-overview) Depois que um aplicativo é associado a um fluxo de usuários, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[Coleção authenticationListener](../resources/authenticationlistener.md)|Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.|
|[Criar authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Crie um novo objeto authenticationListener para o evento onSignupStart.|
|[Atualizar authenticationListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|Atualize o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Colocar authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|Substitua as propriedades de um objeto authenticationListener.|
|[Obter authenticationListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|Obter o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Excluir authenticationListener](../api/authenticationlistener-delete.md)|Nenhum|Exclua o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da ação.|
|prioridade|Int32|A prioridade do ouvinte. Determina a ordem de avaliação quando um evento tem vários ouvintes. A prioridade é avaliada de baixo para alto.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado. No momento, isso está limitado a avaliações com base no aplicativo ao que o usuário está autenticando.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
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
