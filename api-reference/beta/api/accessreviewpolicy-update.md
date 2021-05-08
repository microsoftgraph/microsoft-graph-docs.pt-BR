---
title: Atualizar accessReviewPolicy
description: Atualize as propriedades de um objeto accessReviewPolicy.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cd774e18586218182379a0523df304a20a8e7e7c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240615"
---
# <a name="update-accessreviewpolicy"></a><span data-ttu-id="37c46-103">Atualizar accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="37c46-103">Update accessReviewPolicy</span></span>
<span data-ttu-id="37c46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c46-105">Atualize as propriedades de [um objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37c46-105">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37c46-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37c46-106">Permissions</span></span>
<span data-ttu-id="37c46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37c46-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37c46-109">Permission type</span></span>|<span data-ttu-id="37c46-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37c46-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37c46-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37c46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37c46-112">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="37c46-112">Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="37c46-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37c46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c46-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c46-114">Not supported.</span></span>|
|<span data-ttu-id="37c46-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37c46-115">Application</span></span>|<span data-ttu-id="37c46-116">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="37c46-116">Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="37c46-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37c46-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/accessReviewPolicy
PATCH /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="37c46-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37c46-118">Request headers</span></span>
|<span data-ttu-id="37c46-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37c46-119">Name</span></span>|<span data-ttu-id="37c46-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c46-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37c46-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37c46-121">Authorization</span></span>|<span data-ttu-id="37c46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c46-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="37c46-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37c46-124">Content-Type</span></span>|<span data-ttu-id="37c46-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c46-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37c46-127">Request body</span></span>
<span data-ttu-id="37c46-128">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37c46-128">In the request body, supply a JSON representation of the [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

<span data-ttu-id="37c46-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o accessReviewPolicy](../resources/accessreviewpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="37c46-129">The following table shows the properties that are required when you update the [accessReviewPolicy](../resources/accessreviewpolicy.md).</span></span>

|<span data-ttu-id="37c46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37c46-130">Property</span></span>|<span data-ttu-id="37c46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37c46-131">Type</span></span>|<span data-ttu-id="37c46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c46-133">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="37c46-133">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="37c46-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="37c46-134">Boolean</span></span>|<span data-ttu-id="37c46-135">Se `true` , os proprietários do grupo podem criar e gerenciar avaliações de acesso nos grupos que eles próprios têm.</span><span class="sxs-lookup"><span data-stu-id="37c46-135">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|



## <a name="response"></a><span data-ttu-id="37c46-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c46-136">Response</span></span>

<span data-ttu-id="37c46-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37c46-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="37c46-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37c46-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37c46-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37c46-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="37c46-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c46-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/accessReviewPolicy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="37c46-141">C#</span><span class="sxs-lookup"><span data-stu-id="37c46-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c46-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c46-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c46-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c46-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c46-144">Java</span><span class="sxs-lookup"><span data-stu-id="37c46-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37c46-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c46-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="request"></a><span data-ttu-id="37c46-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37c46-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="37c46-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c46-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy_2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="37c46-148">C#</span><span class="sxs-lookup"><span data-stu-id="37c46-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c46-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c46-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c46-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c46-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c46-151">Java</span><span class="sxs-lookup"><span data-stu-id="37c46-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37c46-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c46-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
