---
title: Listar nomes
description: 'Recupere uma lista de itens nomeados associados à planilha. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f11bdbc850108d284329d36fff901323b596aa38
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636888"
---
# <a name="list-names"></a><span data-ttu-id="6c344-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="6c344-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c344-104">Recupere uma lista de itens nomeados associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="6c344-104">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="6c344-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c344-105">Permissions</span></span>
<span data-ttu-id="6c344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c344-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c344-108">Permission type</span></span>      | <span data-ttu-id="6c344-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c344-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c344-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c344-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c344-111">Files. Read, files. ReadWrite, sites. Read. All</span><span class="sxs-lookup"><span data-stu-id="6c344-111">Files.Read, Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="6c344-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c344-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c344-113">Files. Read, files. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c344-113">Files.Read, Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c344-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c344-114">Application</span></span> | <span data-ttu-id="6c344-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c344-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c344-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c344-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c344-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c344-117">Optional query parameters</span></span>
<span data-ttu-id="6c344-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c344-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c344-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c344-119">Request headers</span></span>
| <span data-ttu-id="6c344-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6c344-120">Name</span></span>      |<span data-ttu-id="6c344-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c344-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c344-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c344-122">Authorization</span></span>  | <span data-ttu-id="6c344-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c344-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c344-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c344-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c344-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c344-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c344-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c344-128">Request body</span></span>
<span data-ttu-id="6c344-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c344-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c344-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c344-130">Response</span></span>

<span data-ttu-id="6c344-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c344-131">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c344-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c344-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c344-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c344-133">Request</span></span>
<span data-ttu-id="6c344-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c344-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="6c344-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c344-135">Response</span></span>
<span data-ttu-id="6c344-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c344-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c344-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6c344-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c344-140">Basic</span><span class="sxs-lookup"><span data-stu-id="6c344-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tables-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c344-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c344-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tables-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-list-names.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheet-list-names.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
