---
title: Atualizar authenticationFlowsPolicy
description: Atualize a propriedade booleana selfServiceSignUp de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d81986c75cb636c45488d2fb35e69b05fdb06e2a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882858"
---
# <a name="update-authenticationflowspolicy"></a>Atualizar authenticationFlowsPolicy

Namespace: microsoft.graph

Atualize a propriedade **selfServiceSignUp** de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md). As propriedades **id**, **tipo** e **descrição** não podem ser modificadas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationFlows|
|Delegada (conta pessoal da Microsoft)|Não suportado|
|Aplicativo|Policy.ReadWrite.AuthenticationFlows|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, você pode fornecer uma representação JSON do objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).

A tabela a seguir mostra as propriedades obrigatórias ao atualizar [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)|Configuração de inscrição de autoatendimento.|

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

``` http
HTTP/1.1 204 No Content
```
