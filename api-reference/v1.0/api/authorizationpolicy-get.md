---
title: Obter authorizationPolicy
description: Recupere as propriedades e as relações do objeto authorizationPolicy.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ff9c46876ac2c3f7605ed93f905d392142cb1a51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038458"
---
# <a name="get-authorizationpolicy"></a>Obter authorizationPolicy

Namespace: microsoft.graph

Recupere as propriedades de um [objeto authorizationPolicy.](../resources/authorizationpolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Policy.Read.All, Policy.ReadWrite.Authorization |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy.Read.All, Policy.ReadWrite.Authorization |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [authorizationPolicy](../resources/authorizationpolicy.md) único no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "allowInvitesFrom": "everyone",
    "allowedToSignUpEmailBasedSubscriptions": true,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "blockMsolPowerShell": null,
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": true,
        "allowedToReadOtherUsers": true,
        "permissionGrantPoliciesAssigned": [
            "just-user-read"
        ]
    }
}
```
