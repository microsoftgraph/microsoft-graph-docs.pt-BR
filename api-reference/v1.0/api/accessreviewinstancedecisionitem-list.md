---
title: Listar accessReviewInstanceDecisionItems
description: Obter uma lista dos objetos accessReviewInstanceDecisionItem e suas propriedades.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1ffc4738de0cbef15aa9c440f9e1f80045df01bc
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030994"
---
# <a name="list-accessreviewinstancedecisionitems"></a><span data-ttu-id="69311-103">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="69311-103">List accessReviewInstanceDecisionItems</span></span>
<span data-ttu-id="69311-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69311-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69311-105">Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="69311-105">Get a list of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="69311-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="69311-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="69311-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="69311-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="69311-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="69311-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="69311-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="69311-109">Permissions</span></span>
<span data-ttu-id="69311-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69311-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69311-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69311-112">Permission type</span></span>|<span data-ttu-id="69311-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69311-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69311-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69311-114">Delegated (work or school account)</span></span>|<span data-ttu-id="69311-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69311-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="69311-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69311-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69311-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69311-117">Not supported.</span></span>|
|<span data-ttu-id="69311-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69311-118">Application</span></span>|<span data-ttu-id="69311-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69311-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69311-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69311-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69311-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="69311-121">Optional query parameters</span></span>
<span data-ttu-id="69311-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="69311-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="69311-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="69311-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="69311-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69311-124">Request headers</span></span>
|<span data-ttu-id="69311-125">Nome</span><span class="sxs-lookup"><span data-stu-id="69311-125">Name</span></span>|<span data-ttu-id="69311-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="69311-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69311-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="69311-127">Authorization</span></span>|<span data-ttu-id="69311-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69311-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69311-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69311-130">Request body</span></span>
<span data-ttu-id="69311-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69311-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69311-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="69311-132">Response</span></span>

<span data-ttu-id="69311-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69311-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69311-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69311-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69311-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69311-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/7070ea1c-8d12-457b-bd35-a37dc59e54e0/decisions
```


### <a name="response"></a><span data-ttu-id="69311-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="69311-136">Response</span></span>
><span data-ttu-id="69311-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="69311-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd')/instances('7070ea1c-8d12-457b-bd35-a37dc59e54e0')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "9550e25b-f315-4454-9d87-16b885c35de4",
            "accessReviewId": "7070ea1c-8d12-457b-bd35-a37dc59e54e0",
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
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "guest example",
                "userPrincipalName": "guest@guest.com"
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
