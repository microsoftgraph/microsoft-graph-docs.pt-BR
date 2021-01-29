---
title: 'authenticationMethodsRoot: usersRegisteredByFeature'
description: Obter o número de usuários capazes de autenticação multifa factor, redefinição de senha de autoatendado e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 3006ca1dafc1eda4774879144673cb804be552e5
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052550"
---
# <a name="authenticationmethodsroot-usersregisteredbyfeature"></a>authenticationMethodsRoot: usersRegisteredByFeature
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o número de usuários capazes de autenticação multifa factor, redefinição de senha de autoatendado e autenticação sem senha.

## <a name="permissions"></a>Permissões
As permissões a seguir são necessárias para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Reports.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

Para acessar a API, [uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) é necessária:

* Leitor de relatórios
* Leitor de segurança
* Administrador de segurança
* Leitor global
* Administração global

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByFeature
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|includedUserTypes|includedUserTypes|Tipo de usuário. Os valores possíveis são: `all`, `member`, `guest`.|
|includedUserRoles|includedUserRoles|Tipo de função de usuário. Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.|

O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:

* Administrador global
* Administrador de segurança
* Administrador de acesso condicional
* Administrador do Exchange
* Administrador do SharePoint
* Administrador de help desk
* Administrador de faturamento
* Administrador de usuários
* Administrador de autenticação

O valor inclui todas as funções de administrador do `admin` Azure AD. 

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta função retornará um código de resposta e um `200 OK` [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbyfeature"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
    "totalUserCount": 23123,
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationFeatureCounts": [{
            "feature": "ssprRegistered",
            "userCount": 23423
        },
        {
            "feature": "ssprEnabled",
            "userCount": 4234
        },
        {
            "feature": "ssprCapable",
            "userCount": 4234
        }, {
            "feature": "passwordlessRegistered",
            "userCount": 323
        },
        {
            "feature": "mfaCapable",
            "userCount": 3345
        }
    ]
}
```