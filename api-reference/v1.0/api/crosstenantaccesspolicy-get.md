---
title: Obter crossTenantAccessPolicy
description: Leia as propriedades e as relações de um objeto crossTenantAccessPolicy.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5263c7486869c68f6e91d22bc390a625da41a514
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604531"
---
# <a name="get-crosstenantaccesspolicy"></a>Obter crossTenantAccessPolicy

Namespace: microsoft.graph

Leia as propriedades e as relações de um [objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.CrossTenantAccess|
|Delegado (conta pessoal da Microsoft)|Não aplicável|
|Aplicativo|Policy.Read.All, Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/crossTenantAccessPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_crosstenantaccesspolicy"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.crossTenantAccessPolicy",
    "displayName": "CrossTenantAccessPolicy",
    "definition": "Cross tenant access policy..."
  }
}
```
