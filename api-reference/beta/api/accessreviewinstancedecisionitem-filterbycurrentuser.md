---
title: 'accessReviewInstanceDecisionItem: filterByCurrentUser'
description: Recupera todos os objetos accessReviewInstanceDecisionItem em um accessReviewInstance para o qual o usuário de chamada é o revisor.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f4f045ac67e1b98179f64a5a09102c975a2f0374
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031427"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a><span data-ttu-id="1c223-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="1c223-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span></span>
<span data-ttu-id="1c223-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c223-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c223-105">Recupera todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em um [determinado accessReviewInstance](../resources/accessreviewinstance.md) para o qual o usuário de chamada é o revisor.</span><span class="sxs-lookup"><span data-stu-id="1c223-105">Retrieves all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on a given [accessReviewInstance](../resources/accessreviewinstance.md) for which the calling user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="1c223-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstanceDecisionItem.</span><span class="sxs-lookup"><span data-stu-id="1c223-106">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="1c223-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="1c223-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="1c223-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1c223-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c223-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c223-109">Permissions</span></span>
<span data-ttu-id="1c223-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c223-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c223-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c223-112">Permission type</span></span>|<span data-ttu-id="1c223-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c223-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c223-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c223-114">Delegated (work or school account)</span></span>|<span data-ttu-id="1c223-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c223-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="1c223-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c223-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c223-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c223-117">Not supported.</span></span>|
|<span data-ttu-id="1c223-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c223-118">Application</span></span>|<span data-ttu-id="1c223-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c223-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c223-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c223-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c223-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c223-121">Optional query parameters</span></span>
<span data-ttu-id="1c223-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c223-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1c223-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c223-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c223-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c223-124">Request headers</span></span>
|<span data-ttu-id="1c223-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1c223-125">Name</span></span>|<span data-ttu-id="1c223-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c223-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c223-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c223-127">Authorization</span></span>|<span data-ttu-id="1c223-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c223-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c223-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c223-130">Request body</span></span>
<span data-ttu-id="1c223-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c223-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c223-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c223-132">Response</span></span>

<span data-ttu-id="1c223-133">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c223-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c223-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c223-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c223-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c223-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="1c223-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c223-136">Response</span></span>
><span data-ttu-id="1c223-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c223-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
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
                "userPrincipalName": "guest@contoso.com"
            }
        }
    ]
}
```
