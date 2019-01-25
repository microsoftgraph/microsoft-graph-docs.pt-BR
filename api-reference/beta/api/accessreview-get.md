---
title: Obter accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, recuperar um objeto accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529142"
---
# <a name="get-accessreview"></a><span data-ttu-id="56ba1-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="56ba1-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56ba1-104">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere um objeto de [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="56ba1-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="56ba1-105">Para recuperar os revisores da revisão access, use os [Revisores de accessReview lista](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="56ba1-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="56ba1-106">Para recuperar as decisões da revisão access, use a API de [decisões de accessReview de lista](accessreview-listdecisions.md) ou a API de [Listar Minhas decisões accessReview](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="56ba1-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="56ba1-107">Se essa for uma análise mais acesso recorrente, em seguida, use o `instances` relação para recuperar uma coleção de [accessReview](../resources/accessreview.md) de passado, instâncias atuais e futuros da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="56ba1-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="56ba1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="56ba1-108">Permissions</span></span>
<span data-ttu-id="56ba1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ba1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ba1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56ba1-111">Permission type</span></span>                        | <span data-ttu-id="56ba1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56ba1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="56ba1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56ba1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="56ba1-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="56ba1-114"></span></span>  <span data-ttu-id="56ba1-115">O usuário conectado também deve ser em uma função de diretório que permite que uma revisão de acesso de leitura ou atribuído como um revisor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="56ba1-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="56ba1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56ba1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ba1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ba1-117">Not supported.</span></span> |
|<span data-ttu-id="56ba1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56ba1-118">Application</span></span>                            | <span data-ttu-id="56ba1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ba1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ba1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ba1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="56ba1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ba1-121">Request headers</span></span>
| <span data-ttu-id="56ba1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="56ba1-122">Name</span></span>         | <span data-ttu-id="56ba1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ba1-123">Type</span></span>        | <span data-ttu-id="56ba1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ba1-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="56ba1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ba1-125">Authorization</span></span> | <span data-ttu-id="56ba1-126">string</span><span class="sxs-lookup"><span data-stu-id="56ba1-126">string</span></span> | <span data-ttu-id="56ba1-127">Token de portador</span><span class="sxs-lookup"><span data-stu-id="56ba1-127">Bearer \{token\}.</span></span> <span data-ttu-id="56ba1-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ba1-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56ba1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ba1-129">Request body</span></span>
<span data-ttu-id="56ba1-130">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="56ba1-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="56ba1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ba1-131">Response</span></span>
<span data-ttu-id="56ba1-132">Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ba1-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ba1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ba1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56ba1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ba1-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="56ba1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ba1-135">Response</span></span>
><span data-ttu-id="56ba1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56ba1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="56ba1-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="56ba1-138">See also</span></span>

| <span data-ttu-id="56ba1-139">Método</span><span class="sxs-lookup"><span data-stu-id="56ba1-139">Method</span></span>           | <span data-ttu-id="56ba1-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56ba1-140">Return Type</span></span>    |<span data-ttu-id="56ba1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ba1-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56ba1-142">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="56ba1-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="56ba1-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="56ba1-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="56ba1-144">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="56ba1-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="56ba1-145">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="56ba1-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="56ba1-146">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="56ba1-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="56ba1-147">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="56ba1-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="56ba1-148">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="56ba1-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="56ba1-149">coleção [userIdentity](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="56ba1-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="56ba1-150">Obtenha os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="56ba1-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="56ba1-151">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="56ba1-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="56ba1-152">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="56ba1-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="56ba1-153">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="56ba1-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="56ba1-154">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="56ba1-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="56ba1-155">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="56ba1-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="56ba1-156">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="56ba1-156">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
