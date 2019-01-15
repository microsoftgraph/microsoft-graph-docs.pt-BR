---
title: Obter accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, recuperar um objeto accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a13776b9aa215d752797b6ba2de2f477660ed31d
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016652"
---
# <a name="get-accessreview"></a><span data-ttu-id="e3946-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="e3946-103">Get accessReview</span></span>

> <span data-ttu-id="e3946-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3946-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3946-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3946-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3946-106">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere um objeto de [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="e3946-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="e3946-107">Para recuperar os revisores da revisão access, use os [Revisores de accessReview lista](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="e3946-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="e3946-108">Para recuperar as decisões da revisão access, use a API de [decisões de accessReview de lista](accessreview-listdecisions.md) ou a API de [Listar Minhas decisões accessReview](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="e3946-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="e3946-109">Se essa for uma análise mais acesso recorrente, em seguida, use o `instances` relação para recuperar uma coleção de [accessReview](../resources/accessreview.md) de passado, instâncias atuais e futuros da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="e3946-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3946-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3946-110">Permissions</span></span>
<span data-ttu-id="e3946-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3946-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3946-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3946-113">Permission type</span></span>                        | <span data-ttu-id="e3946-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3946-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3946-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3946-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3946-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e3946-116"></span></span>  <span data-ttu-id="e3946-117">O usuário conectado também deve ser em uma função de diretório que permite que uma revisão de acesso de leitura ou atribuído como um revisor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="e3946-117">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="e3946-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3946-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3946-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3946-119">Not supported.</span></span> |
|<span data-ttu-id="e3946-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3946-120">Application</span></span>                            | <span data-ttu-id="e3946-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3946-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3946-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3946-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="e3946-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3946-123">Request headers</span></span>
| <span data-ttu-id="e3946-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e3946-124">Name</span></span>         | <span data-ttu-id="e3946-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3946-125">Type</span></span>        | <span data-ttu-id="e3946-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3946-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3946-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3946-127">Authorization</span></span> | <span data-ttu-id="e3946-128">string</span><span class="sxs-lookup"><span data-stu-id="e3946-128">string</span></span> | <span data-ttu-id="e3946-129">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="e3946-129">Bearer \{token\}.</span></span> <span data-ttu-id="e3946-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3946-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3946-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3946-131">Request body</span></span>
<span data-ttu-id="e3946-132">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="e3946-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e3946-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3946-133">Response</span></span>
<span data-ttu-id="e3946-134">Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3946-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3946-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3946-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3946-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3946-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="e3946-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3946-137">Response</span></span>
><span data-ttu-id="e3946-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3946-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e3946-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="e3946-140">See also</span></span>

| <span data-ttu-id="e3946-141">Método</span><span class="sxs-lookup"><span data-stu-id="e3946-141">Method</span></span>           | <span data-ttu-id="e3946-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3946-142">Return Type</span></span>    |<span data-ttu-id="e3946-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3946-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3946-144">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="e3946-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="e3946-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="e3946-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e3946-146">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="e3946-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="e3946-147">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="e3946-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="e3946-148">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e3946-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="e3946-149">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="e3946-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="e3946-150">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="e3946-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="e3946-151">coleção [userIdentity](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="e3946-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="e3946-152">Obtenha os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="e3946-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="e3946-153">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="e3946-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="e3946-154">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="e3946-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="e3946-155">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="e3946-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="e3946-156">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="e3946-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="e3946-157">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="e3946-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="e3946-158">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="e3946-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
