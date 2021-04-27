---
title: Listar revisores do accessReview
description: No recurso de revisões de acesso do Azure AD, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 457064b9dfa866d0d5bfe8285b495ecd3f8a4fe4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048460"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="84f57-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="84f57-103">List accessReview reviewers</span></span>

<span data-ttu-id="84f57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84f57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84f57-105">No recurso de revisões de acesso do Azure AD, recupere os [revisores](../resources/accessreviews-root.md) de um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="84f57-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84f57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84f57-106">Permissions</span></span>
<span data-ttu-id="84f57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84f57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84f57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84f57-109">Permission type</span></span>                        | <span data-ttu-id="84f57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84f57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="84f57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84f57-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="84f57-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84f57-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="84f57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84f57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84f57-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84f57-114">Not supported.</span></span> |
|<span data-ttu-id="84f57-115">Application</span><span class="sxs-lookup"><span data-stu-id="84f57-115">Application</span></span>                            | <span data-ttu-id="84f57-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="84f57-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="84f57-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="84f57-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="84f57-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84f57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="84f57-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84f57-119">Request headers</span></span>
| <span data-ttu-id="84f57-120">Nome</span><span class="sxs-lookup"><span data-stu-id="84f57-120">Name</span></span>         | <span data-ttu-id="84f57-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="84f57-121">Type</span></span>        | <span data-ttu-id="84f57-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="84f57-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="84f57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84f57-123">Authorization</span></span> | <span data-ttu-id="84f57-124">string</span><span class="sxs-lookup"><span data-stu-id="84f57-124">string</span></span> | <span data-ttu-id="84f57-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84f57-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84f57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84f57-127">Request body</span></span>
<span data-ttu-id="84f57-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="84f57-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="84f57-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="84f57-129">Response</span></span>
<span data-ttu-id="84f57-130">Se tiver êxito, este método retornará um código de resposta e uma `200, OK` matriz de [objetos userIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84f57-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84f57-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84f57-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84f57-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84f57-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="84f57-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84f57-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="84f57-134">C#</span><span class="sxs-lookup"><span data-stu-id="84f57-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84f57-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84f57-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84f57-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84f57-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84f57-137">Java</span><span class="sxs-lookup"><span data-stu-id="84f57-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="84f57-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="84f57-138">Response</span></span>
><span data-ttu-id="84f57-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="84f57-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="84f57-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="84f57-140">See also</span></span>

| <span data-ttu-id="84f57-141">Método</span><span class="sxs-lookup"><span data-stu-id="84f57-141">Method</span></span>           | <span data-ttu-id="84f57-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="84f57-142">Return Type</span></span>    |<span data-ttu-id="84f57-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="84f57-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84f57-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="84f57-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="84f57-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="84f57-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="84f57-146">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="84f57-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="84f57-147">Adicionar o revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="84f57-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="84f57-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84f57-148">None.</span></span>   |   <span data-ttu-id="84f57-149">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="84f57-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="84f57-150">Remover o revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="84f57-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="84f57-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84f57-151">None.</span></span> |   <span data-ttu-id="84f57-152">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="84f57-152">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


