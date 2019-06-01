---
title: Adicionar revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0839fe486679b4388b0bbdd714bb775b8090b27
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655569"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="1142a-105">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="1142a-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1142a-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="1142a-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="1142a-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="1142a-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="1142a-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="1142a-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="1142a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1142a-109">Permissions</span></span>
<span data-ttu-id="1142a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1142a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1142a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1142a-112">Permission type</span></span>                        | <span data-ttu-id="1142a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1142a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1142a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1142a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1142a-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1142a-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1142a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1142a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1142a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1142a-117">Not supported.</span></span> |
|<span data-ttu-id="1142a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1142a-118">Application</span></span>                            | <span data-ttu-id="1142a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1142a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1142a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1142a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="1142a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1142a-121">Request headers</span></span>
| <span data-ttu-id="1142a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1142a-122">Name</span></span>         | <span data-ttu-id="1142a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1142a-123">Type</span></span>        | <span data-ttu-id="1142a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1142a-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1142a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1142a-125">Authorization</span></span> | <span data-ttu-id="1142a-126">string</span><span class="sxs-lookup"><span data-stu-id="1142a-126">string</span></span> | <span data-ttu-id="1142a-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1142a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1142a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1142a-129">Request body</span></span>
<span data-ttu-id="1142a-130">No corpo da solicitação, forneça uma representação JSON da ID de um usuário que será um revisor.</span><span class="sxs-lookup"><span data-stu-id="1142a-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="1142a-131">A tabela a seguir mostra as propriedades que podem ser fornecidas ao atualizar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="1142a-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="1142a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1142a-132">Property</span></span>     | <span data-ttu-id="1142a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1142a-133">Type</span></span>        | <span data-ttu-id="1142a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1142a-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="1142a-135">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1142a-135">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="1142a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1142a-136">Response</span></span>
<span data-ttu-id="1142a-137">Se tiver êxito, este método retornará `201, Created` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="1142a-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="1142a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1142a-138">Example</span></span>

<span data-ttu-id="1142a-139">Este é um exemplo de atualização de uma revisão de acesso de um único tempo (sem refazê-las) com um revisor adicional.</span><span class="sxs-lookup"><span data-stu-id="1142a-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="1142a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1142a-140">Request</span></span>
<span data-ttu-id="1142a-141">No corpo da solicitação, forneça uma representação JSON da ID do objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="1142a-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1142a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1142a-142">Response</span></span>
><span data-ttu-id="1142a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1142a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1142a-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1142a-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1142a-146">C#</span><span class="sxs-lookup"><span data-stu-id="1142a-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/add_accessReview_reviewer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1142a-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="1142a-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/add_accessReview_reviewer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
