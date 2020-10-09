---
title: 'searchEntity: consulta'
description: Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c699dab1c97d5b7650f42d4282e36d35b2769a31
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401796"
---
# <a name="searchentity-query"></a><span data-ttu-id="64a14-104">searchEntity: consulta</span><span class="sxs-lookup"><span data-stu-id="64a14-104">searchEntity: query</span></span>

<span data-ttu-id="64a14-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64a14-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a14-106">Executa a consulta especificada no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a14-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="64a14-107">Os resultados da pesquisa são fornecidos na resposta.</span><span class="sxs-lookup"><span data-stu-id="64a14-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="64a14-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64a14-108">Permissions</span></span>

<span data-ttu-id="64a14-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="64a14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64a14-111">Permission type</span></span>                        | <span data-ttu-id="64a14-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64a14-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="64a14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64a14-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64a14-114">Mail. Read, mail. ReadWrite, Calendars. Read, Calendars. ReadWrite, files. Read. All, files. ReadWrite. All, sites. Read. All, sites. ReadWrite. All, ExternalItem. Read. All</span><span class="sxs-lookup"><span data-stu-id="64a14-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="64a14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64a14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64a14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64a14-116">Not supported.</span></span> |
| <span data-ttu-id="64a14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64a14-117">Application</span></span>                            | <span data-ttu-id="64a14-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64a14-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64a14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64a14-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="64a14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64a14-120">Request headers</span></span>

| <span data-ttu-id="64a14-121">Nome</span><span class="sxs-lookup"><span data-stu-id="64a14-121">Name</span></span>          | <span data-ttu-id="64a14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a14-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="64a14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64a14-123">Authorization</span></span> | <span data-ttu-id="64a14-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64a14-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64a14-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="64a14-126">Content-type</span></span> | <span data-ttu-id="64a14-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64a14-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64a14-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64a14-129">Request body</span></span>

<span data-ttu-id="64a14-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a14-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="64a14-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64a14-131">Parameter</span></span>    | <span data-ttu-id="64a14-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="64a14-132">Type</span></span>        | <span data-ttu-id="64a14-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a14-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64a14-134">Quest</span><span class="sxs-lookup"><span data-stu-id="64a14-134">requests</span></span>|<span data-ttu-id="64a14-135">coleção [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="64a14-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="64a14-136">Uma coleção de uma ou mais solicitações de pesquisa cada formatadas em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="64a14-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="64a14-137">Cada blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="64a14-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="64a14-138">Esteja ciente das [limitações conhecidas](../resources/search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="64a14-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="64a14-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a14-139">Response</span></span>

<span data-ttu-id="64a14-140">Se bem-sucedido, este método retorna o `HTTP 200 OK` código de resposta e um objeto da coleção [searchResponse](../resources/searchresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64a14-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="64a14-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64a14-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64a14-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a14-142">Request</span></span>

<span data-ttu-id="64a14-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a14-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64a14-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="64a14-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_query"
}-->

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "queryString": "contoso product"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="64a14-145">C#</span><span class="sxs-lookup"><span data-stu-id="64a14-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64a14-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64a14-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64a14-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64a14-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64a14-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a14-148">Response</span></span>

<span data-ttu-id="64a14-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a14-149">The following is an example of the response.</span></span>

> <span data-ttu-id="64a14-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64a14-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
  "value": [
    {
      "searchTerms": [
        "searchTerms-value"
      ],
      "hitsContainers": [
        {
          "hits": [
            {
              "hitId": "1",
              "rank": 1,
              "summary": "_summary-value",
              "resource": "The source field will contain the underlying graph entity part of the response"
            }
          ],
          "total": 47,
          "moreResultsAvailable": true
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="64a14-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="64a14-152">See also</span></span>
- <span data-ttu-id="64a14-153">[Mensagens de email](/graph/search-concept-messages) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="64a14-153">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="64a14-154">[Eventos de calendário](/graph/search-concept-events) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="64a14-154">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="64a14-155">Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="64a14-155">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="64a14-156">Dados [de tipos personalizados de pesquisa (conectores do gráfico)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="64a14-156">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="64a14-157">[Classificar](/graph/search-concept-sort) resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="64a14-157">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="64a14-158">Usar [agregações](/graph/search-concept-aggregations) para refinar os resultados da pesquisa</span><span class="sxs-lookup"><span data-stu-id="64a14-158">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


