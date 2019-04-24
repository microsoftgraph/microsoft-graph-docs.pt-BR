---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458765"
---
# <a name="get-accessreview"></a><span data-ttu-id="17baf-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17baf-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="17baf-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="17baf-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="17baf-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="17baf-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="17baf-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="17baf-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="17baf-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="17baf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="17baf-108">Permissions</span></span>
<span data-ttu-id="17baf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17baf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17baf-111">Permission type</span></span>                        | <span data-ttu-id="17baf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17baf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="17baf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17baf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="17baf-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="17baf-114"></span></span>  <span data-ttu-id="17baf-115">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="17baf-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="17baf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17baf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17baf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17baf-117">Not supported.</span></span> |
|<span data-ttu-id="17baf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17baf-118">Application</span></span>                            | <span data-ttu-id="17baf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17baf-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17baf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17baf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="17baf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17baf-121">Request headers</span></span>
| <span data-ttu-id="17baf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="17baf-122">Name</span></span>         | <span data-ttu-id="17baf-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="17baf-123">Type</span></span>        | <span data-ttu-id="17baf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="17baf-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="17baf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="17baf-125">Authorization</span></span> | <span data-ttu-id="17baf-126">string</span><span class="sxs-lookup"><span data-stu-id="17baf-126">string</span></span> | <span data-ttu-id="17baf-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17baf-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17baf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17baf-129">Request body</span></span>
<span data-ttu-id="17baf-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="17baf-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="17baf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="17baf-131">Response</span></span>
<span data-ttu-id="17baf-132">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17baf-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17baf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17baf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17baf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17baf-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="17baf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17baf-135">Response</span></span>
><span data-ttu-id="17baf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17baf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="17baf-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="17baf-138">See also</span></span>

| <span data-ttu-id="17baf-139">Método</span><span class="sxs-lookup"><span data-stu-id="17baf-139">Method</span></span>           | <span data-ttu-id="17baf-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17baf-140">Return Type</span></span>    |<span data-ttu-id="17baf-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="17baf-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17baf-142">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="17baf-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="17baf-144">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="17baf-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="17baf-145">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="17baf-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="17baf-146">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="17baf-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="17baf-147">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="17baf-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="17baf-148">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="17baf-149">[](../resources/useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="17baf-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="17baf-150">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="17baf-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="17baf-151">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="17baf-152">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="17baf-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="17baf-153">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="17baf-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="17baf-154">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="17baf-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="17baf-155">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="17baf-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="17baf-156">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="17baf-156">As a reviewer, get my decisions of an accessReview.</span></span>|


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
