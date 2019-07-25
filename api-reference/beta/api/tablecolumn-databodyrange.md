---
title: 'TableColumn: DataBodyRange'
description: Obtém o objeto de intervalo associado ao corpo de dados da coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09f7107d3407b06f8aa85196948fe735e03769fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868710"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="34d89-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="34d89-103">TableColumn: DataBodyRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34d89-104">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="34d89-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="34d89-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34d89-105">Permissions</span></span>
<span data-ttu-id="34d89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34d89-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34d89-108">Permission type</span></span>      | <span data-ttu-id="34d89-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34d89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34d89-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34d89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34d89-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34d89-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34d89-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34d89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34d89-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34d89-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34d89-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34d89-114">Application</span></span> | <span data-ttu-id="34d89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34d89-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34d89-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34d89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="34d89-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34d89-117">Request headers</span></span>
| <span data-ttu-id="34d89-118">Nome</span><span class="sxs-lookup"><span data-stu-id="34d89-118">Name</span></span>       | <span data-ttu-id="34d89-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="34d89-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34d89-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="34d89-120">Authorization</span></span>  | <span data-ttu-id="34d89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34d89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34d89-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34d89-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="34d89-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="34d89-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34d89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34d89-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="34d89-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="34d89-127">Response</span></span>

<span data-ttu-id="34d89-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34d89-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34d89-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34d89-129">Example</span></span>
<span data-ttu-id="34d89-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="34d89-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34d89-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34d89-131">Request</span></span>
<span data-ttu-id="34d89-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34d89-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34d89-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="34d89-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_databodyrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34d89-134">C#</span><span class="sxs-lookup"><span data-stu-id="34d89-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34d89-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="34d89-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34d89-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="34d89-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34d89-137">Java</span><span class="sxs-lookup"><span data-stu-id="34d89-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34d89-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="34d89-138">Response</span></span>
<span data-ttu-id="34d89-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34d89-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
