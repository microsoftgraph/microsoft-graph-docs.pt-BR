---
title: Obter accessReviewInstance
description: Recupere um objeto accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bd333a0620b8825400f89338112060c48611f302
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030737"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="47bbe-103">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="47bbe-103">Get accessReviewInstance</span></span>

<span data-ttu-id="47bbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47bbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47bbe-105">Recupere um [objeto accessReviewInstance](../resources/accessreviewinstance.md) usando o identificador de um accessReviewInstance e seu [acesso paiReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="47bbe-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="47bbe-106">Isso retorna todas as propriedades da instância, exceto o [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)associado.</span><span class="sxs-lookup"><span data-stu-id="47bbe-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="47bbe-107">Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="47bbe-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47bbe-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="47bbe-108">Permissions</span></span>
<span data-ttu-id="47bbe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bbe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47bbe-111">Permission type</span></span>                        | <span data-ttu-id="47bbe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47bbe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bbe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47bbe-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="47bbe-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47bbe-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="47bbe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47bbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47bbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47bbe-116">Not supported.</span></span>|
|<span data-ttu-id="47bbe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47bbe-117">Application</span></span>                            | <span data-ttu-id="47bbe-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47bbe-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="47bbe-119">Para chamar essa API, o usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="47bbe-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="47bbe-120">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="47bbe-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="47bbe-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47bbe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47bbe-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47bbe-122">Optional query parameters</span></span>
<span data-ttu-id="47bbe-123">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47bbe-123">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="47bbe-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47bbe-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47bbe-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbe-125">Request headers</span></span>
<span data-ttu-id="47bbe-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47bbe-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="47bbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbe-127">Request body</span></span>
<span data-ttu-id="47bbe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47bbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bbe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bbe-129">Response</span></span>
<span data-ttu-id="47bbe-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47bbe-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47bbe-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47bbe-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="47bbe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbe-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="47bbe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="47bbe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24
```
# <a name="c"></a>[<span data-ttu-id="47bbe-134">C#</span><span class="sxs-lookup"><span data-stu-id="47bbe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47bbe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47bbe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47bbe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47bbe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47bbe-137">Java</span><span class="sxs-lookup"><span data-stu-id="47bbe-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---



### <a name="response"></a><span data-ttu-id="47bbe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bbe-138">Response</span></span>
><span data-ttu-id="47bbe-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47bbe-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('6af553ce-104d-4842-ab5f-67d7b556e9dd')/instances/$entity",
    "id": "9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24",
    "startDateTime": "2021-03-11T16:44:59.337Z",
    "endDateTime": "2021-06-09T16:44:59.337Z",
    "status": "InProgress",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/97eebd44-61fd-4d42-8b2a-a4de41b6c572/transitiveMembers",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    }
}
```

## <a name="see-also"></a><span data-ttu-id="47bbe-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="47bbe-140">See also</span></span>

- [<span data-ttu-id="47bbe-141">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="47bbe-141">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="47bbe-142">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="47bbe-142">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
