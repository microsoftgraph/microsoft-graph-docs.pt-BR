---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 263749521e199079dc8b4d9b352eb9c2cb5adf35
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323642"
---
# <a name="get-accessreview"></a><span data-ttu-id="7cff7-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cff7-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="7cff7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="7cff7-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="7cff7-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="7cff7-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="7cff7-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="7cff7-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="7cff7-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cff7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cff7-108">Permissions</span></span>
<span data-ttu-id="7cff7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cff7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cff7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cff7-111">Permission type</span></span>                        | <span data-ttu-id="7cff7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cff7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cff7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cff7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cff7-114">AccessReview. Read. All</span><span class="sxs-lookup"><span data-stu-id="7cff7-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="7cff7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cff7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cff7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cff7-116">Not supported.</span></span> |
|<span data-ttu-id="7cff7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cff7-117">Application</span></span>                            | <span data-ttu-id="7cff7-118">AccessReview. Read. All</span><span class="sxs-lookup"><span data-stu-id="7cff7-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="7cff7-119">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="7cff7-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="7cff7-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="7cff7-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="7cff7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cff7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="7cff7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cff7-122">Request headers</span></span>
| <span data-ttu-id="7cff7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7cff7-123">Name</span></span>         | <span data-ttu-id="7cff7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cff7-124">Type</span></span>        | <span data-ttu-id="7cff7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cff7-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7cff7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cff7-126">Authorization</span></span> | <span data-ttu-id="7cff7-127">string</span><span class="sxs-lookup"><span data-stu-id="7cff7-127">string</span></span> | <span data-ttu-id="7cff7-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cff7-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cff7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cff7-130">Request body</span></span>
<span data-ttu-id="7cff7-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="7cff7-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7cff7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cff7-132">Response</span></span>
<span data-ttu-id="7cff7-133">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cff7-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cff7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cff7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cff7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cff7-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```

##### <a name="response"></a><span data-ttu-id="7cff7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cff7-136">Response</span></span>
><span data-ttu-id="7cff7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cff7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7cff7-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="7cff7-139">See also</span></span>

| <span data-ttu-id="7cff7-140">Método</span><span class="sxs-lookup"><span data-stu-id="7cff7-140">Method</span></span>           | <span data-ttu-id="7cff7-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7cff7-141">Return Type</span></span>    |<span data-ttu-id="7cff7-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cff7-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cff7-143">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="7cff7-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="7cff7-145">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="7cff7-145">Create a new accessReview.</span></span> |
|[<span data-ttu-id="7cff7-146">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="7cff7-146">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="7cff7-147">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="7cff7-147">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="7cff7-148">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="7cff7-148">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="7cff7-149">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-149">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="7cff7-150">[](../resources/useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="7cff7-150">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="7cff7-151">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="7cff7-151">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="7cff7-152">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-152">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="7cff7-153">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="7cff7-153">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7cff7-154">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="7cff7-154">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="7cff7-155">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="7cff7-155">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="7cff7-156">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="7cff7-156">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7cff7-157">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="7cff7-157">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
