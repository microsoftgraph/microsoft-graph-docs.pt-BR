---
title: Listar credentialUserRegistrationDetails
description: Obter uma lista de objetos credentialUserRegistrationDetails para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136665"
---
# <a name="list-credentialuserregistrationdetails"></a>Listar credentialUserRegistrationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Reports.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**. Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso credentialUserRegistrationDetails.](../resources/credentialuserregistrationdetails.md)

| Propriedades | Descrição e exemplo |
| --------- | ----------------------- |
| userDisplayName | Filtrar por nome de usuário. Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`. Operadores de filtro com suporte: `eq` e `startswith()` . Dá suporte a maiúsculas e minúsculas. |
| userPrincipalName | Filtrar pelo nome principal do usuário. Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`. Operadores de filtro com suporte: `eq` e `startswith()` . Dá suporte a maiúsculas e minúsculas. |
| authMethods | Filtrar pelos métodos de autenticação usados durante o registro. Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`. Operadores de filtro com suporte: `eq` . |
| isRegistered | Filtro para usuários que se registraram para redefinição de senha de autoatendado (SSPR). Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`. Operadores de filtro com suporte: `eq` . |
| isEnabled | Filtro para usuários que foram habilitados para SSPR. Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`. Operadores de filtter com suporte: `eq` . |
| isCapable | Filtro para usuários que estão prontos para executar a redefinição de senha ou autenticação multifatória (MFA). Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`. Operadores de filtro com suporte: `eq` |
| isMfaRegistered | Filtro para usuários que estão registrados para MFA. Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`. Operadores de filtro com suporte: `eq` . |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades são retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


