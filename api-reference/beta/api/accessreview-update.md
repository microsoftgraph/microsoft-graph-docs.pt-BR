---
title: Atualizar accessReview
description: No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para alterar uma ou mais das suas propriedades.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524363"
---
# <a name="update-accessreview"></a><span data-ttu-id="6d3dc-103">Atualizar accessReview</span><span class="sxs-lookup"><span data-stu-id="6d3dc-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d3dc-104">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais das suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="6d3dc-105">Essa API não deve alterar os revisores ou decisões de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="6d3dc-106">Para alterar os revisores, use o [addReviewer](accessreview-addreviewer.md) ou [removeReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="6d3dc-107">Para interromper uma revisão ocasional já iniciado ou uma instância já iniciado de uma revisão recorrente, no início, use o [Parar](accessreview-stop.md) API.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="6d3dc-108">Para aplicar as decisões os direitos de acesso de grupo ou o aplicativo de destino, use a [Aplicar](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="6d3dc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d3dc-109">Permissions</span></span>
<span data-ttu-id="6d3dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d3dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d3dc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d3dc-112">Permission type</span></span>                        | <span data-ttu-id="6d3dc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d3dc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d3dc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d3dc-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d3dc-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d3dc-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="6d3dc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d3dc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d3dc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-117">Not supported.</span></span> |
|<span data-ttu-id="6d3dc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d3dc-118">Application</span></span>                            | <span data-ttu-id="6d3dc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d3dc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d3dc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="6d3dc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d3dc-121">Request headers</span></span>
| <span data-ttu-id="6d3dc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6d3dc-122">Name</span></span>         | <span data-ttu-id="6d3dc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3dc-123">Type</span></span>        | <span data-ttu-id="6d3dc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3dc-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6d3dc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d3dc-125">Authorization</span></span> | <span data-ttu-id="6d3dc-126">string</span><span class="sxs-lookup"><span data-stu-id="6d3dc-126">string</span></span> | <span data-ttu-id="6d3dc-127">Token de portador</span><span class="sxs-lookup"><span data-stu-id="6d3dc-127">Bearer \{token\}.</span></span> <span data-ttu-id="6d3dc-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d3dc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d3dc-129">Request body</span></span>
<span data-ttu-id="6d3dc-130">No corpo da solicitação, fornece uma representação JSON dos parâmetros de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3dc-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="6d3dc-131">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="6d3dc-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d3dc-132">Property</span></span>     | <span data-ttu-id="6d3dc-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3dc-133">Type</span></span>        | <span data-ttu-id="6d3dc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3dc-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="6d3dc-135">O nome de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="6d3dc-136">DateTime quando a revisão está agendada para ser iniciar.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="6d3dc-137">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="6d3dc-138">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="6d3dc-139">Isto deve ser de pelo menos um dia mais recente do que a data de início.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="6d3dc-140">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="6d3dc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d3dc-141">Response</span></span>
<span data-ttu-id="6d3dc-142">Se tiver êxito, este método retornará um `204, Accepted` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d3dc-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d3dc-143">Example</span></span>

<span data-ttu-id="6d3dc-144">Este é um exemplo de atualização de uma única revisão de acesso (não recorrentes).</span><span class="sxs-lookup"><span data-stu-id="6d3dc-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="6d3dc-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d3dc-145">Request</span></span>
<span data-ttu-id="6d3dc-146">No corpo da solicitação, fornece uma representação JSON das novas propriedades do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3dc-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a><span data-ttu-id="6d3dc-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d3dc-147">Response</span></span>
><span data-ttu-id="6d3dc-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d3dc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
