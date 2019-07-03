---
title: 'Table: HeaderRowRange'
description: Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1730e4d233a7017c9b5da182c1151341433b7510
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458056"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="5b79a-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="5b79a-103">Table: HeaderRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b79a-104">Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.</span><span class="sxs-lookup"><span data-stu-id="5b79a-104">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b79a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b79a-105">Permissions</span></span>
<span data-ttu-id="5b79a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b79a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b79a-108">Permission type</span></span>      | <span data-ttu-id="5b79a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b79a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b79a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b79a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b79a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b79a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b79a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b79a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b79a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b79a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b79a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b79a-114">Application</span></span> | <span data-ttu-id="5b79a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b79a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b79a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b79a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="5b79a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b79a-117">Request headers</span></span>
| <span data-ttu-id="5b79a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5b79a-118">Name</span></span>       | <span data-ttu-id="5b79a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b79a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5b79a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b79a-120">Authorization</span></span>  | <span data-ttu-id="5b79a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b79a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b79a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5b79a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b79a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5b79a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b79a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b79a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5b79a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b79a-127">Response</span></span>

<span data-ttu-id="5b79a-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b79a-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b79a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b79a-129">Example</span></span>
<span data-ttu-id="5b79a-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5b79a-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b79a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b79a-131">Request</span></span>
<span data-ttu-id="5b79a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b79a-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b79a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b79a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b79a-134">C#</span><span class="sxs-lookup"><span data-stu-id="5b79a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b79a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b79a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b79a-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5b79a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5b79a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b79a-137">Response</span></span>
<span data-ttu-id="5b79a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b79a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
