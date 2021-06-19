---
title: Listar decisões
description: Obter os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 74de88c1e14e9983580a80c1c1698842eaddc8f9
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031429"
---
# <a name="list-decisions"></a><span data-ttu-id="599c4-103">Listar decisões</span><span class="sxs-lookup"><span data-stu-id="599c4-103">List decisions</span></span>
<span data-ttu-id="599c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="599c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="599c4-105">Obter os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) das decisões em [um accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="599c4-105">Get the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects from the decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

>[!NOTE]
><span data-ttu-id="599c4-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="599c4-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="599c4-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="599c4-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="599c4-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="599c4-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="599c4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="599c4-109">Permissions</span></span>
<span data-ttu-id="599c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="599c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="599c4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="599c4-112">Permission type</span></span>|<span data-ttu-id="599c4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="599c4-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="599c4-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="599c4-114">Delegated (work or school account)</span></span>|<span data-ttu-id="599c4-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599c4-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="599c4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="599c4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="599c4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="599c4-117">Not supported.</span></span>|
|<span data-ttu-id="599c4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="599c4-118">Application</span></span>|<span data-ttu-id="599c4-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599c4-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="599c4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="599c4-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="599c4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="599c4-121">Optional query parameters</span></span>
<span data-ttu-id="599c4-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="599c4-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="599c4-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="599c4-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="599c4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="599c4-124">Request headers</span></span>
|<span data-ttu-id="599c4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="599c4-125">Name</span></span>|<span data-ttu-id="599c4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="599c4-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="599c4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="599c4-127">Authorization</span></span>|<span data-ttu-id="599c4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="599c4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="599c4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="599c4-130">Request body</span></span>
<span data-ttu-id="599c4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="599c4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="599c4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="599c4-132">Response</span></span>

<span data-ttu-id="599c4-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="599c4-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="599c4-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="599c4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="599c4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="599c4-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/decisions
```


### <a name="response"></a><span data-ttu-id="599c4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="599c4-136">Response</span></span>
><span data-ttu-id="599c4-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="599c4-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('16d424f6-0100-4bf1-9ebc-fe009c5e5006')/instances('bb14c722-51b8-4962-9bd2-1d96ba773d80')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "bfbd4d74-275c-4368-aaa1-06c93838d0d5",
            "accessReviewId": "bb14c722-51b8-4962-9bd2-1d96ba773d80",
            "reviewedDateTime": "2021-05-05T16:48:28.79Z",
            "decision": "Deny",
            "justification": "bye alexxxxx",
            "appliedDateTime": "2021-05-05T16:50:30.9Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/540da31b-4d25-4934-b7f7-98bc230eb15a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "ff15bedb-22de-49ad-b2d7-59656607484d",
                "displayName": "group owner",
                "userPrincipalName": "group owner"
            },
            "appliedBy": {
                "id": "8798d204-fa3c-4d7b-977d-bc939b8a0848",
                "displayName": "Access Reviews",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        }
    ]
}
```
