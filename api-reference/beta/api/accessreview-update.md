---
title: Atualizar accessReview
description: No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para alterar uma ou mais das suas propriedades.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e09219c1979f974b62f17c52163fc93b5d2d3c2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941349"
---
# <a name="update-accessreview"></a><span data-ttu-id="48755-103">Atualizar accessReview</span><span class="sxs-lookup"><span data-stu-id="48755-103">Update accessReview</span></span>

> <span data-ttu-id="48755-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48755-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48755-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48755-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48755-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais das suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="48755-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="48755-107">Essa API não deve alterar os revisores ou decisões de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="48755-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="48755-108">Para alterar os revisores, use o [addReviewer](accessreview-addreviewer.md) ou [removeReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="48755-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="48755-109">Para interromper uma revisão ocasional já iniciado ou uma instância já iniciado de uma revisão recorrente, no início, use o [Parar](accessreview-stop.md) API e para aplicar as decisões para os destino grupo ou app direitos de acesso, use a [Aplicar](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="48755-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API, and to apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="48755-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="48755-110">Permissions</span></span>
<span data-ttu-id="48755-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48755-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48755-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48755-113">Permission type</span></span>                        | <span data-ttu-id="48755-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48755-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="48755-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48755-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="48755-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48755-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="48755-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48755-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48755-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48755-118">Not supported.</span></span> |
|<span data-ttu-id="48755-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48755-119">Application</span></span>                            | <span data-ttu-id="48755-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48755-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48755-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48755-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="48755-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48755-122">Request headers</span></span>
| <span data-ttu-id="48755-123">Nome</span><span class="sxs-lookup"><span data-stu-id="48755-123">Name</span></span>         | <span data-ttu-id="48755-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="48755-124">Type</span></span>        | <span data-ttu-id="48755-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="48755-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="48755-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="48755-126">Authorization</span></span> | <span data-ttu-id="48755-127">string</span><span class="sxs-lookup"><span data-stu-id="48755-127">string</span></span> | <span data-ttu-id="48755-128">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="48755-128">Bearer \{token\}.</span></span> <span data-ttu-id="48755-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48755-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48755-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48755-130">Request body</span></span>
<span data-ttu-id="48755-131">No corpo da solicitação, fornece uma representação de JSON dos parâmetros de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="48755-131">In the request body, supply a JSON representation of a parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="48755-132">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.</span><span class="sxs-lookup"><span data-stu-id="48755-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="48755-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48755-133">Property</span></span>     | <span data-ttu-id="48755-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="48755-134">Type</span></span>        | <span data-ttu-id="48755-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="48755-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="48755-136">O nome de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="48755-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="48755-137">DateTime quando a revisão está agendada para ser iniciar.</span><span class="sxs-lookup"><span data-stu-id="48755-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="48755-138">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="48755-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="48755-139">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="48755-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="48755-140">Isto deve ser de pelo menos um dia mais recente do que a data de início.</span><span class="sxs-lookup"><span data-stu-id="48755-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="48755-141">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="48755-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="48755-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="48755-142">Response</span></span>
<span data-ttu-id="48755-143">Se tiver êxito, este método retornará um `204, Accepted` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48755-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48755-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48755-144">Example</span></span>

<span data-ttu-id="48755-145">Este é um exemplo de atualização de uma única revisão de acesso (não recorrentes).</span><span class="sxs-lookup"><span data-stu-id="48755-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="48755-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48755-146">Request</span></span>
<span data-ttu-id="48755-147">No corpo da solicitação, fornece uma representação JSON das novas propriedades do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="48755-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="48755-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="48755-148">Response</span></span>
><span data-ttu-id="48755-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48755-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
