---
title: Atualizar permissionGrantPolicy
description: Atualizar um objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 0ccc47ff73b11fcbc0c465bb1dbe8979939511ac
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433506"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="582f1-103">Atualizar permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="582f1-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="582f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="582f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="582f1-105">Atualizar propriedades de um  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="582f1-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="582f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="582f1-106">Permissions</span></span>

<span data-ttu-id="582f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="582f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="582f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="582f1-109">Permission type</span></span>                        | <span data-ttu-id="582f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="582f1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="582f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="582f1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="582f1-112">Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="582f1-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="582f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="582f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="582f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="582f1-114">Not supported.</span></span> |
| <span data-ttu-id="582f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="582f1-115">Application</span></span>                            | <span data-ttu-id="582f1-116">Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="582f1-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="582f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="582f1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="582f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="582f1-118">Request headers</span></span>

| <span data-ttu-id="582f1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="582f1-119">Name</span></span>           | <span data-ttu-id="582f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="582f1-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="582f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="582f1-121">Authorization</span></span>  | <span data-ttu-id="582f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="582f1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="582f1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="582f1-124">Request body</span></span>

<span data-ttu-id="582f1-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="582f1-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="582f1-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="582f1-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="582f1-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="582f1-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="582f1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="582f1-128">Property</span></span>     | <span data-ttu-id="582f1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="582f1-129">Type</span></span> |<span data-ttu-id="582f1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="582f1-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="582f1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="582f1-131">displayName</span></span> | <span data-ttu-id="582f1-132">String</span><span class="sxs-lookup"><span data-stu-id="582f1-132">String</span></span> |<span data-ttu-id="582f1-133">O nome de exibição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="582f1-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="582f1-134">description</span><span class="sxs-lookup"><span data-stu-id="582f1-134">description</span></span> |<span data-ttu-id="582f1-135">String</span><span class="sxs-lookup"><span data-stu-id="582f1-135">String</span></span>| <span data-ttu-id="582f1-136">A descrição da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="582f1-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="582f1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="582f1-137">Response</span></span>

<span data-ttu-id="582f1-138">Se tiver êxito, este método retornará um `204 No Content` código de resposta e não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="582f1-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="582f1-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="582f1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="582f1-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="582f1-140">Request</span></span>

<span data-ttu-id="582f1-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="582f1-141">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="582f1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="582f1-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
