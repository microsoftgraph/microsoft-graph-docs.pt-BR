---
title: Listar accessReviews
description: Recuperar objetos accessReview para um businessFlowTemplate.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1e138f7b255053797bc671adcad7ce20ed99480
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119511"
---
# <a name="list-accessreviews"></a><span data-ttu-id="63124-103">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="63124-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63124-104">Recupere os objetos [accessReview](../resources/accessreview.md) para um determinado [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="63124-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="63124-105">Uma lista de zero ou mais objetos **accessReview** são retornadas para cada revisão de acesso único e recorrente que foi criada com esse modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="63124-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="63124-106">Observe que as IDs do modelo de fluxo de negócios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="63124-106">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="63124-107">Se qualquer uma das revisões do Access que corresponderem ao filtro for uma análise de acesso recorrente, um objeto **accessReview** será retornado para representar cada série recorrente como um todo.</span><span class="sxs-lookup"><span data-stu-id="63124-107">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="63124-108">Por exemplo, se houver uma revisão de acesso recorrente mensal de membros convidados do grupo A, uma revisão trimestral de acesso recorrente de membros convidados do grupo B e uma revisão de acesso de um único tempo de membros convidados do grupo C e o chamador consulta as revisões de acesso com um fluxo de negócios modelo de revisões de membros convidados de grupos, serão retornados três objetos.</span><span class="sxs-lookup"><span data-stu-id="63124-108">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="63124-109">Para recuperar as instâncias de uma revisão de acesso recorrente ou a instância de revisão do Access agendada para um mês ou trimestre específico, o chamador pode, subsequentemente, navegar na relação de **instância** do objeto **accessReview** recorrente.</span><span class="sxs-lookup"><span data-stu-id="63124-109">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="63124-110">A relação de **instância** vincula aos objetos **accessReview** para uma instância atual ou passada da revisão recorrente do acesso.</span><span class="sxs-lookup"><span data-stu-id="63124-110">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="63124-111">Se muitas revisões de acesso corresponderem ao filtro, para melhorar a eficiência e evitar tempos limite, recupere o conjunto de resultados nas páginas `$top` , incluindo o parâmetro de consulta com um tamanho de página, por `$skip=0` exemplo, 100, e o parâmetro de consulta na solicitação.</span><span class="sxs-lookup"><span data-stu-id="63124-111">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="63124-112">Esses parâmetros podem ser incluídos, mesmo quando você não prevê que a solicitação vai estender várias páginas.</span><span class="sxs-lookup"><span data-stu-id="63124-112">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="63124-113">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com `@odata.nextLink` uma propriedade na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="63124-113">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="63124-114">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="63124-114">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="63124-115">Os objetos **accessReview** retornados por essa API não incluirão Propriedades de estrutura aninhadas, como **configurações**ou relações.</span><span class="sxs-lookup"><span data-stu-id="63124-115">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="63124-116">Para recuperar as configurações ou relações de revisão do Access, use a API [Get accessReview](accessreview-get.md) .</span><span class="sxs-lookup"><span data-stu-id="63124-116">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="63124-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="63124-117">Permissions</span></span>
<span data-ttu-id="63124-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63124-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63124-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63124-120">Permission type</span></span>                        | <span data-ttu-id="63124-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63124-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="63124-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63124-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="63124-123">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="63124-123">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="63124-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63124-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63124-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63124-125">Not supported.</span></span> |
|<span data-ttu-id="63124-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63124-126">Application</span></span>                            | <span data-ttu-id="63124-127">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="63124-127">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="63124-128">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="63124-128">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="63124-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63124-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="63124-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63124-130">Request headers</span></span>
| <span data-ttu-id="63124-131">Nome</span><span class="sxs-lookup"><span data-stu-id="63124-131">Name</span></span>         | <span data-ttu-id="63124-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="63124-132">Type</span></span>        | <span data-ttu-id="63124-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="63124-133">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="63124-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="63124-134">Authorization</span></span> | <span data-ttu-id="63124-135">string</span><span class="sxs-lookup"><span data-stu-id="63124-135">string</span></span> | <span data-ttu-id="63124-p106">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63124-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63124-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63124-138">Request body</span></span>
<span data-ttu-id="63124-139">Não forneça um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63124-139">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="63124-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="63124-140">Response</span></span>
<span data-ttu-id="63124-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma matriz de objetos [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63124-141">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63124-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="63124-142">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="63124-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63124-143">Request</span></span>
<span data-ttu-id="63124-144">O exemplo a seguir mostra uma solicitação para recuperar todas as revisões de acesso único e recorrentes de um modelo de fluxo de negócios ' 6e4f3d20-c5c3-407F-9695-8460952bcc68 '.</span><span class="sxs-lookup"><span data-stu-id="63124-144">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63124-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="63124-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63124-146">C#</span><span class="sxs-lookup"><span data-stu-id="63124-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63124-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63124-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63124-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63124-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
null
---


##### <a name="response"></a><span data-ttu-id="63124-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="63124-149">Response</span></span>
><span data-ttu-id="63124-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63124-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="63124-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="63124-152">See also</span></span>

- [<span data-ttu-id="63124-153">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="63124-153">Get accessReview</span></span>](accessreview-get.md)


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
