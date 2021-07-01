---
title: 'accessReviewInstance: filterByCurrentUser'
description: Recupere todos os objetos accessReviewInstance para um determinado revisor.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6d32cf12ed95c34cc82dd40a05e928f4069c1f51
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209839"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="00536-103">accessReviewInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="00536-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="00536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00536-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00536-105">Recupere todos os objetos [accessReviewInstance](../resources/accessreviewinstance.md) em um [determinado accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) onde o usuário de chamada é um revisor em um ou mais objetos [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="00536-105">Retrieve all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="00536-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="00536-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="00536-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="00536-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="00536-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="00536-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="00536-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="00536-109">Permissions</span></span>
<span data-ttu-id="00536-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00536-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00536-112">Permission type</span></span>|<span data-ttu-id="00536-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00536-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00536-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00536-114">Delegated (work or school account)</span></span>|<span data-ttu-id="00536-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00536-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="00536-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00536-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00536-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00536-117">Not supported.</span></span>|
|<span data-ttu-id="00536-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00536-118">Application</span></span>|<span data-ttu-id="00536-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00536-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00536-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00536-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00536-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00536-121">Optional query parameters</span></span>
<span data-ttu-id="00536-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00536-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="00536-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="00536-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="00536-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00536-124">Request headers</span></span>
|<span data-ttu-id="00536-125">Nome</span><span class="sxs-lookup"><span data-stu-id="00536-125">Name</span></span>|<span data-ttu-id="00536-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="00536-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="00536-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="00536-127">Authorization</span></span>|<span data-ttu-id="00536-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00536-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00536-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00536-130">Request body</span></span>
<span data-ttu-id="00536-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00536-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00536-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="00536-132">Response</span></span>

<span data-ttu-id="00536-133">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00536-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00536-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00536-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00536-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00536-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="00536-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="00536-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="00536-137">C#</span><span class="sxs-lookup"><span data-stu-id="00536-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00536-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00536-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00536-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00536-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00536-140">Java</span><span class="sxs-lookup"><span data-stu-id="00536-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="00536-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="00536-141">Response</span></span>
><span data-ttu-id="00536-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="00536-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 1,
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
        }
    ]
}
```
