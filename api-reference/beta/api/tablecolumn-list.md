---
title: Listar TableColumnCollection
description: Recupere uma lista de objetos tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 63d40091eae8b6053be4e0af48f9cc2e5e7617a6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270956"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="31b2a-103">Listar TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="31b2a-103">List TableColumnCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b2a-104">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="31b2a-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="31b2a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="31b2a-105">Permissions</span></span>
<span data-ttu-id="31b2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31b2a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31b2a-108">Permission type</span></span>      | <span data-ttu-id="31b2a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31b2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31b2a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31b2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31b2a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31b2a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31b2a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31b2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b2a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31b2a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31b2a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31b2a-114">Application</span></span> | <span data-ttu-id="31b2a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31b2a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31b2a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31b2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31b2a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31b2a-117">Optional query parameters</span></span>
<span data-ttu-id="31b2a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="31b2a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31b2a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31b2a-119">Request headers</span></span>
| <span data-ttu-id="31b2a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="31b2a-120">Name</span></span>      |<span data-ttu-id="31b2a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="31b2a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31b2a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31b2a-122">Authorization</span></span>  | <span data-ttu-id="31b2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31b2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31b2a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="31b2a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="31b2a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="31b2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31b2a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31b2a-128">Request body</span></span>
<span data-ttu-id="31b2a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31b2a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31b2a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="31b2a-130">Response</span></span>

<span data-ttu-id="31b2a-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31b2a-131">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31b2a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31b2a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31b2a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31b2a-133">Request</span></span>
<span data-ttu-id="31b2a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31b2a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="31b2a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="31b2a-135">Response</span></span>
<span data-ttu-id="31b2a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31b2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="31b2a-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="31b2a-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="31b2a-140">C#</span><span class="sxs-lookup"><span data-stu-id="31b2a-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tablecolumncollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31b2a-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="31b2a-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tablecolumncollection-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="31b2a-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="31b2a-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tablecolumncollection-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablecolumn-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumn-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
