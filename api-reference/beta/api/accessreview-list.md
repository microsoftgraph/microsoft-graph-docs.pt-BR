---
title: Listar accessReviews
description: Recupere objetos accessReview para um businessFlowTemplate.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 443ffc2c5a31ac33cba89cb689884a3bae4ab645
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048488"
---
# <a name="list-accessreviews"></a><span data-ttu-id="ebcf4-103">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="ebcf4-103">List accessReviews</span></span>

<span data-ttu-id="ebcf4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebcf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebcf4-105">Recupere os [objetos accessReview](../resources/accessreview.md) para um [determinado businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ebcf4-105">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="ebcf4-106">Uma lista de zero ou mais objetos **accessReview** são retornados, para cada revisão de acesso única e recorrente que foi criada com esse modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-106">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="ebcf4-107">Observe que as IDs do modelo de fluxo de negócios são sensíveis a minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-107">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="ebcf4-108">Se qualquer uma das avaliações de acesso que correspondem ao filtro for uma revisão de acesso recorrente, um objeto **accessReview** será retornado para representar cada série recorrente como um todo, além de qualquer instância atual, passada e próxima.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-108">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole, in addition to any current, past and the next upcoming instance.</span></span> <span data-ttu-id="ebcf4-109">Por exemplo, se houver uma revisão de acesso recorrente mensal de membros convidados do grupo A, uma revisão de acesso recorrente trimestral de membros convidados do grupo B e uma revisão de acesso único de membros convidados do grupo C, cada uma dessas recorrências acabou de ser iniciada e o chamador consulta para análises de acesso com um modelo de fluxo de negócios de avaliações de membros convidados de grupos , três objetos serão retornados representando as três séries, bem como três objetos para as instâncias de revisão de acesso atuais e, potencialmente, três objetos para as próximas instâncias.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-109">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, each of these recurrences have just started, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned representing the three series, as well as three objects for the current access review instances, and potentially three objects for the next upcoming instances.</span></span> <span data-ttu-id="ebcf4-110">Para recuperar as instâncias de uma revisão de acesso recorrente ou a instância de revisão de  acesso agendada para um determinado mês ou trimestre, o chamador pode navegar subsequentemente pela relação de instância do objeto **accessReview** recorrente.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-110">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="ebcf4-111">A **relação** de instância se vincula aos **objetos accessReview** para uma instância atual ou anterior da revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-111">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="ebcf4-112">Se muitas análises de acesso corresponderem ao filtro, para melhorar a eficiência e evitar tempos-de-tempo, recupere o resultado definido em páginas, incluindo o parâmetro de consulta com um tamanho de página, por exemplo, 100 e o parâmetro de consulta na `$top` `$skip=0` solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-112">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="ebcf4-113">Esses parâmetros podem ser incluídos mesmo quando você não previu que a solicitação abrange várias páginas.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-113">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="ebcf4-114">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade na resposta que contém uma URL para `@odata.nextLink` a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-114">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="ebcf4-115">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="ebcf4-115">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="ebcf4-116">Os **objetos accessReview** retornados por essa API não incluirão propriedades de estrutura aninhadas, como **configurações** ou relações.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-116">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="ebcf4-117">Para recuperar as configurações ou as relações de revisão de acesso, use a API [get accessReview.](accessreview-get.md)</span><span class="sxs-lookup"><span data-stu-id="ebcf4-117">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="ebcf4-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebcf4-118">Permissions</span></span>
<span data-ttu-id="ebcf4-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcf4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcf4-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebcf4-121">Permission type</span></span>                        | <span data-ttu-id="ebcf4-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebcf4-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcf4-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebcf4-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebcf4-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcf4-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="ebcf4-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebcf4-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcf4-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-126">Not supported.</span></span> |
|<span data-ttu-id="ebcf4-127">Application</span><span class="sxs-lookup"><span data-stu-id="ebcf4-127">Application</span></span>                            | <span data-ttu-id="ebcf4-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="ebcf4-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="ebcf4-129">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-129">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="ebcf4-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcf4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="ebcf4-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcf4-131">Request headers</span></span>
| <span data-ttu-id="ebcf4-132">Nome</span><span class="sxs-lookup"><span data-stu-id="ebcf4-132">Name</span></span>         | <span data-ttu-id="ebcf4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebcf4-133">Type</span></span>        | <span data-ttu-id="ebcf4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcf4-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ebcf4-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebcf4-135">Authorization</span></span> | <span data-ttu-id="ebcf4-136">string</span><span class="sxs-lookup"><span data-stu-id="ebcf4-136">string</span></span> | <span data-ttu-id="ebcf4-p106">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebcf4-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcf4-139">Request body</span></span>
<span data-ttu-id="ebcf4-140">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-140">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="ebcf4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcf4-141">Response</span></span>
<span data-ttu-id="ebcf4-142">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-142">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebcf4-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ebcf4-143">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="ebcf4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcf4-144">Request</span></span>
<span data-ttu-id="ebcf4-145">O exemplo a seguir mostra uma solicitação para recuperar todas as análises de acesso único e recorrente para um modelo de fluxo de negócios '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-145">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebcf4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcf4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="ebcf4-147">C#</span><span class="sxs-lookup"><span data-stu-id="ebcf4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebcf4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebcf4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebcf4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebcf4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebcf4-150">Java</span><span class="sxs-lookup"><span data-stu-id="ebcf4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a><span data-ttu-id="ebcf4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcf4-151">Response</span></span>
><span data-ttu-id="ebcf4-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ebcf4-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ebcf4-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="ebcf4-153">See also</span></span>

- [<span data-ttu-id="ebcf4-154">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="ebcf4-154">Get accessReview</span></span>](accessreview-get.md)


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


