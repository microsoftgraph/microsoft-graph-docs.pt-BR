---
title: Atualizar accessReview
description: No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ab56d4c9ffaced579b4b1933f461227cccb25ff
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049512"
---
# <a name="update-accessreview"></a><span data-ttu-id="56025-103">Atualizar accessReview</span><span class="sxs-lookup"><span data-stu-id="56025-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56025-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="56025-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="56025-105">Esta API não se destina a alterar os revisores ou as decisões de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="56025-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="56025-106">Para alterar os revisores, use as [](accessreview-addreviewer.md) APIs revisar ou [removeReviewer](accessreview-removereviewer.md) .</span><span class="sxs-lookup"><span data-stu-id="56025-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="56025-107">Para interromper uma revisão única já iniciada ou uma instância já iniciada de uma revisão recorrente, antes, use a API de [parada](accessreview-stop.md) .</span><span class="sxs-lookup"><span data-stu-id="56025-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="56025-108">Para aplicar as decisões ao grupo de destino ou aos direitos de acesso do aplicativo, use a API [aplicar](accessreview-apply.md) .</span><span class="sxs-lookup"><span data-stu-id="56025-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="56025-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="56025-109">Permissions</span></span>
<span data-ttu-id="56025-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56025-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56025-112">Permission type</span></span>                        | <span data-ttu-id="56025-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56025-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="56025-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56025-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="56025-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56025-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="56025-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56025-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56025-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56025-117">Not supported.</span></span> |
|<span data-ttu-id="56025-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56025-118">Application</span></span>                            | <span data-ttu-id="56025-119">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="56025-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="56025-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56025-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="56025-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56025-121">Request headers</span></span>
| <span data-ttu-id="56025-122">Nome</span><span class="sxs-lookup"><span data-stu-id="56025-122">Name</span></span>         | <span data-ttu-id="56025-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="56025-123">Type</span></span>        | <span data-ttu-id="56025-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="56025-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="56025-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="56025-125">Authorization</span></span> | <span data-ttu-id="56025-126">string</span><span class="sxs-lookup"><span data-stu-id="56025-126">string</span></span> | <span data-ttu-id="56025-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56025-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56025-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56025-129">Request body</span></span>
<span data-ttu-id="56025-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="56025-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="56025-131">A tabela a seguir mostra as propriedades que podem ser fornecidas ao atualizar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="56025-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="56025-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56025-132">Property</span></span>     | <span data-ttu-id="56025-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="56025-133">Type</span></span>        | <span data-ttu-id="56025-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="56025-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="56025-135">O nome de revisão do acesso.</span><span class="sxs-lookup"><span data-stu-id="56025-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="56025-136">O DateTime quando a revisão está agendada para ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="56025-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="56025-137">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="56025-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="56025-138">O DateTime quando a revisão é agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="56025-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="56025-139">Este deve ser pelo menos um dia depois da data de início.</span><span class="sxs-lookup"><span data-stu-id="56025-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="56025-140">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="56025-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="56025-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="56025-141">Response</span></span>
<span data-ttu-id="56025-142">Se tiver êxito, este método retornará `204, Accepted` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56025-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56025-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56025-143">Example</span></span>

<span data-ttu-id="56025-144">Este é um exemplo de atualização de uma revisão de acesso de uma única vez (sem refazêvel).</span><span class="sxs-lookup"><span data-stu-id="56025-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="56025-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56025-145">Request</span></span>
<span data-ttu-id="56025-146">No corpo da solicitação, forneça uma representação JSON das novas propriedades do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="56025-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56025-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="56025-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="56025-148">C#</span><span class="sxs-lookup"><span data-stu-id="56025-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56025-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="56025-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56025-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="56025-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="56025-151">Java</span><span class="sxs-lookup"><span data-stu-id="56025-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56025-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="56025-152">Response</span></span>
><span data-ttu-id="56025-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56025-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
