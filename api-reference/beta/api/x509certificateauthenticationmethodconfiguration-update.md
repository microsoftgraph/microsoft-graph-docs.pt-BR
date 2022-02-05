---
title: Atualizar x509CertificateAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto x509CertificateAuthenticationMethodConfiguration.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
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
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
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
    "state": "disabled",
    "certificateUserBindings": [{
            "x509CertificateField": "PrincipalName",
            "userProperty": "onPremisesUserPrincipalName",
            "priority": 1
        },
        {
            "x509CertificateField": "RFC822Name",
            "userProperty": "userPrincipalName",
            "priority": 2
        }
    ],
    "authenticationModeConfiguration": {
        "x509CertificateAuthenticationDefaultMode": "x509CertificateSingleFactor",
        "rules": []
    },
    "includeTargets": [{
        "targetType": "group",
        "id": "all_users",
        "isRegistrationRequired": false
    }]
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```

