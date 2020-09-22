---
title: 'TableColumn: DataBodyRange'
description: Obtém o objeto de intervalo associado ao corpo de dados da coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d33ff0efb32a8a6fd5ce70def4ae9ce736033630
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091989"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="4f0af-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="4f0af-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="4f0af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f0af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f0af-105">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="4f0af-105">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f0af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f0af-106">Permissions</span></span>
<span data-ttu-id="4f0af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f0af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f0af-109">Permission type</span></span>      | <span data-ttu-id="4f0af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f0af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f0af-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f0af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f0af-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f0af-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f0af-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f0af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f0af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f0af-114">Not supported.</span></span>    |
|<span data-ttu-id="4f0af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f0af-115">Application</span></span> | <span data-ttu-id="4f0af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f0af-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f0af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f0af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="4f0af-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f0af-118">Request headers</span></span>
| <span data-ttu-id="4f0af-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4f0af-119">Name</span></span>       | <span data-ttu-id="4f0af-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f0af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f0af-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f0af-121">Authorization</span></span>  | <span data-ttu-id="4f0af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f0af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f0af-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f0af-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f0af-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4f0af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f0af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f0af-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4f0af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f0af-128">Response</span></span>

<span data-ttu-id="4f0af-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f0af-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f0af-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f0af-130">Example</span></span>
<span data-ttu-id="4f0af-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4f0af-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f0af-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f0af-132">Request</span></span>
<span data-ttu-id="4f0af-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f0af-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f0af-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f0af-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="4f0af-135">C#</span><span class="sxs-lookup"><span data-stu-id="4f0af-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f0af-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f0af-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f0af-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f0af-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f0af-138">Java</span><span class="sxs-lookup"><span data-stu-id="4f0af-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f0af-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f0af-139">Response</span></span>
<span data-ttu-id="4f0af-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f0af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

