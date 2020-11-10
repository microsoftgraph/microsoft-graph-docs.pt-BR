---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b1acf9a196551c0f2f170ca9df507d902558744
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951496"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="85ef3-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="85ef3-103">List accessReview reviewers</span></span>

<span data-ttu-id="85ef3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85ef3-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="85ef3-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="85ef3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85ef3-106">Permissions</span></span>
<span data-ttu-id="85ef3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85ef3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85ef3-109">Permission type</span></span>                        | <span data-ttu-id="85ef3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85ef3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85ef3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85ef3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85ef3-112">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85ef3-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="85ef3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85ef3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85ef3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85ef3-114">Not supported.</span></span> |
|<span data-ttu-id="85ef3-115">Application</span><span class="sxs-lookup"><span data-stu-id="85ef3-115">Application</span></span>                            | <span data-ttu-id="85ef3-116">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="85ef3-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="85ef3-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="85ef3-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="85ef3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85ef3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="85ef3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85ef3-119">Request headers</span></span>
| <span data-ttu-id="85ef3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="85ef3-120">Name</span></span>         | <span data-ttu-id="85ef3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="85ef3-121">Type</span></span>        | <span data-ttu-id="85ef3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="85ef3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85ef3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85ef3-123">Authorization</span></span> | <span data-ttu-id="85ef3-124">string</span><span class="sxs-lookup"><span data-stu-id="85ef3-124">string</span></span> | <span data-ttu-id="85ef3-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85ef3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85ef3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85ef3-127">Request body</span></span>
<span data-ttu-id="85ef3-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="85ef3-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="85ef3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="85ef3-129">Response</span></span>
<span data-ttu-id="85ef3-130">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [UserIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85ef3-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85ef3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85ef3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85ef3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85ef3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="85ef3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85ef3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="85ef3-134">C#</span><span class="sxs-lookup"><span data-stu-id="85ef3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85ef3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85ef3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85ef3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85ef3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85ef3-137">Java</span><span class="sxs-lookup"><span data-stu-id="85ef3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85ef3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="85ef3-138">Response</span></span>
><span data-ttu-id="85ef3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85ef3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="85ef3-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="85ef3-141">See also</span></span>

| <span data-ttu-id="85ef3-142">Método</span><span class="sxs-lookup"><span data-stu-id="85ef3-142">Method</span></span>           | <span data-ttu-id="85ef3-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85ef3-143">Return Type</span></span>    |<span data-ttu-id="85ef3-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="85ef3-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85ef3-145">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="85ef3-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="85ef3-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="85ef3-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="85ef3-147">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="85ef3-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="85ef3-148">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="85ef3-148">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="85ef3-149">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85ef3-149">None.</span></span>   |   <span data-ttu-id="85ef3-150">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="85ef3-150">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="85ef3-151">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="85ef3-151">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="85ef3-152">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85ef3-152">None.</span></span> |   <span data-ttu-id="85ef3-153">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="85ef3-153">Remove a reviewer from an accessReview.</span></span> |


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


