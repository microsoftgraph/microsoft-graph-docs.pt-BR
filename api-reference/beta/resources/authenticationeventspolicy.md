---
title: Tipo de recurso authenticationEventsPolicy
description: Os eventos de autenticação são usados para invocar fluxos de usuário em pontos específicos no fluxo de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6cd727ebe51bbb6d5ad2162b180c4fc891ff792a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443164"
---
# <a name="authenticationeventspolicy-resource-type"></a>Tipo de recurso authenticationEventsPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso que especifica os eventos na experiência de autenticação, com cada evento definindo ainda mais os tipos disponíveis de ouvintes que podem ser criados para o evento. Os eventos são inerentes à experiência de autenticação; esse recurso não é configurável pelo usuário.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ouvintes onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[Coleção authenticationListener](../resources/authenticationlistener.md)|Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.|
|[Criar authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Crie um novo objeto authenticationListener para o evento onSignupStart.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da política.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|onSignupStart|[Coleção authenticationListener](../resources/authenticationlistener.md)|Uma lista de ações aplicáveis a serem tomadas ao se inscrever.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
