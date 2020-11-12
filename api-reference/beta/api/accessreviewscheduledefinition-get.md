---
title: Obter accessReviewScheduleDefinition
description: Recupere um objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6c5619222eb8a96fbf54a8f796abdc2d2bb85ec
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000731"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="3e317-103">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="3e317-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="3e317-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e317-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e317-105">Recupere um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="3e317-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="3e317-106">Isso retorna todas as propriedades da série de revisão do Access agendada, exceto a accessReviewInstances associada.</span><span class="sxs-lookup"><span data-stu-id="3e317-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="3e317-107">Cada accessReviewScheduleDefinition tem pelo menos uma instância.</span><span class="sxs-lookup"><span data-stu-id="3e317-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="3e317-108">Uma instância representa uma revisão para um recurso específico (como membros de um determinado grupo), durante uma ocorrência (por exemplo, 2021 de março) de uma revisão recorrente.</span><span class="sxs-lookup"><span data-stu-id="3e317-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="3e317-109">Para recuperar as instâncias da série de revisão do Access, use a API [list accessReviewInstance](accessreviewinstance-list.md) .</span><span class="sxs-lookup"><span data-stu-id="3e317-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e317-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e317-110">Permissions</span></span>
<span data-ttu-id="3e317-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e317-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e317-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e317-113">Permission type</span></span>                        | <span data-ttu-id="3e317-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e317-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e317-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e317-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e317-116">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3e317-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="3e317-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e317-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e317-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e317-118">Not supported.</span></span>|
|<span data-ttu-id="3e317-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e317-119">Application</span></span>                            | <span data-ttu-id="3e317-120">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3e317-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="3e317-121">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="3e317-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="3e317-122">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="3e317-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e317-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e317-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="3e317-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e317-124">Request headers</span></span>
<span data-ttu-id="3e317-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3e317-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="3e317-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e317-126">Request body</span></span>
<span data-ttu-id="3e317-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e317-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e317-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e317-128">Response</span></span>
<span data-ttu-id="3e317-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e317-129">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e317-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e317-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="3e317-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e317-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
---

### <a name="response"></a><span data-ttu-id="3e317-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e317-132">Response</span></span>
><span data-ttu-id="3e317-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e317-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "createdDateTime": "2020-09-14T20:03:36.7391027Z",
    "lastModifiedDateTime": "2020-09-14T20:04:28Z",
    "status": "InProgress",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "createdBy": {
        "id": "957f1027-c0ee-460d-4444-b8828e59e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="3e317-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="3e317-135">See also</span></span>

- [<span data-ttu-id="3e317-136">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="3e317-136">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-create.md)
- [<span data-ttu-id="3e317-137">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="3e317-137">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="3e317-138">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="3e317-138">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
