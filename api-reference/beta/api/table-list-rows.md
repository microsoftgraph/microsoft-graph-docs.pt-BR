---
title: Listar linhas
description: Recupere uma lista de objetos tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 99bb88587259cfc0deb423df4e41bd0db5601193
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722220"
---
# <a name="list-rows"></a><span data-ttu-id="5ee8b-103">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="5ee8b-103">List rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee8b-104">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ee8b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ee8b-105">Permissions</span></span>
<span data-ttu-id="5ee8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee8b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee8b-108">Permission type</span></span>      | <span data-ttu-id="5ee8b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee8b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ee8b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee8b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ee8b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee8b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ee8b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee8b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee8b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee8b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ee8b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee8b-114">Application</span></span> | <span data-ttu-id="5ee8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ee8b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee8b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ee8b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ee8b-117">Optional query parameters</span></span>
<span data-ttu-id="5ee8b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="5ee8b-119">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="5ee8b-120">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ee8b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8b-121">Request headers</span></span>
| <span data-ttu-id="5ee8b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee8b-122">Name</span></span>      |<span data-ttu-id="5ee8b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee8b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ee8b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee8b-124">Authorization</span></span>  | <span data-ttu-id="5ee8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ee8b-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ee8b-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ee8b-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee8b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8b-130">Request body</span></span>
<span data-ttu-id="5ee8b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee8b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8b-132">Response</span></span>

<span data-ttu-id="5ee8b-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-133">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ee8b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ee8b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ee8b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8b-135">Request</span></span>
<span data-ttu-id="5ee8b-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5ee8b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee8b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ee8b-138">C#</span><span class="sxs-lookup"><span data-stu-id="5ee8b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ee8b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee8b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ee8b-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5ee8b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ee8b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8b-141">Response</span></span>
<span data-ttu-id="5ee8b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="5ee8b-145">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="5ee8b-145">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="5ee8b-146">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="5ee8b-146">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
