---
title: Obter authorizationPolicy
description: Recupere as propriedades e as relações do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ca66332d7461dfe4e2fc298fffab9ed0cff6e795
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047949"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="93486-103">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="93486-103">Get authorizationPolicy</span></span>

<span data-ttu-id="93486-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93486-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93486-105">Recupere as propriedades de um [objeto authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93486-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93486-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93486-106">Permissions</span></span>

<span data-ttu-id="93486-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93486-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93486-109">Permission type</span></span>                        | <span data-ttu-id="93486-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93486-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93486-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93486-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93486-112">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="93486-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="93486-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93486-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93486-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93486-114">Not supported.</span></span> |
| <span data-ttu-id="93486-115">Application</span><span class="sxs-lookup"><span data-stu-id="93486-115">Application</span></span>                            | <span data-ttu-id="93486-116">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="93486-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="93486-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93486-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="93486-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93486-118">Request headers</span></span>

| <span data-ttu-id="93486-119">Nome</span><span class="sxs-lookup"><span data-stu-id="93486-119">Name</span></span>      |<span data-ttu-id="93486-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="93486-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93486-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="93486-121">Authorization</span></span> | <span data-ttu-id="93486-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93486-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93486-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93486-124">Request body</span></span>

<span data-ttu-id="93486-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93486-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93486-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="93486-126">Response</span></span>

<span data-ttu-id="93486-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [authorizationPolicy](../resources/authorizationpolicy.md) único no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93486-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93486-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93486-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93486-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93486-129">Request</span></span>

<span data-ttu-id="93486-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93486-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="93486-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="93486-131">Response</span></span>

<span data-ttu-id="93486-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93486-132">The following is an example of the response.</span></span>

> <span data-ttu-id="93486-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="93486-133">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "enabledPreviewFeatures": [],
    "guestUserRoleId": "10dae51f-b6af-4016-8d66-8c2a99b929b3",
    "blockMsolPowerShell": ""
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": false,
        "allowedToReadOtherUsers": true
    }
    "allowedToSignUpEmailBasedSubscriptions": false,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
}
```


