---
title: Atualizar crossTenantAccessPolicyConfigurationDefault
description: Atualize a configuração padrão de uma política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: be3e4d38320ffea436f9cced328a4f849d4f4d0a
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604532"
---
# <a name="update-crosstenantaccesspolicyconfigurationdefault"></a>Atualizar crossTenantAccessPolicyConfigurationDefault

Namespace: microsoft.graph

Atualize [a configuração padrão](../resources/crosstenantaccesspolicyconfigurationdefault.md) de uma política de acesso entre locatários.

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
PATCH /policies/crossTenantAccessPolicy/default
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
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração padrão para confiar em outras declarações de Acesso Condicional de organizações Azure AD externas. |
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários de outras organizações que acessam seus recursos por meio Azure AD colaboração B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD colaboração B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários de outras organizações que acessam seus recursos por meio Azure AD conexão direta B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD conexão direta B2B. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicyconfigurationdefault"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/default
Content-Type: application/json

{
  "b2bCollaborationOutbound":
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "0be493dc-cb56-4a53-936f-9cf64410b8b0",
          "targetType": "group"
        }
      ]
    },
    "applications":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
  }
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
