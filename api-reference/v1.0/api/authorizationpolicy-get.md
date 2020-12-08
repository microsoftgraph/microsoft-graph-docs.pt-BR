---
title: Obter authorizationPolicy
description: Recupere as propriedades e os relacionamentos do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 620c01155c8ae1af11416c88ccdf1793bfb054f7
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581180"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="094e7-103">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="094e7-103">Get authorizationPolicy</span></span>

<span data-ttu-id="094e7-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="094e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="094e7-105">Recupere as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="094e7-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="094e7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="094e7-106">Permissions</span></span>

<span data-ttu-id="094e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="094e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="094e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="094e7-109">Permission type</span></span>                        | <span data-ttu-id="094e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="094e7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="094e7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="094e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="094e7-112">Policy. Read. All, Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="094e7-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="094e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="094e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="094e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="094e7-114">Not supported.</span></span> |
| <span data-ttu-id="094e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="094e7-115">Application</span></span>                            | <span data-ttu-id="094e7-116">Policy. Read. All, Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="094e7-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="094e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="094e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="094e7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="094e7-118">Request headers</span></span>

| <span data-ttu-id="094e7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="094e7-119">Name</span></span>      |<span data-ttu-id="094e7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="094e7-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="094e7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="094e7-121">Authorization</span></span> | <span data-ttu-id="094e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="094e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="094e7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="094e7-124">Request body</span></span>

<span data-ttu-id="094e7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="094e7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="094e7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="094e7-126">Response</span></span>

<span data-ttu-id="094e7-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e o único objeto [authorizationPolicy](../resources/authorizationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="094e7-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="094e7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="094e7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="094e7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="094e7-129">Request</span></span>

<span data-ttu-id="094e7-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="094e7-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="094e7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="094e7-131">Response</span></span>

<span data-ttu-id="094e7-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="094e7-132">The following is an example of the response.</span></span>

> <span data-ttu-id="094e7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="094e7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
