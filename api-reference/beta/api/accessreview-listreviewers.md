---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d946584221d2bab4cf1ee80a840a34ec864e4789
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258860"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="a0ece-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="a0ece-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ece-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a0ece-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0ece-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0ece-105">Permissions</span></span>
<span data-ttu-id="a0ece-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0ece-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0ece-108">Permission type</span></span>                        | <span data-ttu-id="a0ece-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0ece-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0ece-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0ece-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0ece-111">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a0ece-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a0ece-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0ece-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ece-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0ece-113">Not supported.</span></span> |
|<span data-ttu-id="a0ece-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ece-114">Application</span></span>                            | <span data-ttu-id="a0ece-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0ece-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="a0ece-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a0ece-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0ece-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ece-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="a0ece-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ece-118">Request headers</span></span>
| <span data-ttu-id="a0ece-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a0ece-119">Name</span></span>         | <span data-ttu-id="a0ece-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0ece-120">Type</span></span>        | <span data-ttu-id="a0ece-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ece-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a0ece-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0ece-122">Authorization</span></span> | <span data-ttu-id="a0ece-123">string</span><span class="sxs-lookup"><span data-stu-id="a0ece-123">string</span></span> | <span data-ttu-id="a0ece-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ece-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0ece-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ece-126">Request body</span></span>
<span data-ttu-id="a0ece-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="a0ece-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a0ece-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ece-128">Response</span></span>
<span data-ttu-id="a0ece-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos UserIdentity no corpo da resposta. [](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="a0ece-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0ece-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0ece-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0ece-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ece-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="a0ece-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ece-132">Response</span></span>
><span data-ttu-id="a0ece-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0ece-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0ece-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a0ece-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0ece-136">C#</span><span class="sxs-lookup"><span data-stu-id="a0ece-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0ece-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0ece-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a0ece-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a0ece-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="a0ece-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0ece-139">See also</span></span>

| <span data-ttu-id="a0ece-140">Método</span><span class="sxs-lookup"><span data-stu-id="a0ece-140">Method</span></span>           | <span data-ttu-id="a0ece-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0ece-141">Return Type</span></span>    |<span data-ttu-id="a0ece-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ece-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0ece-143">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="a0ece-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a0ece-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="a0ece-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a0ece-145">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a0ece-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a0ece-146">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="a0ece-146">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="a0ece-147">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0ece-147">None.</span></span>   |   <span data-ttu-id="a0ece-148">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a0ece-148">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a0ece-149">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="a0ece-149">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="a0ece-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0ece-150">None.</span></span> |   <span data-ttu-id="a0ece-151">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a0ece-151">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
