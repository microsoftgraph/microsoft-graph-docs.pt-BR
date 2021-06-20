---
title: Listar accessReviewInstances
description: Obter uma lista dos objetos accessReviewInstance e suas propriedades.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 01a52e1b597971d887b763076913e8db0c70abc7
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031005"
---
# <a name="list-accessreviewinstances"></a><span data-ttu-id="1682d-103">Listar accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="1682d-103">List accessReviewInstances</span></span>
<span data-ttu-id="1682d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1682d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1682d-105">Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1682d-105">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="1682d-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="1682d-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="1682d-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="1682d-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="1682d-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1682d-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="1682d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1682d-109">Permissions</span></span>
<span data-ttu-id="1682d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1682d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1682d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1682d-112">Permission type</span></span>|<span data-ttu-id="1682d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1682d-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1682d-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1682d-114">Delegated (work or school account)</span></span>|<span data-ttu-id="1682d-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1682d-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="1682d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1682d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1682d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1682d-117">Not supported.</span></span>|
|<span data-ttu-id="1682d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1682d-118">Application</span></span>|<span data-ttu-id="1682d-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1682d-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1682d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1682d-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1682d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1682d-121">Optional query parameters</span></span>
<span data-ttu-id="1682d-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1682d-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1682d-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1682d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1682d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1682d-124">Request headers</span></span>
|<span data-ttu-id="1682d-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1682d-125">Name</span></span>|<span data-ttu-id="1682d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1682d-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1682d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1682d-127">Authorization</span></span>|<span data-ttu-id="1682d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1682d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1682d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1682d-130">Request body</span></span>
<span data-ttu-id="1682d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1682d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1682d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1682d-132">Response</span></span>

<span data-ttu-id="1682d-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1682d-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1682d-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1682d-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1682d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1682d-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances
```


### <a name="response"></a><span data-ttu-id="1682d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1682d-136">Response</span></span>
><span data-ttu-id="1682d-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1682d-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
