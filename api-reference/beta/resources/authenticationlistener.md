---
title: Tipo de recurso authenticationListener
description: Define o ouvinte a ser avaliada durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41114f69bb169922b5594ee5cbbcdb236edfb0d0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159161"
---
# <a name="authenticationlistener-resource-type"></a>Tipo de recurso authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um ouvinte a ser avaliada quando um evento de autenticação ocorre em uma experiência de autenticação. Um authenticationListener é abstrato e é a classe base dos vários tipos de ouvintes que você pode avaliar durante um evento de autenticação. 

Você pode criar [um invokeUserFlowListener para](../resources/invokeuserflowlistener.md) o evento onSignUpStart. Isso associa um aplicativo a um fluxo de usuário, habilitando um processo de inscrição [de autoatendenciamento.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) Depois que um aplicativo é associado a um fluxo de usuário, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[Coleção authenticationListener](../resources/authenticationlistener.md)|Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.|
|[Criar authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Crie um novo objeto authenticationListener para o evento onSignupStart.|
|[Atualizar authenticationListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|Atualize o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Colocar authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|Substitua as propriedades de um objeto authenticationListener.|
|[Obter authenticationListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|Obter o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|
|[Excluir authenticationListener](../api/authenticationlistener-delete.md)|Nenhum(a)|Exclua o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da ação.|
|prioridade|Int32|A prioridade do ouvinte. Determina a ordem de avaliação quando um evento tem vários ouvintes. A prioridade é avaliada de baixo para alto.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado. Atualmente, isso está limitado a avaliações baseadas no aplicativo ao usuário que está autenticando.|

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
