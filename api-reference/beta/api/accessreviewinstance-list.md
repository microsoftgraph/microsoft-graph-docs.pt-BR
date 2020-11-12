---
title: Listar accessReviewInstance
description: Recuperar objetos accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844564c383b065adc80672cad727807cbb590ca7
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000741"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="4a874-103">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="4a874-103">List accessReviewInstance</span></span>

<span data-ttu-id="4a874-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a874-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a874-105">Recupere os objetos [accessReviewInstance](../resources/accessreviewinstance.md) para um [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)específico.</span><span class="sxs-lookup"><span data-stu-id="4a874-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="4a874-106">Uma lista de zero ou mais objetos **accessReviewInstance** é retornada, incluindo todas as suas propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="4a874-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="4a874-107">Os objetos retornados não incluem accessReviewInstanceDecisionItems associados.</span><span class="sxs-lookup"><span data-stu-id="4a874-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="4a874-108">Para recuperar as decisões na instância, use [list accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="4a874-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="4a874-109">Se muitos **accessReviewInstances** forem retornados, para melhorar a eficiência e evitar tempos limite, recupere o conjunto de resultados nas páginas, incluindo o parâmetro de consulta $Top com um tamanho de página de no máximo 100, e o parâmetro de consulta $Skip = 0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a874-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="4a874-110">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata. nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="4a874-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="4a874-111">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata. nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito em paginação de dados do Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a874-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="4a874-112">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph pausará automaticamente os resultados a 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="4a874-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a874-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a874-113">Permissions</span></span>
<span data-ttu-id="4a874-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a874-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a874-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a874-116">Permission type</span></span>                        | <span data-ttu-id="4a874-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a874-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a874-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a874-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a874-119">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4a874-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4a874-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a874-120">Application</span></span>                            | <span data-ttu-id="4a874-121">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4a874-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="4a874-122">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="4a874-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="4a874-123">Para exibir apenas as instâncias em que o usuário conectado recebeu o revisor, consulte [list Pending Access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="4a874-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="4a874-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a874-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="4a874-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a874-125">Request headers</span></span>
<span data-ttu-id="4a874-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4a874-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="4a874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a874-127">Request body</span></span>
<span data-ttu-id="4a874-128">Não forneça um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a874-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="4a874-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a874-129">Response</span></span>
<span data-ttu-id="4a874-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma matriz de objetos [accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a874-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a874-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a874-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4a874-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a874-132">Request</span></span>
<span data-ttu-id="4a874-133">O exemplo a seguir mostra uma solicitação para recuperar todas as instâncias de análise de acesso para uma definição.</span><span class="sxs-lookup"><span data-stu-id="4a874-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```

### <a name="response"></a><span data-ttu-id="4a874-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a874-134">Response</span></span>
><span data-ttu-id="4a874-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a874-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
            "startDateTime": "2020-09-21T20:03:36Z",
            "endDateTime": "2020-09-23T20:03:36Z",
            "status": "NotStarted",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        },
        {
            "id": "64444761-b89f-4d9c-afb9-fcfc8bb9cf45",
            "startDateTime": "2020-09-14T20:03:36.74Z",
            "endDateTime": "2020-09-16T20:03:36.74Z",
            "status": "Completed",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="4a874-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="4a874-137">See also</span></span>

- [<span data-ttu-id="4a874-138">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4a874-138">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="4a874-139">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="4a874-139">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
