---
title: Obter authorizationPolicy
description: Recupere as propriedades e as relações do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a5a108cc74ba41cfa5ac21a362c053bfc966bf14
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052527"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="d1dd9-103">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="d1dd9-103">Get authorizationPolicy</span></span>

<span data-ttu-id="d1dd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1dd9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1dd9-105">Recupere as propriedades de um [objeto authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d1dd9-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1dd9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1dd9-106">Permissions</span></span>

<span data-ttu-id="d1dd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1dd9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1dd9-109">Permission type</span></span>                        | <span data-ttu-id="d1dd9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1dd9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1dd9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1dd9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1dd9-112">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="d1dd9-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="d1dd9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1dd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1dd9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-114">Not supported.</span></span> |
| <span data-ttu-id="d1dd9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1dd9-115">Application</span></span>                            | <span data-ttu-id="d1dd9-116">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="d1dd9-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1dd9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1dd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="d1dd9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd9-118">Request headers</span></span>

| <span data-ttu-id="d1dd9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d1dd9-119">Name</span></span>      |<span data-ttu-id="d1dd9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1dd9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1dd9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1dd9-121">Authorization</span></span> | <span data-ttu-id="d1dd9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1dd9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd9-124">Request body</span></span>

<span data-ttu-id="d1dd9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1dd9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dd9-126">Response</span></span>

<span data-ttu-id="d1dd9-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [authorizationPolicy](../resources/authorizationpolicy.md) único no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1dd9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1dd9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1dd9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd9-129">Request</span></span>

<span data-ttu-id="d1dd9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="d1dd9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dd9-131">Response</span></span>

<span data-ttu-id="d1dd9-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-132">The following is an example of the response.</span></span>

> <span data-ttu-id="d1dd9-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d1dd9-133">**Note:** The response object shown here might be shortened for readability.</span></span>

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
