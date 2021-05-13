---
title: Listar accessReviewHistoryDefinitions
description: Obter uma lista dos objetos accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 633b8e075f9bbeedf47e24fcebf560a85d2590d6
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474138"
---
# <a name="list-accessreviewhistorydefinitions"></a><span data-ttu-id="bb107-103">Listar accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="bb107-103">List accessReviewHistoryDefinitions</span></span>
<span data-ttu-id="bb107-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb107-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb107-105">Recupere os [objetos accessReviewHistoryDefinition criados](../resources/accessreviewhistorydefinition.md) nos últimos 30 dias, incluindo todas as propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="bb107-105">Retrieve the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects created in the last 30 days, including all nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="bb107-106">O tamanho padrão da página para essa API é de 100 **objetos accessReviewHistoryDefinitions.**</span><span class="sxs-lookup"><span data-stu-id="bb107-106">The default page size for this API is 100 **accessReviewHistoryDefinitions** objects.</span></span> <span data-ttu-id="bb107-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="bb107-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="bb107-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="bb107-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
>
><span data-ttu-id="bb107-109">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="bb107-109">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb107-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb107-110">Permissions</span></span>

<span data-ttu-id="bb107-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb107-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb107-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb107-113">Permission type</span></span>|<span data-ttu-id="bb107-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb107-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb107-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb107-115">Delegated (work or school account)</span></span>|<span data-ttu-id="bb107-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb107-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="bb107-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb107-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb107-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb107-118">Not supported.</span></span>|
|<span data-ttu-id="bb107-119">Application</span><span class="sxs-lookup"><span data-stu-id="bb107-119">Application</span></span>|<span data-ttu-id="bb107-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb107-120">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="bb107-121">Se o usuário de entrada não for um membro de função de diretório do Administrador Global ou um membro da função de diretório Leitor Global, somente as definições criadas pelo usuário in-loco serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="bb107-121">If the signed-in user is not a Global Admin directory role member or a Global Reader directory role member, only the definitions that the signed-in user created will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb107-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb107-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb107-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb107-123">Optional query parameters</span></span>
<span data-ttu-id="bb107-124">Este método dá suporte `$top` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$skip` a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb107-124">This method supports the `$top`, `$filter`, and `$skip` OData query parameters to help customize the response.</span></span> <span data-ttu-id="bb107-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bb107-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span> 

## <a name="request-headers"></a><span data-ttu-id="bb107-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb107-126">Request headers</span></span>
|<span data-ttu-id="bb107-127">Nome</span><span class="sxs-lookup"><span data-stu-id="bb107-127">Name</span></span>|<span data-ttu-id="bb107-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb107-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb107-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb107-129">Authorization</span></span>|<span data-ttu-id="bb107-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb107-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb107-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb107-132">Request body</span></span>
<span data-ttu-id="bb107-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb107-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb107-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb107-134">Response</span></span>

<span data-ttu-id="bb107-135">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb107-135">If successful, this method returns a `200 OK` response code and a collection of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb107-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb107-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb107-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb107-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bb107-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb107-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
```
# <a name="c"></a>[<span data-ttu-id="bb107-139">C#</span><span class="sxs-lookup"><span data-stu-id="bb107-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb107-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb107-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb107-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb107-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb107-142">Java</span><span class="sxs-lookup"><span data-stu-id="bb107-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bb107-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb107-143">Response</span></span>
><span data-ttu-id="bb107-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bb107-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "isCollection": "true"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.count": 1,
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
      "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
      "displayName": "Last quarter's group reviews April 2021",
      "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
      "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
      "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
      ],
      "status": "done",
      "createdDateTime": "2021-04-14T00:22:48.9392594Z",
      "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
      "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
      "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
      },
      "scopes": [
        {
          "@odata.type": "#microsoft.graph.accessReviewQueryScope",
          "queryType": "MicrosoftGraph",     
          "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
          "queryRoot": null
        },  
        {
          "@odata.type": "#microsoft.graph.accessReviewQueryScope",
          "queryType": "MicrosoftGraph",     
          "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
          "queryRoot": null
        }
      ]
    }
  ]
}
```
