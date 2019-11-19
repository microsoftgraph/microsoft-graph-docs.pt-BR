---
title: 'pesquisa: consulta'
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b5da13640d2c62eb8258ca1a154ddcb8c2e1b353
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703704"
---
# <a name="search-query"></a><span data-ttu-id="2ea96-103">pesquisa: consulta</span><span class="sxs-lookup"><span data-stu-id="2ea96-103">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ea96-104">Executa a consulta especificada no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ea96-104">Executes the query specified in the request body.</span></span> <span data-ttu-id="2ea96-105">Os resultados da pesquisa são fornecidos na resposta.</span><span class="sxs-lookup"><span data-stu-id="2ea96-105">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2ea96-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ea96-106">Permissions</span></span>

<span data-ttu-id="2ea96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ea96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ea96-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ea96-109">Permission type</span></span>                        | <span data-ttu-id="2ea96-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ea96-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ea96-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ea96-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ea96-112">Mail. Read, files. Read. All, Calendars. Read, ExternalItem. Read. All</span><span class="sxs-lookup"><span data-stu-id="2ea96-112">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="2ea96-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ea96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ea96-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ea96-114">Not supported.</span></span> |
| <span data-ttu-id="2ea96-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ea96-115">Application</span></span>                            | <span data-ttu-id="2ea96-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ea96-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ea96-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea96-117">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="2ea96-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea96-118">Request headers</span></span>

| <span data-ttu-id="2ea96-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ea96-119">Name</span></span>          | <span data-ttu-id="2ea96-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ea96-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ea96-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ea96-121">Authorization</span></span> | <span data-ttu-id="2ea96-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2ea96-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ea96-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea96-123">Request body</span></span>

<span data-ttu-id="2ea96-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ea96-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ea96-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ea96-125">Parameter</span></span>    | <span data-ttu-id="2ea96-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ea96-126">Type</span></span>        | <span data-ttu-id="2ea96-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ea96-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ea96-128">Quest</span><span class="sxs-lookup"><span data-stu-id="2ea96-128">requests</span></span>|<span data-ttu-id="2ea96-129">coleção [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2ea96-129">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="2ea96-130">A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta formatado em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="2ea96-130">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="2ea96-131">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="2ea96-131">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="2ea96-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ea96-132">Response</span></span>

<span data-ttu-id="2ea96-133">Se bem-sucedido, este método retorna `HTTP 200 OK` o código de resposta e um objeto da coleção [searchResponse](../resources/searchresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ea96-133">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="2ea96-134">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="2ea96-134">Common use cases</span></span>

- <span data-ttu-id="2ea96-135">[Mensagens de email](/graph/search-concept-messages) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2ea96-135">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="2ea96-136">[Eventos de calendário](/graph/search-concept-events) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2ea96-136">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="2ea96-137">[Arquivos](/graph/search-concept-files) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2ea96-137">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="2ea96-138">Dados [de tipos personalizados de pesquisa (conectores)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="2ea96-138">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="2ea96-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ea96-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ea96-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea96-140">Request</span></span>

<span data-ttu-id="2ea96-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ea96-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ea96-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea96-142">HTTP</span></span>](#tab/http)
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
        "microsoft.graph.externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "query_string": {
          "query": "contoso product"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ea96-143">C#</span><span class="sxs-lookup"><span data-stu-id="2ea96-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ea96-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ea96-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ea96-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ea96-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ea96-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ea96-146">Response</span></span>

<span data-ttu-id="2ea96-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ea96-147">The following is an example of the response.</span></span>

> <span data-ttu-id="2ea96-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ea96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
              "_id": "1",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "_summary-value",
              "_source": "The source field will contain the underlying graph entity part of the response"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
