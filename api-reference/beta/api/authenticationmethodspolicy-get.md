---
title: Obter authenticationMethodsPolicy
description: Leia as propriedades e as relações de um objeto authenticationMethodsPolicy.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 95454980e17b8c531eca7af41d6bd80126e6317f
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2022
ms.locfileid: "62238984"
---
# <a name="get-authenticationmethodspolicy"></a>Obter authenticationMethodsPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.AuthenticationMethod|

Para cenários delegados, o administrador precisa de uma das seguintes funções [do Azure AD:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Leitor global
* Administrador de Política de Autenticação
* Administrador Global

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método não dá suporte a parâmetros de consulta opcionais.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-authenticationmethodspolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-authenticationmethodspolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
    "id": "authenticationMethodsPolicy",
    "displayName": "Authentication Methods Policy",
    "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
    "lastModifiedDateTime": "2022-01-26T10:47:26.6044384Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 1,
            "state": "default",
            "excludeTargets": [],
            "includeTargets": [
                {
                    "id": "all_users",
                    "targetType": "group",
                    "targetedAuthenticationMethod": "microsoftAuthenticator"
                }
            ]
        }
    },
    "authenticationMethodConfigurations@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations",
    "authenticationMethodConfigurations": [
        {
            "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
            "id": "Fido2",
            "state": "disabled",
            "isSelfServiceRegistrationAllowed": true,
            "isAttestationEnforced": true,
            "keyRestrictions": {
                "isEnforced": false,
                "enforcementType": "block",
                "aaGuids": []
            },
            "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('Fido2')/microsoft.graph.fido2AuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
            "id": "MicrosoftAuthenticator",
            "state": "disabled",
            "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('MicrosoftAuthenticator')/microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false,
                    "authenticationMode": "any",
                    "outlookMobileAllowedState": "default",
                    "displayAppInformationRequiredState": "default",
                    "numberMatchingRequiredState": "default"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
            "id": "Sms",
            "state": "enabled",
            "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('Sms')/microsoft.graph.smsAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false,
                    "isUsableForSignIn": true
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
            "id": "TemporaryAccessPass",
            "state": "disabled",
            "defaultLifetimeInMinutes": 60,
            "defaultLength": 8,
            "minimumLifetimeInMinutes": 60,
            "maximumLifetimeInMinutes": 480,
            "isUsableOnce": false,
            "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('TemporaryAccessPass')/microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
            "id": "Email",
            "state": "enabled",
            "allowExternalIdToUseEmailOtp": "default",
            "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('Email')/microsoft.graph.emailAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": []
        }
    ]
}
```
