---
title: Adicionar revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 423fd326ffa2d577d24265931deb5ad84027ecc4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951720"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="7ae13-105">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="7ae13-105">Add accessReview reviewer</span></span>

<span data-ttu-id="7ae13-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ae13-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ae13-107">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="7ae13-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="7ae13-108">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="7ae13-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="7ae13-109">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="7ae13-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7ae13-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ae13-110">Permissions</span></span>
<span data-ttu-id="7ae13-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ae13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ae13-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ae13-113">Permission type</span></span>                        | <span data-ttu-id="7ae13-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ae13-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ae13-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ae13-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ae13-116">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7ae13-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7ae13-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ae13-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ae13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ae13-118">Not supported.</span></span> |
|<span data-ttu-id="7ae13-119">Application</span><span class="sxs-lookup"><span data-stu-id="7ae13-119">Application</span></span>                            | <span data-ttu-id="7ae13-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="7ae13-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ae13-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae13-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="7ae13-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae13-122">Request headers</span></span>
| <span data-ttu-id="7ae13-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7ae13-123">Name</span></span>         | <span data-ttu-id="7ae13-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ae13-124">Type</span></span>        | <span data-ttu-id="7ae13-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae13-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7ae13-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ae13-126">Authorization</span></span> | <span data-ttu-id="7ae13-127">string</span><span class="sxs-lookup"><span data-stu-id="7ae13-127">string</span></span> | <span data-ttu-id="7ae13-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ae13-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ae13-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae13-130">Request body</span></span>
<span data-ttu-id="7ae13-131">No corpo da solicitação, forneça uma representação JSON da ID de um usuário que será um revisor.</span><span class="sxs-lookup"><span data-stu-id="7ae13-131">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="7ae13-132">A tabela a seguir mostra as propriedades que podem ser fornecidas ao atualizar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="7ae13-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="7ae13-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ae13-133">Property</span></span>     | <span data-ttu-id="7ae13-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ae13-134">Type</span></span>        | <span data-ttu-id="7ae13-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae13-135">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="7ae13-136">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="7ae13-136">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="7ae13-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae13-137">Response</span></span>
<span data-ttu-id="7ae13-138">Se tiver êxito, este método retornará um `201, Created` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae13-138">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="7ae13-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ae13-139">Example</span></span>

<span data-ttu-id="7ae13-140">Este é um exemplo de atualização de uma revisão de acesso de um único tempo (sem refazê-las) com um revisor adicional.</span><span class="sxs-lookup"><span data-stu-id="7ae13-140">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="7ae13-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae13-141">Request</span></span>
<span data-ttu-id="7ae13-142">No corpo da solicitação, forneça uma representação JSON da ID do objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="7ae13-142">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="7ae13-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae13-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="c"></a>[<span data-ttu-id="7ae13-144">C#</span><span class="sxs-lookup"><span data-stu-id="7ae13-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ae13-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ae13-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ae13-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ae13-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ae13-147">Java</span><span class="sxs-lookup"><span data-stu-id="7ae13-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ae13-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae13-148">Response</span></span>
><span data-ttu-id="7ae13-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ae13-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


