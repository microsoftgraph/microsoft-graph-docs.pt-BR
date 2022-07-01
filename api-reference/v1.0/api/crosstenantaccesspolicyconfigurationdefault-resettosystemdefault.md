---
title: 'crossTenantAccessPolicyConfigurationDefault: resetToSystemDefault'
description: Redefina as alterações feitas na configuração padrão em uma política de acesso entre locatários de volta para o padrão do sistema.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d648111a55750a645fc9da1fcd9de4e134a94e3e
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604528"
---
# <a name="crosstenantaccesspolicyconfigurationdefault-resettosystemdefault"></a>crossTenantAccessPolicyConfigurationDefault: resetToSystemDefault

Namespace: microsoft.graph

Redefina as alterações feitas na configuração padrão em uma política de acesso entre locatários de volta para o padrão do sistema.

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
POST /policies/crossTenantAccessPolicy/default/resetToSystemDefault
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`. Para confirmar que a configuração padrão foi restaurada para os padrões do sistema, execute [Get crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md) e confirme se **isSystemDefault** está definido como `true`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "crosstenantaccesspolicyconfigurationdefault_resettosystemdefault"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/default/resetToSystemDefault
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
