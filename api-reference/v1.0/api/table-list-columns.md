---
title: Listar colunas
description: Recupere uma lista de objetos tablecolumn.
ms.openlocfilehash: dcaaaa92bf8d97119233b35f39fd98b2589be129
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004381"
---
# <a name="list-columns"></a><span data-ttu-id="c2926-103">Listar colunas</span><span class="sxs-lookup"><span data-stu-id="c2926-103">List columns</span></span>

<span data-ttu-id="c2926-104">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="c2926-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2926-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2926-105">Permissions</span></span>
<span data-ttu-id="c2926-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2926-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2926-108">Permission type</span></span>      | <span data-ttu-id="c2926-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2926-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2926-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2926-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2926-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2926-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2926-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2926-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2926-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2926-113">Not supported.</span></span>    |
|<span data-ttu-id="c2926-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2926-114">Application</span></span> | <span data-ttu-id="c2926-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2926-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2926-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2926-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2926-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2926-117">Optional query parameters</span></span>
<span data-ttu-id="c2926-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2926-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="c2926-119">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="c2926-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="c2926-120">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="c2926-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2926-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2926-121">Request headers</span></span>
| <span data-ttu-id="c2926-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c2926-122">Name</span></span>      |<span data-ttu-id="c2926-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2926-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2926-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2926-124">Authorization</span></span>  | <span data-ttu-id="c2926-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2926-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2926-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c2926-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="c2926-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c2926-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2926-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2926-130">Request body</span></span>
<span data-ttu-id="c2926-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2926-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2926-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2926-132">Response</span></span>

<span data-ttu-id="c2926-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2926-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2926-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2926-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2926-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2926-135">Request</span></span>
<span data-ttu-id="c2926-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2926-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="c2926-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2926-137">Response</span></span>
<span data-ttu-id="c2926-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2926-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="c2926-141">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de colunas.</span><span class="sxs-lookup"><span data-stu-id="c2926-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="c2926-142">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="c2926-142">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->