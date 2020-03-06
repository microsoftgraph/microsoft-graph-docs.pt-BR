---
title: 'TableColumn: HeaderRowRange'
description: Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9ae6271ee4d742adf7daa7e4ecdd221a020db318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509581"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="b5806-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="b5806-103">TableColumn: HeaderRowRange</span></span>

<span data-ttu-id="b5806-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5806-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5806-105">Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.</span><span class="sxs-lookup"><span data-stu-id="b5806-105">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5806-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5806-106">Permissions</span></span>
<span data-ttu-id="b5806-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5806-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5806-109">Permission type</span></span>      | <span data-ttu-id="b5806-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5806-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5806-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5806-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5806-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5806-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5806-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5806-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5806-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5806-114">Not supported.</span></span>    |
|<span data-ttu-id="b5806-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5806-115">Application</span></span> | <span data-ttu-id="b5806-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5806-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5806-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5806-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="b5806-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5806-118">Request headers</span></span>
| <span data-ttu-id="b5806-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b5806-119">Name</span></span>       | <span data-ttu-id="b5806-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5806-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5806-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5806-121">Authorization</span></span>  | <span data-ttu-id="b5806-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5806-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5806-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b5806-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b5806-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b5806-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5806-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5806-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b5806-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5806-128">Response</span></span>

<span data-ttu-id="b5806-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5806-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5806-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5806-130">Example</span></span>
<span data-ttu-id="b5806-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b5806-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b5806-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5806-132">Request</span></span>
<span data-ttu-id="b5806-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5806-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5806-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5806-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange
```
# <a name="c"></a>[<span data-ttu-id="b5806-135">C#</span><span class="sxs-lookup"><span data-stu-id="b5806-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5806-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5806-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5806-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5806-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5806-138">Java</span><span class="sxs-lookup"><span data-stu-id="b5806-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-headerrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5806-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5806-139">Response</span></span>
<span data-ttu-id="b5806-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5806-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
