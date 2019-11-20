---
title: Listar accessReviews
description: Recuperar objetos accessReview para um businessFlowTemplate.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa164aba8d59b2695ff39652e1ea12a587426321
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747143"
---
# <a name="list-accessreviews"></a><span data-ttu-id="9a19c-103">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="9a19c-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a19c-104">Recupere os objetos [accessReview](../resources/accessreview.md) para um determinado [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="9a19c-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="9a19c-105">Uma lista de zero ou mais objetos **accessReview** são retornadas para cada revisão de acesso único e recorrente que foi criada com esse modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="9a19c-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="9a19c-106">Observe que as IDs do modelo de fluxo de negócios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9a19c-106">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="9a19c-107">Se qualquer uma das revisões do Access que corresponderem ao filtro for uma análise de acesso recorrente, um objeto **accessReview** será retornado para representar cada série recorrente como um todo.</span><span class="sxs-lookup"><span data-stu-id="9a19c-107">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="9a19c-108">Por exemplo, se houver uma revisão de acesso recorrente mensal de membros convidados do grupo A, uma revisão trimestral de acesso recorrente de membros convidados do grupo B e uma revisão de acesso de um único tempo de membros convidados do grupo C e o chamador consulta as revisões de acesso com um fluxo de negócios modelo de revisões de membros convidados de grupos, serão retornados três objetos.</span><span class="sxs-lookup"><span data-stu-id="9a19c-108">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="9a19c-109">Para recuperar as instâncias de uma revisão de acesso recorrente ou a instância de revisão do Access agendada para um mês ou trimestre específico, o chamador pode, subsequentemente, navegar na relação de **instância** do objeto **accessReview** recorrente.</span><span class="sxs-lookup"><span data-stu-id="9a19c-109">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="9a19c-110">A relação de **instância** vincula aos objetos **accessReview** para uma instância atual ou passada da revisão recorrente do acesso.</span><span class="sxs-lookup"><span data-stu-id="9a19c-110">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a19c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a19c-111">Permissions</span></span>
<span data-ttu-id="9a19c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a19c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a19c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a19c-114">Permission type</span></span>                        | <span data-ttu-id="9a19c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a19c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a19c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a19c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a19c-117">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9a19c-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="9a19c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a19c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a19c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a19c-119">Not supported.</span></span> |
|<span data-ttu-id="9a19c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a19c-120">Application</span></span>                            | <span data-ttu-id="9a19c-121">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="9a19c-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="9a19c-122">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="9a19c-122">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="9a19c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a19c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a><span data-ttu-id="9a19c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a19c-124">Request headers</span></span>
| <span data-ttu-id="9a19c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9a19c-125">Name</span></span>         | <span data-ttu-id="9a19c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a19c-126">Type</span></span>        | <span data-ttu-id="9a19c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a19c-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9a19c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a19c-128">Authorization</span></span> | <span data-ttu-id="9a19c-129">string</span><span class="sxs-lookup"><span data-stu-id="9a19c-129">string</span></span> | <span data-ttu-id="9a19c-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a19c-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a19c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a19c-132">Request body</span></span>
<span data-ttu-id="9a19c-133">Não forneça um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a19c-133">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="9a19c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a19c-134">Response</span></span>
<span data-ttu-id="9a19c-135">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a19c-135">If successful, this method returns a `200, OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a19c-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a19c-136">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="9a19c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a19c-137">Request</span></span>
<span data-ttu-id="9a19c-138">O exemplo a seguir mostra uma solicitação para recuperar todas as revisões de acesso único e recorrentes de um modelo de fluxo de negócios ' 6e4f3d20-c5c3-407F-9695-8460952bcc68 '.</span><span class="sxs-lookup"><span data-stu-id="9a19c-138">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a19c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a19c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a19c-140">C#</span><span class="sxs-lookup"><span data-stu-id="9a19c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a19c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a19c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a19c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a19c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
null
---


##### <a name="response"></a><span data-ttu-id="9a19c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a19c-143">Response</span></span>
><span data-ttu-id="9a19c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a19c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="9a19c-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="9a19c-146">See also</span></span>

- [<span data-ttu-id="9a19c-147">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="9a19c-147">Get accessReview</span></span>](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
