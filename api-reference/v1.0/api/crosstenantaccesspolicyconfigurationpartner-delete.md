---
title: Excluir crossTenantAccessPolicyConfigurationPartner
description: Exclua uma configuração específica do parceiro em uma política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b77745667559e3388d054ffd0ec6cb7e1ec80945
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604545"
---
# <a name="delete-crosstenantaccesspolicyconfigurationpartner"></a>Excluir crossTenantAccessPolicyConfigurationPartner

Namespace: microsoft.graph

Exclua [uma configuração específica do parceiro](../resources/crosstenantaccesspolicyconfigurationpartner.md) em uma política de acesso entre locatários.

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
DELETE /policies/crossTenantAccessPolicy/partners/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551
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
