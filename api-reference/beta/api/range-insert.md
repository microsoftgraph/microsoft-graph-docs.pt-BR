---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1b62bdc66f5070c47a22074f60b5ae0f0df4e590
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611126"
---
# <a name="range-insert"></a><span data-ttu-id="f8a7c-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="f8a7c-104">Range: insert</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8a7c-p102">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8a7c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8a7c-107">Permissions</span></span>
<span data-ttu-id="f8a7c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8a7c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8a7c-110">Permission type</span></span>      | <span data-ttu-id="f8a7c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8a7c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8a7c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8a7c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f8a7c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8a7c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8a7c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8a7c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8a7c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8a7c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8a7c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8a7c-116">Application</span></span> | <span data-ttu-id="f8a7c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8a7c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8a7c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="f8a7c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a7c-119">Request headers</span></span>
| <span data-ttu-id="f8a7c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f8a7c-120">Name</span></span>       | <span data-ttu-id="f8a7c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8a7c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8a7c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8a7c-122">Authorization</span></span>  | <span data-ttu-id="f8a7c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8a7c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f8a7c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8a7c-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8a7c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a7c-128">Request body</span></span>
<span data-ttu-id="f8a7c-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8a7c-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f8a7c-130">Parameter</span></span>    | <span data-ttu-id="f8a7c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8a7c-131">Type</span></span>   |<span data-ttu-id="f8a7c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8a7c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8a7c-133">shift</span><span class="sxs-lookup"><span data-stu-id="f8a7c-133">shift</span></span>|<span data-ttu-id="f8a7c-134">string</span><span class="sxs-lookup"><span data-stu-id="f8a7c-134">string</span></span>|<span data-ttu-id="f8a7c-p106">Especifica como deslocar as células.  Os valores possíveis são: `Down` e `Right`.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="f8a7c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8a7c-137">Response</span></span>

<span data-ttu-id="f8a7c-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8a7c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8a7c-139">Example</span></span>
<span data-ttu-id="f8a7c-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8a7c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8a7c-141">Request</span></span>
<span data-ttu-id="f8a7c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="f8a7c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8a7c-143">Response</span></span>
<span data-ttu-id="f8a7c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8a7c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8a7c-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f8a7c-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8a7c-148">Basic</span><span class="sxs-lookup"><span data-stu-id="f8a7c-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_insert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8a7c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8a7c-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_insert-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
