---
title: 'pesquisa: consulta'
description: Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff5d67dc749ce60797ec6c6387d79795718409c5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868846"
---
# <a name="search-query"></a><span data-ttu-id="112d5-104">pesquisa: consulta</span><span class="sxs-lookup"><span data-stu-id="112d5-104">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="112d5-105">Executa a consulta especificada no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="112d5-105">Runs the query specified in the request body.</span></span> <span data-ttu-id="112d5-106">Os resultados da pesquisa são fornecidos na resposta.</span><span class="sxs-lookup"><span data-stu-id="112d5-106">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="112d5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="112d5-107">Permissions</span></span>

<span data-ttu-id="112d5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="112d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="112d5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="112d5-110">Permission type</span></span>                        | <span data-ttu-id="112d5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="112d5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="112d5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="112d5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="112d5-113">Mail. Read, files. Read. All, Calendars. Read, ExternalItem. Read. All</span><span class="sxs-lookup"><span data-stu-id="112d5-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="112d5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="112d5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="112d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="112d5-115">Not supported.</span></span> |
| <span data-ttu-id="112d5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="112d5-116">Application</span></span>                            | <span data-ttu-id="112d5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="112d5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="112d5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="112d5-118">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="112d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="112d5-119">Request headers</span></span>

| <span data-ttu-id="112d5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="112d5-120">Name</span></span>          | <span data-ttu-id="112d5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="112d5-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="112d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="112d5-122">Authorization</span></span> | <span data-ttu-id="112d5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="112d5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="112d5-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="112d5-125">Content-type</span></span> | <span data-ttu-id="112d5-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="112d5-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="112d5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="112d5-128">Request body</span></span>

<span data-ttu-id="112d5-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="112d5-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="112d5-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="112d5-130">Parameter</span></span>    | <span data-ttu-id="112d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="112d5-131">Type</span></span>        | <span data-ttu-id="112d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="112d5-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="112d5-133">Quest</span><span class="sxs-lookup"><span data-stu-id="112d5-133">requests</span></span>|<span data-ttu-id="112d5-134">coleção [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="112d5-134">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="112d5-135">A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta formatado em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="112d5-135">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="112d5-136">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="112d5-136">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="112d5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="112d5-137">Response</span></span>

<span data-ttu-id="112d5-138">Se bem-sucedido, este método retorna `HTTP 200 OK` o código de resposta e um objeto da coleção [searchResponse](../resources/searchresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="112d5-138">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="112d5-139">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="112d5-139">Common use cases</span></span>

- <span data-ttu-id="112d5-140">[Mensagens de email](/graph/search-concept-messages) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="112d5-140">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="112d5-141">[Eventos de calendário](/graph/search-concept-events) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="112d5-141">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="112d5-142">[Arquivos](/graph/search-concept-files) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="112d5-142">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="112d5-143">Dados [de tipos personalizados de pesquisa (conectores)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="112d5-143">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="112d5-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="112d5-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="112d5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="112d5-145">Request</span></span>

<span data-ttu-id="112d5-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="112d5-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="112d5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="112d5-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="112d5-148">C#</span><span class="sxs-lookup"><span data-stu-id="112d5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="112d5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="112d5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="112d5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="112d5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="112d5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="112d5-151">Response</span></span>

<span data-ttu-id="112d5-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="112d5-152">The following is an example of the response.</span></span>

> <span data-ttu-id="112d5-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="112d5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
