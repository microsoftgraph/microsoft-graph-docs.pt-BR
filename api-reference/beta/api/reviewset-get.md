---
title: Obter reviewset
description: Recupere as propriedades e os relacionamentos de um objeto reviewset.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 6bbc6d0dc347e056740591ca401289534ffb179e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085441"
---
# <a name="get-reviewset"></a><span data-ttu-id="a15a2-103">Obter reviewset</span><span class="sxs-lookup"><span data-stu-id="a15a2-103">Get reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a15a2-104">Recupere as propriedades e os relacionamentos de um objeto [reviewset](../resources/reviewset.md) .</span><span class="sxs-lookup"><span data-stu-id="a15a2-104">Retrieve the properties and relationships of a [reviewSet](../resources/reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a15a2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a15a2-105">Permissions</span></span>

<span data-ttu-id="a15a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a15a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a15a2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a15a2-108">Permission type</span></span>                        | <span data-ttu-id="a15a2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a15a2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a15a2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a15a2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a15a2-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="a15a2-111">User.Read</span></span> |
| <span data-ttu-id="a15a2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a15a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a15a2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a15a2-113">Not supported.</span></span> |
| <span data-ttu-id="a15a2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a15a2-114">Application</span></span>                            | <span data-ttu-id="a15a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a15a2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a15a2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a15a2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a15a2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a15a2-117">Optional query parameters</span></span>

<span data-ttu-id="a15a2-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a15a2-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a15a2-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a15a2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="a15a2-120">Por padrão, todos os campos do conjunto de revisão são retornados; no entanto, você pode especificar certos campos a serem retornados usando o `$select` parâmetro de consulta OData.</span><span class="sxs-lookup"><span data-stu-id="a15a2-120">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="a15a2-121">Por exemplo, para retornar apenas **DisplayName** e ID, adicione o seguinte à sua consulta: `$select=displayName,Id` .</span><span class="sxs-lookup"><span data-stu-id="a15a2-121">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="a15a2-122">Como uma solicitação pode retornar muitos casos, você pode filtrá-los usando **DisplayName**.</span><span class="sxs-lookup"><span data-stu-id="a15a2-122">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="a15a2-123">Para filtrar por **DisplayName**, adicione o seguinte à sua consulta: `$filter=displayName eq 'rs1'` , onde o nome do conjunto de revisão é RS1.</span><span class="sxs-lookup"><span data-stu-id="a15a2-123">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="a15a2-124">Para obter mais informações sobre filtragem e especificação de campos, consulte [usando expressões de filtro em URIs OData ](https://docs.microsoft.com/dynamics-nav/using-filter-expressions-in-odata-uris).</span><span class="sxs-lookup"><span data-stu-id="a15a2-124">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](https://docs.microsoft.com/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a15a2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a15a2-125">Request headers</span></span>

| <span data-ttu-id="a15a2-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a15a2-126">Name</span></span>      |<span data-ttu-id="a15a2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a15a2-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a15a2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a15a2-128">Authorization</span></span> | <span data-ttu-id="a15a2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a15a2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a15a2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a15a2-131">Request body</span></span>

<span data-ttu-id="a15a2-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a15a2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a15a2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a15a2-133">Response</span></span>

<span data-ttu-id="a15a2-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [reviewset](../resources/reviewset.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a15a2-134">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a15a2-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a15a2-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a15a2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a15a2-136">Request</span></span>

<span data-ttu-id="a15a2-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a15a2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a15a2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a15a2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="a15a2-139">C#</span><span class="sxs-lookup"><span data-stu-id="a15a2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a15a2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a15a2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a15a2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a15a2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a15a2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a15a2-142">Response</span></span>

<span data-ttu-id="a15a2-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a15a2-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a15a2-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a15a2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


