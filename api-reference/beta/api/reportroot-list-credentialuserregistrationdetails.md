---
title: Listar credentialUserRegistrationDetails
description: Obter uma lista de objetos credentialUserRegistrationDetails para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: bbb4c1b71e596eebc4055732b0423c2b0fd55786
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871175"
---
# <a name="list-credentialuserregistrationdetails"></a>Listar credentialUserRegistrationDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.

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

Essa função suporta o parâmetro de consulta OData opcional **$Filter**. Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) .

| Propriedades | Descrição e exemplo |
| --------- | ----------------------- |
| userDisplayName | Filtrar por nome de usuário. Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`. Operadores de filtro suportados `eq`:, `startswith()`e. Dá suporte a maiúsculas e minúsculas. |
| userPrincipalName | Filtrar por nome principal do usuário. Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`. Operadores de filtro suportados `eq` : `startswith()`e. Dá suporte a maiúsculas e minúsculas. |
| authMethods | Filtrar pelos métodos de autenticação usados durante o registro. Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`. Operadores de filtro suportados `eq`:. |
| IsRegistered | Filtro para usuários que registraram a redefinição de senha de autoatendimento (SSPR). Por exemplo: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`. Operadores de filtro suportados `eq`:. |
| isEnabled | Filtro para usuários que foram habilitados para o SSPR. Por exemplo: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`. Operadores filtter com suporte `eq`:. |
| iscapable | Filtro para usuários que estão prontos para executar redefinição de senha ou a autenticação multifator (MFA). Por exemplo: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`. Operadores de filtro suportados:`eq` |
| isMfaRegistered | Filtro para usuários registrados para MFA. Por exemplo: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`. Operadores de filtro suportados `eq`:. |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
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
