---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c394bf0d75e9115f3cfe7ec44ff4978f716401d0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435989"
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

Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Administrador global


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
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


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
Content-length: 491

{
   "value":{
      "@odata.type":"#microsoft.graph.fido2AuthenticationMethodConfiguration",
      "id":"Fido2",
      "state":"enabled",
      "isSelfServiceRegistrationAllowed":true,
      "isAttestationEnforced":true,
      "keyRestrictions":{
         "isEnforced":false,
         "enforcementType":"block",
         "aaGuids":[
            
         ]
      },
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false,
            "useForSignIn":true
         }
      ]
   }
}
```

