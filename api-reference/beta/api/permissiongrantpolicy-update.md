---
title: Atualizar permissionGrantPolicy
description: Atualizar um objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 1bc18442c7c6e1713ca1ed863a631519aeadef00
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459603"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="5a896-103">Atualizar permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="5a896-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="5a896-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a896-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a896-105">Atualizar propriedades de um  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5a896-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a896-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a896-106">Permissions</span></span>

<span data-ttu-id="5a896-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a896-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a896-109">Permission type</span></span>                        | <span data-ttu-id="5a896-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a896-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a896-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a896-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a896-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a896-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="5a896-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a896-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a896-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a896-114">Not supported.</span></span> |
| <span data-ttu-id="5a896-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a896-115">Application</span></span>                            | <span data-ttu-id="5a896-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a896-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a896-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a896-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a896-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a896-118">Request headers</span></span>

| <span data-ttu-id="5a896-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5a896-119">Name</span></span>           | <span data-ttu-id="5a896-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a896-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="5a896-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a896-121">Authorization</span></span>  | <span data-ttu-id="5a896-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a896-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a896-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a896-124">Request body</span></span>

<span data-ttu-id="5a896-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5a896-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5a896-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5a896-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5a896-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5a896-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a896-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a896-128">Property</span></span>     | <span data-ttu-id="5a896-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a896-129">Type</span></span> |<span data-ttu-id="5a896-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a896-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a896-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5a896-131">displayName</span></span> | <span data-ttu-id="5a896-132">String</span><span class="sxs-lookup"><span data-stu-id="5a896-132">String</span></span> |<span data-ttu-id="5a896-133">O nome de exibição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="5a896-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="5a896-134">description</span><span class="sxs-lookup"><span data-stu-id="5a896-134">description</span></span> |<span data-ttu-id="5a896-135">String</span><span class="sxs-lookup"><span data-stu-id="5a896-135">String</span></span>| <span data-ttu-id="5a896-136">A descrição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="5a896-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="5a896-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a896-137">Response</span></span>

<span data-ttu-id="5a896-138">Se tiver êxito, este método retornará um `204 No Content` código de resposta e não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a896-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a896-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a896-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a896-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a896-140">Request</span></span>

<span data-ttu-id="5a896-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a896-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a896-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a896-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[<span data-ttu-id="5a896-143">C#</span><span class="sxs-lookup"><span data-stu-id="5a896-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a896-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a896-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a896-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a896-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5a896-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a896-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
