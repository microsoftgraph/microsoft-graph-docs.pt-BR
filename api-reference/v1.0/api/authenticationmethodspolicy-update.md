---
title: Atualizar autenticaçãoMethodsPolicy
description: Atualize as propriedades de um objeto authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 89c3f68a27ca67fdae0560fc43f02356ff93e5f1
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2021
ms.locfileid: "53547557"
---
# <a name="update-authenticationmethodspolicy"></a>Atualizar autenticaçãoMethodsPolicy
Namespace: microsoft.graph

Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
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


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content

```
