---
title: Atualizar crossTenantAccessPolicy
description: Atualize as propriedades de uma política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 33559dec1bdd8d29f3a8559aabc4b47aa8950b3f
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604534"
---
# <a name="update-crosstenantaccesspolicy"></a>Atualizar crossTenantAccessPolicy

Namespace: microsoft.graph

Atualize as propriedades de uma política [de acesso entre locatários](../resources/crosstenantaccesspolicy.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.ReadWrite.CrossTenantAccess|
|Delegado (conta pessoal da Microsoft)|Não aplicável|
|Aplicativo|Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/crossTenantAccessPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da política de acesso entre locatários.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

O [tamanho do objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) está atualmente limitado a 25 KB. Esse método retornará um código `400 Bad Request` de erro se o tamanho da política exceder 25 KB.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy
Content-Type: application/json

{
  "displayName": "CrossTenantAccessPolicy",
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
