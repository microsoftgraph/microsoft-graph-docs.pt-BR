---
title: 'accessReviewInstance: filterByCurrentUser'
description: Retorna todos os objetos accessReviewInstance para um determinado revisor.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db6de64071645fe97d5fffa4e3968ea63db5578e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031430"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="25315-103">accessReviewInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="25315-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="25315-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25315-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25315-105">Retorna todos os objetos [accessReviewInstance](../resources/accessreviewinstance.md) em um [determinado accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) onde o usuário de chamada é um revisor em um ou mais [objetos accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="25315-105">Returns all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="25315-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="25315-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="25315-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="25315-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="25315-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="25315-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="25315-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="25315-109">Permissions</span></span>
<span data-ttu-id="25315-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25315-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25315-112">Permission type</span></span>|<span data-ttu-id="25315-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25315-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25315-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25315-114">Delegated (work or school account)</span></span>|<span data-ttu-id="25315-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25315-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="25315-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25315-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25315-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25315-117">Not supported.</span></span>|
|<span data-ttu-id="25315-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25315-118">Application</span></span>|<span data-ttu-id="25315-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25315-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25315-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25315-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25315-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25315-121">Optional query parameters</span></span>
<span data-ttu-id="25315-122">Este método oferece `$select` suporte `$filter` a parâmetros de consulta , , e `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25315-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="25315-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="25315-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="25315-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25315-124">Request headers</span></span>
|<span data-ttu-id="25315-125">Nome</span><span class="sxs-lookup"><span data-stu-id="25315-125">Name</span></span>|<span data-ttu-id="25315-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="25315-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25315-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="25315-127">Authorization</span></span>|<span data-ttu-id="25315-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25315-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25315-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25315-130">Request body</span></span>
<span data-ttu-id="25315-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25315-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25315-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="25315-132">Response</span></span>

<span data-ttu-id="25315-133">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25315-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25315-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="25315-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25315-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25315-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')
```

### <a name="response"></a><span data-ttu-id="25315-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="25315-136">Response</span></span>
><span data-ttu-id="25315-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="25315-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "7ca879f0-77ea-4386-b110-776dec898935",
            "startDateTime": "2021-04-20T00:45:51.627Z",
            "endDateTime": "2021-04-23T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "00ef5dba-4a32-48b3-b18a-57b244c0c4ba",
            "startDateTime": "2021-04-13T00:45:51.627Z",
            "endDateTime": "2021-04-16T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
