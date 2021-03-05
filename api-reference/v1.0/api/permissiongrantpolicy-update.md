---
title: Atualizar permissionGrantPolicy
description: Atualize um objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 223fffce4f607004897360c2653dc8327c166255
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448071"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="b04b7-103">Atualizar permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="b04b7-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="b04b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b04b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b04b7-105">Atualizar propriedades de  [uma permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b04b7-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b04b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b04b7-106">Permissions</span></span>

<span data-ttu-id="b04b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b04b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b04b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b04b7-109">Permission type</span></span>                        | <span data-ttu-id="b04b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b04b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b04b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b04b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b04b7-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b04b7-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="b04b7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b04b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b04b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b04b7-114">Not supported.</span></span> |
| <span data-ttu-id="b04b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b04b7-115">Application</span></span>                            | <span data-ttu-id="b04b7-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b04b7-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="b04b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b04b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b04b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b04b7-118">Request headers</span></span>

| <span data-ttu-id="b04b7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b04b7-119">Name</span></span>           | <span data-ttu-id="b04b7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b04b7-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b04b7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b04b7-121">Authorization</span></span>  | <span data-ttu-id="b04b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b04b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b04b7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b04b7-124">Request body</span></span>

<span data-ttu-id="b04b7-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b04b7-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b04b7-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b04b7-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b04b7-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b04b7-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b04b7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b04b7-128">Property</span></span>     | <span data-ttu-id="b04b7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b04b7-129">Type</span></span> |<span data-ttu-id="b04b7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b04b7-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b04b7-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b04b7-131">displayName</span></span> | <span data-ttu-id="b04b7-132">String</span><span class="sxs-lookup"><span data-stu-id="b04b7-132">String</span></span> |<span data-ttu-id="b04b7-133">O nome de exibição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="b04b7-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="b04b7-134">descrição</span><span class="sxs-lookup"><span data-stu-id="b04b7-134">description</span></span> |<span data-ttu-id="b04b7-135">String</span><span class="sxs-lookup"><span data-stu-id="b04b7-135">String</span></span>| <span data-ttu-id="b04b7-136">A descrição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="b04b7-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="b04b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b04b7-137">Response</span></span>

<span data-ttu-id="b04b7-138">Se tiver êxito, este método retornará um código `204 No Content` de resposta e não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b04b7-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b04b7-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b04b7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b04b7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b04b7-140">Request</span></span>

<span data-ttu-id="b04b7-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b04b7-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b04b7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b04b7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[<span data-ttu-id="b04b7-143">C#</span><span class="sxs-lookup"><span data-stu-id="b04b7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b04b7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b04b7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b04b7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b04b7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b04b7-146">Java</span><span class="sxs-lookup"><span data-stu-id="b04b7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b04b7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b04b7-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
