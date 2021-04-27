---
title: Atualizar accessReview
description: No recurso de análises de acesso do Azure AD, atualize um objeto accessReview existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1b3870b4d44847d93fb2438c9f61d8ac3529433e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048439"
---
# <a name="update-accessreview"></a><span data-ttu-id="d49e3-103">Atualizar accessReview</span><span class="sxs-lookup"><span data-stu-id="d49e3-103">Update accessReview</span></span>

<span data-ttu-id="d49e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d49e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d49e3-105">No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d49e3-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="d49e3-106">Essa API não se destina a alterar os revisadores ou decisões de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="d49e3-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="d49e3-107">Para alterar os revisores, use [as APIs addReviewer](accessreview-addreviewer.md) [ou removeReviewer.](accessreview-removereviewer.md)</span><span class="sxs-lookup"><span data-stu-id="d49e3-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="d49e3-108">Para interromper uma revisão já iniciada uma vez ou uma instância já iniciada de uma revisão recorrente, antes, use a API [stop.](accessreview-stop.md)</span><span class="sxs-lookup"><span data-stu-id="d49e3-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="d49e3-109">Para aplicar as decisões ao grupo de destino ou aos direitos de acesso ao aplicativo, use a API [de aplicação.](accessreview-apply.md)</span><span class="sxs-lookup"><span data-stu-id="d49e3-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d49e3-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d49e3-110">Permissions</span></span>
<span data-ttu-id="d49e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d49e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49e3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d49e3-113">Permission type</span></span>                        | <span data-ttu-id="d49e3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d49e3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d49e3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d49e3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d49e3-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d49e3-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d49e3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d49e3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d49e3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d49e3-118">Not supported.</span></span> |
|<span data-ttu-id="d49e3-119">Application</span><span class="sxs-lookup"><span data-stu-id="d49e3-119">Application</span></span>                            | <span data-ttu-id="d49e3-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="d49e3-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="d49e3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d49e3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="d49e3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d49e3-122">Request headers</span></span>
| <span data-ttu-id="d49e3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d49e3-123">Name</span></span>         | <span data-ttu-id="d49e3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d49e3-124">Type</span></span>        | <span data-ttu-id="d49e3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d49e3-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d49e3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d49e3-126">Authorization</span></span> | <span data-ttu-id="d49e3-127">string</span><span class="sxs-lookup"><span data-stu-id="d49e3-127">string</span></span> | <span data-ttu-id="d49e3-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49e3-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d49e3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d49e3-130">Request body</span></span>
<span data-ttu-id="d49e3-131">No corpo da solicitação, fornece uma representação JSON dos parâmetros de um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="d49e3-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="d49e3-132">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d49e3-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="d49e3-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d49e3-133">Property</span></span>     | <span data-ttu-id="d49e3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d49e3-134">Type</span></span>        | <span data-ttu-id="d49e3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d49e3-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="d49e3-136">O nome da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d49e3-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="d49e3-137">DateTime quando a revisão está agendada para ser inicial.</span><span class="sxs-lookup"><span data-stu-id="d49e3-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="d49e3-138">Essa deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="d49e3-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="d49e3-139">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="d49e3-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="d49e3-140">Isso deve ser pelo menos um dia depois da data de início.</span><span class="sxs-lookup"><span data-stu-id="d49e3-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="d49e3-141">A descrição, para mostrar aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="d49e3-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="d49e3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49e3-142">Response</span></span>
<span data-ttu-id="d49e3-143">Se tiver êxito, este método retornará um código de resposta e um `204, Accepted` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d49e3-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49e3-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d49e3-144">Example</span></span>

<span data-ttu-id="d49e3-145">Este é um exemplo de atualização de uma revisão de acesso única (não recorrente).</span><span class="sxs-lookup"><span data-stu-id="d49e3-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="d49e3-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d49e3-146">Request</span></span>
<span data-ttu-id="d49e3-147">No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="d49e3-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="d49e3-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d49e3-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="c"></a>[<span data-ttu-id="d49e3-149">C#</span><span class="sxs-lookup"><span data-stu-id="d49e3-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d49e3-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d49e3-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d49e3-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d49e3-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d49e3-152">Java</span><span class="sxs-lookup"><span data-stu-id="d49e3-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d49e3-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49e3-153">Response</span></span>
><span data-ttu-id="d49e3-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d49e3-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


