---
title: 'RangeBorderCollection: ItemAt'
description: Obtém um objeto de borda usando seu índice.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 23ca167b69df2a1c07d2409fd689094e47999e6b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275268"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="66d42-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="66d42-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="66d42-104">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="66d42-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="66d42-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="66d42-105">Permissions</span></span>
<span data-ttu-id="66d42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d42-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d42-108">Permission type</span></span>      | <span data-ttu-id="66d42-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66d42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d42-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66d42-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66d42-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66d42-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d42-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d42-113">Not supported.</span></span>    |
|<span data-ttu-id="66d42-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d42-114">Application</span></span> | <span data-ttu-id="66d42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d42-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="66d42-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d42-117">Request headers</span></span>
| <span data-ttu-id="66d42-118">Nome</span><span class="sxs-lookup"><span data-stu-id="66d42-118">Name</span></span>       | <span data-ttu-id="66d42-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d42-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66d42-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d42-120">Authorization</span></span>  | <span data-ttu-id="66d42-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66d42-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66d42-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66d42-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="66d42-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="66d42-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d42-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d42-126">Request body</span></span>
<span data-ttu-id="66d42-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d42-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66d42-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66d42-128">Parameter</span></span>    | <span data-ttu-id="66d42-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d42-129">Type</span></span>   |<span data-ttu-id="66d42-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d42-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66d42-131">índice</span><span class="sxs-lookup"><span data-stu-id="66d42-131">index</span></span>|<span data-ttu-id="66d42-132">Int32</span><span class="sxs-lookup"><span data-stu-id="66d42-132">Int32</span></span>|<span data-ttu-id="66d42-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="66d42-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="66d42-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d42-135">Response</span></span>

<span data-ttu-id="66d42-136">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d42-136">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d42-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66d42-137">Example</span></span>
<span data-ttu-id="66d42-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="66d42-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66d42-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d42-139">Request</span></span>
<span data-ttu-id="66d42-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d42-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="66d42-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d42-141">Response</span></span>
<span data-ttu-id="66d42-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66d42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66d42-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="66d42-145">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66d42-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="66d42-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangebordercollection_itemat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="66d42-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="66d42-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangebordercollection_itemat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangebordercollection-itemat.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangebordercollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
