---
title: Atualizar autenticaçãoMethodsPolicy
description: Atualize as propriedades de um objeto authenticationMethodsPolicy.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 20f1cd2abb733876c5b8c82dacc620804292019c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038493"
---
# <a name="update-authenticationmethodspolicy"></a>Atualizar autenticaçãoMethodsPolicy
Namespace: microsoft.graph

Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.AuthenticationMethod|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do objeto [authenticationMethodConfigurations](../resources/authenticationmethodconfiguration.md) para solicitar que os usuários configurarem métodos de autenticação direcionados. 

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
    "authenticationMethodConfigurations": [
        {
            "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
            "id": "Fido2",
            "state": "disabled",
            "isSelfServiceRegistrationAllowed": false,
            "isAttestationEnforced": false,
            "keyRestrictions": {
                "isEnforced": false,
                "enforcementType": "block",
                "aaGuids": []
            }
        }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationmethodspolicy-java-snippets.md)]
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
