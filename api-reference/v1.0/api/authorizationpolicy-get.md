---
title: Obter authorizationPolicy
description: Recupere as propriedades e as relações do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7ffb4e245e9a24f5ed33576dbd414891ee5d28ac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434913"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="0150b-103">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0150b-103">Get authorizationPolicy</span></span>

<span data-ttu-id="0150b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0150b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0150b-105">Recupere as propriedades de um [objeto authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0150b-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0150b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0150b-106">Permissions</span></span>

<span data-ttu-id="0150b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0150b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0150b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0150b-109">Permission type</span></span>                        | <span data-ttu-id="0150b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0150b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0150b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0150b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0150b-112">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="0150b-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="0150b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0150b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0150b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0150b-114">Not supported.</span></span> |
| <span data-ttu-id="0150b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0150b-115">Application</span></span>                            | <span data-ttu-id="0150b-116">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="0150b-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="0150b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0150b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="0150b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0150b-118">Request headers</span></span>

| <span data-ttu-id="0150b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0150b-119">Name</span></span>      |<span data-ttu-id="0150b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0150b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0150b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0150b-121">Authorization</span></span> | <span data-ttu-id="0150b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0150b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0150b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0150b-124">Request body</span></span>

<span data-ttu-id="0150b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0150b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0150b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0150b-126">Response</span></span>

<span data-ttu-id="0150b-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [authorizationPolicy](../resources/authorizationpolicy.md) único no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0150b-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0150b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0150b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0150b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0150b-129">Request</span></span>

<span data-ttu-id="0150b-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0150b-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="0150b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0150b-131">Response</span></span>

<span data-ttu-id="0150b-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0150b-132">The following is an example of the response.</span></span>

> <span data-ttu-id="0150b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0150b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
