---
title: Atualizar authenticationListener
description: Atualize o ouvinte definido para um evento no pipeline de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 65e5fa8252bdb4b25c1992282f655f532f66e1f3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438425"
---
# <a name="update-authenticationlistener"></a>Atualizar authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize [a authenticationListener definida](../resources/authenticationlistener.md) para um evento no pipeline de autenticação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.ReadWrite.ApplicationConfiguration|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto authenticationListener.](../resources/authenticationlistener.md)

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [invokeUserFlowAction](../resources/invokeuserflowlistener.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Prioridade|Int32|A prioridade do ouvinte. Determina a ordem de avaliação quando um evento tem vários ouvintes. A prioridade é avaliada de baixo para alto.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado. No momento, isso está limitado a avaliações com base no aplicativo ao que o usuário está autenticando.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_onsignupstart"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
  "priority": 101
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
