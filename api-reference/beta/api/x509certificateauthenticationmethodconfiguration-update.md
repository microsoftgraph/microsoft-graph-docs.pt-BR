---
title: Atualizar x509CertificateAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto x509CertificateAuthenticationMethodConfiguration.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 72d2f549ef6a6a01434c90e14ed8da39f70fde55
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397509"
---
# <a name="update-x509certificateauthenticationmethodconfiguration"></a>Atualizar x509CertificateAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do método de autenticação [de certificado X.509](../resources/x509certificateauthenticationmethodconfiguration.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

Para cenários delegados, o administrador precisa de uma das seguintes funções [do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador de Política de Autenticação
* Administrador Global

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]
As propriedades a seguir podem ser atualizadas.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`. Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|certificateUserBindings|[Coleção x509CertificateUserBinding](../resources/x509certificateuserbinding.md)|Define campos no certificado X.509 que mapeiam para atributos do objeto de usuário do Azure AD para vincular o certificado ao usuário. A **prioridade** do objeto determina a ordem na qual a associação é realizada. A primeira associação que corresponde será usada e o restante ignorado. |
|authenticationModeConfiguration|[x509CertificateAuthenticationModeConfiguration](../resources/x509certificateauthenticationmodeconfiguration.md)|Define configurações de autenticação forte. Essa configuração inclui o modo de autenticação padrão e as diferentes regras para fortes vinculações de autenticação. |

>**Observação:** A `@odata.type` propriedade com um valor de `#microsoft.graph.x509CertificateAuthenticationMethodConfiguration` deve ser incluída no corpo.


## <a name="response"></a>Resposta

Se tiver êxito, este método `204 No Content` retornará um código de resposta e um [objeto x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação de atualização com as seguintes configurações:

+ Habilita o método de autenticação de certificado x509 no locatário.
+ Configura apenas uma associação de usuário entre o **certificado PrincipalName** e as propriedades do Azure AD **onPremisesUserPrincipalName** .
+ Define a autenticação multifato como requisito.
+ Configura as regras de associação para o método de autenticação forte em relação ao tipo de regra.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_x509certificateauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
    "id": "X509Certificate",
    "state": "enabled",
    "certificateUserBindings": [
        {
            "x509CertificateField": "PrincipalName",
            "userProperty": "onPremisesUserPrincipalName",
            "priority": 1
        }
    ],
    "authenticationModeConfiguration": {
        "x509CertificateAuthenticationDefaultMode": "x509CertificateMultiFactor",
        "rules": [
            {
                "x509CertificateRuleType": "issuerSubject",
                "identifier": "CN=ContosoCA,DC=Contoso,DC=org ",
                "x509CertificateAuthenticationMode": "x509CertificateMultiFactor"
            },
            {
                "x509CertificateRuleType": "policyOID",
                "identifier": "1.2.3.4",
                "x509CertificateAuthenticationMode": "x509CertificateMultiFactor"
            }
        ]
    },
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false
        }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-x509certificateauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-x509certificateauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-x509certificateauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-x509certificateauthenticationmethodconfiguration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 204 No Content
```

