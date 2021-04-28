---
title: Listar colunas
description: Recupere uma lista de objetos tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3c6e195338746aab2f2a33293481bb40821977a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054403"
---
# <a name="list-columns"></a><span data-ttu-id="49e58-103">Listar colunas</span><span class="sxs-lookup"><span data-stu-id="49e58-103">List columns</span></span>

<span data-ttu-id="49e58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49e58-105">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="49e58-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="49e58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49e58-106">Permissions</span></span>
<span data-ttu-id="49e58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49e58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49e58-109">Permission type</span></span>      | <span data-ttu-id="49e58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49e58-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49e58-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49e58-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49e58-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49e58-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49e58-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49e58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49e58-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49e58-114">Not supported.</span></span>    |
|<span data-ttu-id="49e58-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49e58-115">Application</span></span> | <span data-ttu-id="49e58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49e58-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49e58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49e58-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49e58-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49e58-118">Optional query parameters</span></span>
<span data-ttu-id="49e58-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49e58-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>  <span data-ttu-id="49e58-120">Para resultados confiáveis, use os parâmetros de consulta [$top](/graph/query-parameters#top) e [$skip](/graph/query-parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="49e58-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="49e58-121">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="49e58-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49e58-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49e58-122">Request headers</span></span>
| <span data-ttu-id="49e58-123">Nome</span><span class="sxs-lookup"><span data-stu-id="49e58-123">Name</span></span>      |<span data-ttu-id="49e58-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="49e58-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49e58-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="49e58-125">Authorization</span></span>  | <span data-ttu-id="49e58-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49e58-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49e58-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49e58-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="49e58-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="49e58-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e58-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49e58-131">Request body</span></span>
<span data-ttu-id="49e58-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49e58-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49e58-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="49e58-133">Response</span></span>

<span data-ttu-id="49e58-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [WorkbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49e58-134">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49e58-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49e58-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49e58-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49e58-136">Request</span></span>
<span data-ttu-id="49e58-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49e58-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49e58-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e58-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="49e58-139">C#</span><span class="sxs-lookup"><span data-stu-id="49e58-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49e58-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e58-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49e58-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e58-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49e58-142">Java</span><span class="sxs-lookup"><span data-stu-id="49e58-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49e58-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="49e58-143">Response</span></span>
<span data-ttu-id="49e58-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49e58-144">Here is an example of the response.</span></span> <span data-ttu-id="49e58-145">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="49e58-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="49e58-146">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](/graph/query-parameters#top) e [$skip](/graph/query-parameters#skip-parameter) para navegar por um grande número de colunas.</span><span class="sxs-lookup"><span data-stu-id="49e58-146">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="49e58-147">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="49e58-147">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
