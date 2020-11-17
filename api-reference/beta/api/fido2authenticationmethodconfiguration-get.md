---
title: Obter fido2AuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e7c133c25d7770257423c803f640e00f23dc449
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086624"
---
# <a name="get-fido2authenticationmethodconfiguration"></a>Obter fido2AuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos do objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , que representa a [política de método de autenticação](../resources/authenticationmethodspolicies-overview.md) de chaves de segurança FIDO2 para o locatário do Azure Active Directory (Azure AD).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegada (conta Microsoft pessoal)|Sem suporte.|
|Aplicativo|Sem suporte.|

Para cenários delegados, o administrador precisa da seguinte [função](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

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

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) no corpo da resposta.

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

