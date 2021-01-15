---
title: Atualizar authenticationListener
description: Atualize o ouvinte definido para um evento no pipeline de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5acb660843bf0b7a60fd66886841ab4c490f396
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872391"
---
# <a name="update-authenticationlistener"></a>Atualizar authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize [o authenticationListener definido](../resources/authenticationlistener.md) para um evento no pipeline de autenticação.

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
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Filtrar com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado. Atualmente, isso está limitado a avaliações baseadas no aplicativo ao usuário que está autenticando.|

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
