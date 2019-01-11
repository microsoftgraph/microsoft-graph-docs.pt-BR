---
title: Listar linhas
description: Recupere uma lista de objetos tablerow.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 9e93b9a8469586d0105f0c170a4ee9f8ebe65ff9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871985"
---
# <a name="list-rows"></a><span data-ttu-id="56660-103">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="56660-103">List rows</span></span>

<span data-ttu-id="56660-104">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="56660-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="56660-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56660-105">Permissions</span></span>
<span data-ttu-id="56660-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56660-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56660-108">Permission type</span></span>      | <span data-ttu-id="56660-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56660-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56660-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56660-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56660-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56660-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56660-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56660-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56660-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56660-113">Not supported.</span></span>    |
|<span data-ttu-id="56660-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56660-114">Application</span></span> | <span data-ttu-id="56660-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56660-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56660-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56660-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56660-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56660-117">Optional query parameters</span></span>
<span data-ttu-id="56660-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56660-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="56660-119">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="56660-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="56660-120">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="56660-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56660-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56660-121">Request headers</span></span>
| <span data-ttu-id="56660-122">Nome</span><span class="sxs-lookup"><span data-stu-id="56660-122">Name</span></span>      |<span data-ttu-id="56660-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="56660-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56660-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="56660-124">Authorization</span></span>  | <span data-ttu-id="56660-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56660-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56660-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56660-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="56660-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="56660-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56660-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56660-130">Request body</span></span>
<span data-ttu-id="56660-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56660-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56660-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="56660-132">Response</span></span>

<span data-ttu-id="56660-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56660-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56660-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56660-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56660-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56660-135">Request</span></span>
<span data-ttu-id="56660-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56660-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="56660-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="56660-137">Response</span></span>
<span data-ttu-id="56660-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56660-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
> <span data-ttu-id="56660-141">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="56660-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="56660-142">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="56660-142">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
