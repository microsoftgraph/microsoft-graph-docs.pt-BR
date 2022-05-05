---
title: 'signIn: confirmCompromised'
description: Permite que você marque Azure AD eventos de entrada como arriscados para Azure AD Identity Protection.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 226a9986402ce315b77472ea1f37062f9e1f6753
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212819"
---
# <a name="signin-confirmcompromised"></a>signIn: confirmCompromised
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permite que os administradores marquem um evento no Azure AD logs de entrada como arriscados. Os eventos marcados como arriscados por um administrador são imediatamente sinalizados como de alto risco no Azure AD Identity Protection, substituindo os estados de risco anteriores. Os administradores podem confirmar se os eventos sinalizados como arriscados pelo Azure AD Identity Protection são de fato arriscados ou podem marcar eventos não marcados como arriscados. 

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityRiskyUser.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|IdentityRiskyUser.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /auditLogs/signIns/confirmCompromised
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|requestIds|Conjunto de cadeias de caracteres|As IDs dos eventos de entrada que devem ser marcados como arriscados para Azure AD Identity Protection.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "signinthis.confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/signIns/confirmCompromised
Content-Type: application/json

{
  "requestIds": [
    "f01c6af6-6683-4a37-a945-0a925501eede",
    "42bf60ac-d0cb-4206-aa5c-101884298f55",
    "f09c8f14-8d8e-42cf-8a7e-732b0594e79b"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/signinthisconfirmcompromised-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/signinthisconfirmcompromised-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/signinthisconfirmcompromised-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/signinthisconfirmcompromised-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/signinthisconfirmcompromised-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

