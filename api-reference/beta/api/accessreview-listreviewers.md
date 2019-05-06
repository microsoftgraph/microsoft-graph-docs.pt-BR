---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 756cb2d7bc93ea8fe490d0f857c609c3f82229f6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33585984"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="26a67-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="26a67-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a67-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="26a67-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26a67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="26a67-105">Permissions</span></span>
<span data-ttu-id="26a67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26a67-108">Permission type</span></span>                        | <span data-ttu-id="26a67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26a67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="26a67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26a67-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26a67-111">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="26a67-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="26a67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26a67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26a67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26a67-113">Not supported.</span></span> |
|<span data-ttu-id="26a67-114">Application</span><span class="sxs-lookup"><span data-stu-id="26a67-114">Application</span></span>                            | <span data-ttu-id="26a67-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a67-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="26a67-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="26a67-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="26a67-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26a67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="26a67-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26a67-118">Request headers</span></span>
| <span data-ttu-id="26a67-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26a67-119">Name</span></span>         | <span data-ttu-id="26a67-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="26a67-120">Type</span></span>        | <span data-ttu-id="26a67-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="26a67-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="26a67-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26a67-122">Authorization</span></span> | <span data-ttu-id="26a67-123">string</span><span class="sxs-lookup"><span data-stu-id="26a67-123">string</span></span> | <span data-ttu-id="26a67-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26a67-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26a67-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26a67-126">Request body</span></span>
<span data-ttu-id="26a67-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="26a67-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="26a67-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a67-128">Response</span></span>
<span data-ttu-id="26a67-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos UserIdentity no corpo da resposta. [](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="26a67-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a67-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26a67-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26a67-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26a67-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="26a67-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="26a67-132">Response</span></span>
><span data-ttu-id="26a67-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26a67-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="26a67-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="26a67-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="26a67-136">Basic</span><span class="sxs-lookup"><span data-stu-id="26a67-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26a67-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26a67-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="26a67-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="26a67-138">See also</span></span>

| <span data-ttu-id="26a67-139">Método</span><span class="sxs-lookup"><span data-stu-id="26a67-139">Method</span></span>           | <span data-ttu-id="26a67-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26a67-140">Return Type</span></span>    |<span data-ttu-id="26a67-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="26a67-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26a67-142">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="26a67-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="26a67-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="26a67-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="26a67-144">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="26a67-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="26a67-145">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="26a67-145">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="26a67-146">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26a67-146">None.</span></span>   |   <span data-ttu-id="26a67-147">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="26a67-147">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="26a67-148">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="26a67-148">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="26a67-149">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26a67-149">None.</span></span> |   <span data-ttu-id="26a67-150">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="26a67-150">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
