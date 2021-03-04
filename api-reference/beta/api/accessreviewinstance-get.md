---
title: Obter accessReviewInstance
description: Recupere um objeto accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5f475f966d3ddc8539431c76fc613e3d6e0044e4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439189"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="f083a-103">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f083a-103">Get accessReviewInstance</span></span>

<span data-ttu-id="f083a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f083a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f083a-105">Recupere um [objeto accessReviewInstance](../resources/accessreviewinstance.md) usando o identificador de um accessReviewInstance e seu [acesso paiReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f083a-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="f083a-106">Isso retorna todas as propriedades da instância, exceto o [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)associado.</span><span class="sxs-lookup"><span data-stu-id="f083a-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="f083a-107">Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="f083a-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f083a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f083a-108">Permissions</span></span>
<span data-ttu-id="f083a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f083a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f083a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f083a-111">Permission type</span></span>                        | <span data-ttu-id="f083a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f083a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f083a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f083a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f083a-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f083a-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f083a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f083a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f083a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f083a-116">Not supported.</span></span>|
|<span data-ttu-id="f083a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f083a-117">Application</span></span>                            | <span data-ttu-id="f083a-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f083a-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="f083a-119">Para chamar essa API, o usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="f083a-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="f083a-120">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="f083a-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="f083a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f083a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="f083a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f083a-122">Request headers</span></span>
<span data-ttu-id="f083a-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f083a-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f083a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f083a-124">Request body</span></span>
<span data-ttu-id="f083a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f083a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f083a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f083a-126">Response</span></span>
<span data-ttu-id="f083a-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f083a-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f083a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f083a-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f083a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f083a-129">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="f083a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f083a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/12490cdb-6a18-4c08-ba2c-44442f0a0138
```
# <a name="c"></a>[<span data-ttu-id="f083a-131">C#</span><span class="sxs-lookup"><span data-stu-id="f083a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f083a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f083a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f083a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f083a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f083a-134">Java</span><span class="sxs-lookup"><span data-stu-id="f083a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f083a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f083a-135">Response</span></span>
><span data-ttu-id="f083a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f083a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
    "startDateTime": "2020-09-21T20:03:36Z",
    "endDateTime": "2020-09-23T20:03:36Z",
    "status": "NotStarted",
    "scope": {
        "query": "/groups/b7a4444b-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="f083a-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="f083a-138">See also</span></span>

- [<span data-ttu-id="f083a-139">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f083a-139">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="f083a-140">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f083a-140">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
