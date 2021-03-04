---
title: Obter authenticationListener
description: Leia as propriedades e as relações de um objeto authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e6cacb31a31963457c2e37fd9a63d1c0eeea2c6c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438481"
---
# <a name="get-authenticationlistener"></a>Obter authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter a autenticação [especificadaListener definida](../resources/authenticationlistener.md) para o evento onSignupStart no pipeline de autenticação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte ao parâmetro de consulta OData para expandir os detalhes `$expand` de um invokeUserFlowListener. Confira abaixo um exemplo. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-an-authenticationlistener-by-id"></a>Exemplo 1: Obter um authenticationListener por id

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
   }
}
```

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a>Exemplo 2: Expanda invokeUserFlowListener para uma autenticação específicaListener

O exemplo a seguir obtém o ouvinte por id do evento onSignupStart e expande o fluxo de usuário invocado.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invokeUserFlowListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
  },
  "userFlow": {
      "id": "B2X_1_Partner",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationListener",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
