---
title: Listar accessReviewInstances
description: Obter uma lista dos objetos accessReviewInstance e suas propriedades.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60b5ba7e35acfb72f033f90cd37d4fd32c8a3d8b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210574"
---
# <a name="list-accessreviewinstances"></a><span data-ttu-id="cd1ab-103">Listar accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="cd1ab-103">List accessReviewInstances</span></span>
<span data-ttu-id="cd1ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd1ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd1ab-105">Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-105">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="cd1ab-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="cd1ab-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="cd1ab-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="cd1ab-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd1ab-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd1ab-109">Permissions</span></span>
<span data-ttu-id="cd1ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd1ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd1ab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd1ab-112">Permission type</span></span>|<span data-ttu-id="cd1ab-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd1ab-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd1ab-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd1ab-114">Delegated (work or school account)</span></span>|<span data-ttu-id="cd1ab-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd1ab-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="cd1ab-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd1ab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd1ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-117">Not supported.</span></span>|
|<span data-ttu-id="cd1ab-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd1ab-118">Application</span></span>|<span data-ttu-id="cd1ab-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd1ab-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd1ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd1ab-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd1ab-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd1ab-121">Optional query parameters</span></span>
<span data-ttu-id="cd1ab-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="cd1ab-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cd1ab-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd1ab-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd1ab-124">Request headers</span></span>
|<span data-ttu-id="cd1ab-125">Nome</span><span class="sxs-lookup"><span data-stu-id="cd1ab-125">Name</span></span>|<span data-ttu-id="cd1ab-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd1ab-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd1ab-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd1ab-127">Authorization</span></span>|<span data-ttu-id="cd1ab-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd1ab-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd1ab-130">Request body</span></span>
<span data-ttu-id="cd1ab-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd1ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd1ab-132">Response</span></span>

<span data-ttu-id="cd1ab-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd1ab-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd1ab-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd1ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd1ab-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cd1ab-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd1ab-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances
```
# <a name="c"></a>[<span data-ttu-id="cd1ab-137">C#</span><span class="sxs-lookup"><span data-stu-id="cd1ab-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd1ab-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd1ab-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd1ab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd1ab-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd1ab-140">Java</span><span class="sxs-lookup"><span data-stu-id="cd1ab-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cd1ab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd1ab-141">Response</span></span>
><span data-ttu-id="cd1ab-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd1ab-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
