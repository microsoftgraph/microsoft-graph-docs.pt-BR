---
title: Obter userRegistrationDetails
description: Leia as propriedades e as relações de um objeto userRegistrationDetails.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: b70b2557ca5ec9b0af2d0a7d5d9f714777b385f1
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201758"
---
# <a name="get-userregistrationdetails"></a>Obter userRegistrationDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto userRegistrationDetails.](../resources/userregistrationdetails.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|UserAuthenticationMethod.Read.All, AuditLog.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|UserAuthenticationMethod.Read.All, AuditLog.Read.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/userRegistrationDetails/{userRegistrationDetailsId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não dá suporte aos parâmetros de consulta OData ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userRegistrationDetails](../resources/userregistrationdetails.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_userregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/userRegistrationDetails/{userRegistrationDetailsId}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.userRegistrationDetails",
    "id": "6832a83d-2ef9-c5f5-9a2d-f2761d7ff317",
    "userDisplayName": "Abbe Smith",
    "userPrincipalName": "abbe@contoso.com",
    "isMfaRegistered": "true",
    "isMfaCapable": "true",
    "isSsprRegistered": "true",
    "isSsprEnabled": "false",
    "isSsprCapable": "false",
    "isPasswordlessCapable": "false",
    "methodsRegistered": [
      "mobilePhone",
      "email"
    ]
  }
}
```

