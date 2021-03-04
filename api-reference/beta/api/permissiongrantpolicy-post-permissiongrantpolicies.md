---
title: Criar permissionGrantPolicy
description: Cria um objeto permissionGrantPolicy que descreve as condições sob as quais as permissões podem ser concedidas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0e682ed0849ac6985b651658a0e06ef2811ff149
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433863"
---
# <a name="create-permissiongrantpolicy"></a><span data-ttu-id="fba2a-103">Criar permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="fba2a-103">Create permissionGrantPolicy</span></span>

<span data-ttu-id="fba2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba2a-105">Cria uma [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fba2a-105">Creates a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span> <span data-ttu-id="fba2a-106">Uma política de concessão de permissão é usada para descrever as condições em que as permissões podem ser concedidas (por exemplo, durante o consentimento do aplicativo).</span><span class="sxs-lookup"><span data-stu-id="fba2a-106">A permission grant policy is used to describe the conditions under which permissions can be granted (for example, during application consent).</span></span>

<span data-ttu-id="fba2a-107">Depois de criar a política de concessão de permissão, você pode adicionar [conjuntos](permissiongrantpolicy-post-includes.md) de condições para adicionar regras correspondentes e adicionar conjuntos de condições [de](permissiongrantpolicy-post-excludes.md) exclusão para adicionar regras de exclusão.</span><span class="sxs-lookup"><span data-stu-id="fba2a-107">After creating the permission grant policy, you can [add include condition sets](permissiongrantpolicy-post-includes.md) to add matching rules, and [add exclude condition sets](permissiongrantpolicy-post-excludes.md) to add exclusion rules.</span></span>

## <a name="permissions"></a><span data-ttu-id="fba2a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fba2a-108">Permissions</span></span>

<span data-ttu-id="fba2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fba2a-111">Permission type</span></span>      | <span data-ttu-id="fba2a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fba2a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fba2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fba2a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fba2a-114">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba2a-114">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="fba2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fba2a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fba2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fba2a-116">Not supported.</span></span>    |
|<span data-ttu-id="fba2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fba2a-117">Application</span></span> | <span data-ttu-id="fba2a-118">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba2a-118">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fba2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fba2a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a><span data-ttu-id="fba2a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fba2a-120">Request headers</span></span>

| <span data-ttu-id="fba2a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fba2a-121">Name</span></span>       | <span data-ttu-id="fba2a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba2a-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="fba2a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fba2a-123">Authorization</span></span> | <span data-ttu-id="fba2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fba2a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fba2a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="fba2a-126">Content-type</span></span> | <span data-ttu-id="fba2a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fba2a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fba2a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fba2a-129">Request body</span></span>

<span data-ttu-id="fba2a-130">No corpo da solicitação, fornece uma representação JSON de [um objeto permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fba2a-130">In the request body, supply a JSON representation of an [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fba2a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba2a-131">Response</span></span>

<span data-ttu-id="fba2a-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fba2a-132">If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fba2a-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fba2a-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fba2a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fba2a-134">Request</span></span>

<span data-ttu-id="fba2a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fba2a-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fba2a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fba2a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
# <a name="c"></a>[<span data-ttu-id="fba2a-137">C#</span><span class="sxs-lookup"><span data-stu-id="fba2a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fba2a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fba2a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fba2a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fba2a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fba2a-140">Java</span><span class="sxs-lookup"><span data-stu-id="fba2a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fba2a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba2a-141">Response</span></span>

<span data-ttu-id="fba2a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fba2a-142">The following is an example of the response.</span></span>

> <span data-ttu-id="fba2a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fba2a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
