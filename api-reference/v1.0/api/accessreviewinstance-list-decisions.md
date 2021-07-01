---
title: Listar decisões
description: Obter os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 116c2c1b6bb4da87673c204536226c20990696cf
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209790"
---
# <a name="list-decisions"></a><span data-ttu-id="03af2-103">Listar decisões</span><span class="sxs-lookup"><span data-stu-id="03af2-103">List decisions</span></span>
<span data-ttu-id="03af2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03af2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03af2-105">Obter os [recursos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) da propriedade de navegação de decisões em um [determinado accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="03af2-105">Get the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) resources from the decisions navigation property on a given [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

>[!NOTE]
><span data-ttu-id="03af2-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="03af2-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="03af2-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="03af2-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="03af2-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="03af2-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="03af2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="03af2-109">Permissions</span></span>
<span data-ttu-id="03af2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03af2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03af2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03af2-112">Permission type</span></span>|<span data-ttu-id="03af2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03af2-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03af2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03af2-114">Delegated (work or school account)</span></span>|<span data-ttu-id="03af2-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03af2-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="03af2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03af2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03af2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03af2-117">Not supported.</span></span>|
|<span data-ttu-id="03af2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03af2-118">Application</span></span>|<span data-ttu-id="03af2-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03af2-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03af2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03af2-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03af2-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03af2-121">Optional query parameters</span></span>
<span data-ttu-id="03af2-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03af2-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="03af2-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="03af2-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="03af2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03af2-124">Request headers</span></span>
|<span data-ttu-id="03af2-125">Nome</span><span class="sxs-lookup"><span data-stu-id="03af2-125">Name</span></span>|<span data-ttu-id="03af2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="03af2-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03af2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="03af2-127">Authorization</span></span>|<span data-ttu-id="03af2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03af2-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03af2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03af2-130">Request body</span></span>
<span data-ttu-id="03af2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03af2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03af2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="03af2-132">Response</span></span>

<span data-ttu-id="03af2-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03af2-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03af2-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03af2-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03af2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03af2-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03af2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="03af2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances/8d035c9d-798d-47fa-beb4-f986a4b8126f/decisions
```
# <a name="c"></a>[<span data-ttu-id="03af2-137">C#</span><span class="sxs-lookup"><span data-stu-id="03af2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03af2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03af2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03af2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03af2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03af2-140">Java</span><span class="sxs-lookup"><span data-stu-id="03af2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="03af2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="03af2-141">Response</span></span>
><span data-ttu-id="03af2-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="03af2-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2dca8959-b716-4b4c-a93d-a535c01eb6e0')/instances('8d035c9d-798d-47fa-beb4-f986a4b8126f')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "guest example",
                "userPrincipalName": "guest@guest.com"
            }
        }
    ]
}
```
