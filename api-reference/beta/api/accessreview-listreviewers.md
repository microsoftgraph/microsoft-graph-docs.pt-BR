---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e4f6900011d75077d30fd16cc16345db0e4c7d6
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172698"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="d10a7-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="d10a7-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d10a7-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="d10a7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d10a7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d10a7-105">Permissions</span></span>
<span data-ttu-id="d10a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d10a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d10a7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d10a7-108">Permission type</span></span>                        | <span data-ttu-id="d10a7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d10a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d10a7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d10a7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d10a7-111">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d10a7-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d10a7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d10a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d10a7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d10a7-113">Not supported.</span></span> |
|<span data-ttu-id="d10a7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d10a7-114">Application</span></span>                            | <span data-ttu-id="d10a7-115">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="d10a7-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="d10a7-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="d10a7-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d10a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d10a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="d10a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a7-118">Request headers</span></span>
| <span data-ttu-id="d10a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d10a7-119">Name</span></span>         | <span data-ttu-id="d10a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d10a7-120">Type</span></span>        | <span data-ttu-id="d10a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d10a7-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d10a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d10a7-122">Authorization</span></span> | <span data-ttu-id="d10a7-123">string</span><span class="sxs-lookup"><span data-stu-id="d10a7-123">string</span></span> | <span data-ttu-id="d10a7-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d10a7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d10a7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a7-126">Request body</span></span>
<span data-ttu-id="d10a7-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d10a7-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d10a7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10a7-128">Response</span></span>
<span data-ttu-id="d10a7-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos UserIdentity no corpo da resposta. [](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="d10a7-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d10a7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d10a7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d10a7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a7-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d10a7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d10a7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d10a7-133">C#</span><span class="sxs-lookup"><span data-stu-id="d10a7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d10a7-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d10a7-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d10a7-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d10a7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d10a7-136">Java</span><span class="sxs-lookup"><span data-stu-id="d10a7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d10a7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10a7-137">Response</span></span>
><span data-ttu-id="d10a7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d10a7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d10a7-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="d10a7-140">See also</span></span>

| <span data-ttu-id="d10a7-141">Método</span><span class="sxs-lookup"><span data-stu-id="d10a7-141">Method</span></span>           | <span data-ttu-id="d10a7-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d10a7-142">Return Type</span></span>    |<span data-ttu-id="d10a7-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d10a7-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d10a7-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="d10a7-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d10a7-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="d10a7-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d10a7-146">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="d10a7-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d10a7-147">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="d10a7-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="d10a7-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d10a7-148">None.</span></span>   |   <span data-ttu-id="d10a7-149">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d10a7-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="d10a7-150">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="d10a7-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="d10a7-151">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d10a7-151">None.</span></span> |   <span data-ttu-id="d10a7-152">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d10a7-152">Remove a reviewer from an accessReview.</span></span> |


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
