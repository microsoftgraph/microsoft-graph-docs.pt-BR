---
title: Adicionar revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8cf965a201010599a0cd76c2ad74dd99438d57d4
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049502"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="c9614-105">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="c9614-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9614-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="c9614-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="c9614-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="c9614-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="c9614-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="c9614-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c9614-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9614-109">Permissions</span></span>
<span data-ttu-id="c9614-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9614-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9614-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9614-112">Permission type</span></span>                        | <span data-ttu-id="c9614-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9614-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9614-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9614-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9614-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9614-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c9614-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9614-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9614-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9614-117">Not supported.</span></span> |
|<span data-ttu-id="c9614-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9614-118">Application</span></span>                            | <span data-ttu-id="c9614-119">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="c9614-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9614-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9614-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="c9614-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9614-121">Request headers</span></span>
| <span data-ttu-id="c9614-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c9614-122">Name</span></span>         | <span data-ttu-id="c9614-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9614-123">Type</span></span>        | <span data-ttu-id="c9614-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9614-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c9614-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9614-125">Authorization</span></span> | <span data-ttu-id="c9614-126">string</span><span class="sxs-lookup"><span data-stu-id="c9614-126">string</span></span> | <span data-ttu-id="c9614-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9614-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9614-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9614-129">Request body</span></span>
<span data-ttu-id="c9614-130">No corpo da solicitação, forneça uma representação JSON da ID de um usuário que será um revisor.</span><span class="sxs-lookup"><span data-stu-id="c9614-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="c9614-131">A tabela a seguir mostra as propriedades que podem ser fornecidas ao atualizar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c9614-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="c9614-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9614-132">Property</span></span>     | <span data-ttu-id="c9614-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9614-133">Type</span></span>        | <span data-ttu-id="c9614-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9614-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="c9614-135">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9614-135">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="c9614-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9614-136">Response</span></span>
<span data-ttu-id="c9614-137">Se tiver êxito, este método retornará `201, Created` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9614-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="c9614-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9614-138">Example</span></span>

<span data-ttu-id="c9614-139">Este é um exemplo de atualização de uma revisão de acesso de um único tempo (sem refazê-las) com um revisor adicional.</span><span class="sxs-lookup"><span data-stu-id="c9614-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="c9614-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9614-140">Request</span></span>
<span data-ttu-id="c9614-141">No corpo da solicitação, forneça uma representação JSON da ID do objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9614-141">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9614-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9614-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9614-143">C#</span><span class="sxs-lookup"><span data-stu-id="c9614-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9614-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9614-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9614-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c9614-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9614-146">Java</span><span class="sxs-lookup"><span data-stu-id="c9614-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c9614-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9614-147">Response</span></span>
><span data-ttu-id="c9614-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9614-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
