---
title: Listar TableCollection
description: Recupere uma lista de objetos de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4d0f9ca75314b4ad0ee4b4f10efdacd3f9c98f66
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637861"
---
# <a name="list-tablecollection"></a><span data-ttu-id="f217f-103">Listar TableCollection</span><span class="sxs-lookup"><span data-stu-id="f217f-103">List TableCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f217f-104">Recupere uma lista de objetos de tabela.</span><span class="sxs-lookup"><span data-stu-id="f217f-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f217f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f217f-105">Permissions</span></span>
<span data-ttu-id="f217f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f217f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f217f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f217f-108">Permission type</span></span>      | <span data-ttu-id="f217f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f217f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f217f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f217f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f217f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f217f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f217f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f217f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f217f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f217f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f217f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f217f-114">Application</span></span> | <span data-ttu-id="f217f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f217f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f217f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f217f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f217f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f217f-117">Optional query parameters</span></span>
<span data-ttu-id="f217f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f217f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f217f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f217f-119">Request headers</span></span>
| <span data-ttu-id="f217f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f217f-120">Name</span></span>      |<span data-ttu-id="f217f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f217f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f217f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f217f-122">Authorization</span></span>  | <span data-ttu-id="f217f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f217f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f217f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f217f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f217f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f217f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f217f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f217f-128">Request body</span></span>
<span data-ttu-id="f217f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f217f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f217f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f217f-130">Response</span></span>

<span data-ttu-id="f217f-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbooktable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f217f-131">If successful, this method returns a `200 OK` response code and collection of [workbookTable](../resources/workbooktable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f217f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f217f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f217f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f217f-133">Request</span></span>
<span data-ttu-id="f217f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f217f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="f217f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f217f-135">Response</span></span>
<span data-ttu-id="f217f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f217f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f217f-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f217f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f217f-140">Basic</span><span class="sxs-lookup"><span data-stu-id="f217f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tablecollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f217f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f217f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tablecollection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
