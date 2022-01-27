---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5182eb1b281eadf314f50e3fe219addd9a3ee3ba
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2022
ms.locfileid: "62238858"
---
# <a name="get-fido2authenticationmethodconfiguration"></a>Obter fido2AuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações do objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) [](../resources/authenticationmethodspolicies-overview.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodConfigurations/$entity",
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
}
```

