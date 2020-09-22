---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff7b4eeb6cd7e4e71e5eb71ab19ebe3112e10c5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983554"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="2cabc-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="2cabc-103">List accessReview reviewers</span></span>

<span data-ttu-id="2cabc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cabc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cabc-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="2cabc-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2cabc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cabc-106">Permissions</span></span>
<span data-ttu-id="2cabc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cabc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cabc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cabc-109">Permission type</span></span>                        | <span data-ttu-id="2cabc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cabc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cabc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cabc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cabc-112">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2cabc-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2cabc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cabc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cabc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cabc-114">Not supported.</span></span> |
|<span data-ttu-id="2cabc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cabc-115">Application</span></span>                            | <span data-ttu-id="2cabc-116">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="2cabc-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="2cabc-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="2cabc-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cabc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cabc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="2cabc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cabc-119">Request headers</span></span>
| <span data-ttu-id="2cabc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2cabc-120">Name</span></span>         | <span data-ttu-id="2cabc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cabc-121">Type</span></span>        | <span data-ttu-id="2cabc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cabc-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2cabc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cabc-123">Authorization</span></span> | <span data-ttu-id="2cabc-124">string</span><span class="sxs-lookup"><span data-stu-id="2cabc-124">string</span></span> | <span data-ttu-id="2cabc-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cabc-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cabc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cabc-127">Request body</span></span>
<span data-ttu-id="2cabc-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="2cabc-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="2cabc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cabc-129">Response</span></span>
<span data-ttu-id="2cabc-130">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [UserIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cabc-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cabc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cabc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cabc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cabc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2cabc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cabc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="2cabc-134">C#</span><span class="sxs-lookup"><span data-stu-id="2cabc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cabc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cabc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cabc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cabc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cabc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cabc-137">Response</span></span>
><span data-ttu-id="2cabc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cabc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2cabc-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2cabc-140">See also</span></span>

| <span data-ttu-id="2cabc-141">Método</span><span class="sxs-lookup"><span data-stu-id="2cabc-141">Method</span></span>           | <span data-ttu-id="2cabc-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2cabc-142">Return Type</span></span>    |<span data-ttu-id="2cabc-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cabc-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cabc-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="2cabc-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="2cabc-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="2cabc-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="2cabc-146">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="2cabc-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="2cabc-147">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="2cabc-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="2cabc-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2cabc-148">None.</span></span>   |   <span data-ttu-id="2cabc-149">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="2cabc-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="2cabc-150">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="2cabc-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="2cabc-151">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2cabc-151">None.</span></span> |   <span data-ttu-id="2cabc-152">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="2cabc-152">Remove a reviewer from an accessReview.</span></span> |


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


