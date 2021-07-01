---
title: Listar instâncias
description: Obter os recursos accessReviewInstance da propriedade de navegação de instâncias.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4cf4701e99754e80e59700fcf7542c5496812430
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208607"
---
# <a name="list-instances"></a><span data-ttu-id="8d1b3-103">Instâncias de lista</span><span class="sxs-lookup"><span data-stu-id="8d1b3-103">List instances</span></span>
<span data-ttu-id="8d1b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d1b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d1b3-105">Obter os [recursos accessReviewInstance](../resources/accessreviewinstance.md) da propriedade de navegação de instâncias em [um accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8d1b3-105">Get the [accessReviewInstance](../resources/accessreviewinstance.md) resources from the instances navigation property on an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

>[!NOTE]
><span data-ttu-id="8d1b3-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="8d1b3-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="8d1b3-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="8d1b3-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d1b3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d1b3-109">Permissions</span></span>
<span data-ttu-id="8d1b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d1b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d1b3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d1b3-112">Permission type</span></span>|<span data-ttu-id="8d1b3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d1b3-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d1b3-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d1b3-114">Delegated (work or school account)</span></span>|<span data-ttu-id="8d1b3-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b3-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8d1b3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d1b3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d1b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-117">Not supported.</span></span>|
|<span data-ttu-id="8d1b3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d1b3-118">Application</span></span>|<span data-ttu-id="8d1b3-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b3-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d1b3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d1b3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d1b3-121">Optional query parameters</span></span>
<span data-ttu-id="8d1b3-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8d1b3-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8d1b3-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d1b3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b3-124">Request headers</span></span>
|<span data-ttu-id="8d1b3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8d1b3-125">Name</span></span>|<span data-ttu-id="8d1b3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d1b3-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d1b3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d1b3-127">Authorization</span></span>|<span data-ttu-id="8d1b3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d1b3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b3-130">Request body</span></span>
<span data-ttu-id="8d1b3-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d1b3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b3-132">Response</span></span>

<span data-ttu-id="8d1b3-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d1b3-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d1b3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d1b3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b3-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8d1b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances
```
# <a name="c"></a>[<span data-ttu-id="8d1b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="8d1b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d1b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d1b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d1b3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d1b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d1b3-140">Java</span><span class="sxs-lookup"><span data-stu-id="8d1b3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8d1b3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b3-141">Response</span></span>
><span data-ttu-id="8d1b3-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d1b3-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2dca8959-b716-4b4c-a93d-a535c01eb6e0')/instances",
    "@odata.count": 1,
    "value": [
        {
            "id": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "startDateTime": "2021-05-01T07:00:00Z",
            "endDateTime": "2021-05-15T07:00:00Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/0914d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
