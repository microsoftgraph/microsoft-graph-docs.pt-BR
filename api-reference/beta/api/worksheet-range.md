---
title: 'Worksheet: Range'
description: Obtém o objeto de intervalo especificado pelo nome ou endereço.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ec627bcdf1415fd022a25a4234371d2c5b9c6a6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456432"
---
# <a name="worksheet-range"></a><span data-ttu-id="c27e8-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="c27e8-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c27e8-104">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="c27e8-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="c27e8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c27e8-105">Permissions</span></span>
<span data-ttu-id="c27e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c27e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c27e8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c27e8-108">Permission type</span></span>      | <span data-ttu-id="c27e8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c27e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c27e8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c27e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c27e8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c27e8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c27e8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c27e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c27e8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c27e8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c27e8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c27e8-114">Application</span></span> | <span data-ttu-id="c27e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c27e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c27e8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c27e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="c27e8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c27e8-117">Request headers</span></span>
| <span data-ttu-id="c27e8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c27e8-118">Name</span></span>       | <span data-ttu-id="c27e8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c27e8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c27e8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c27e8-120">Authorization</span></span>  | <span data-ttu-id="c27e8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c27e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c27e8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c27e8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c27e8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c27e8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c27e8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c27e8-126">Request body</span></span>
<span data-ttu-id="c27e8-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c27e8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c27e8-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c27e8-128">Parameter</span></span>    | <span data-ttu-id="c27e8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c27e8-129">Type</span></span>   |<span data-ttu-id="c27e8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c27e8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c27e8-131">address</span><span class="sxs-lookup"><span data-stu-id="c27e8-131">address</span></span>|<span data-ttu-id="c27e8-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c27e8-132">string</span></span>|<span data-ttu-id="c27e8-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="c27e8-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c27e8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c27e8-136">Response</span></span>

<span data-ttu-id="c27e8-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c27e8-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c27e8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c27e8-138">Example</span></span>
<span data-ttu-id="c27e8-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c27e8-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c27e8-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c27e8-140">Request</span></span>
<span data-ttu-id="c27e8-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c27e8-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c27e8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c27e8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c27e8-143">C#</span><span class="sxs-lookup"><span data-stu-id="c27e8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c27e8-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="c27e8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c27e8-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c27e8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c27e8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c27e8-146">Response</span></span>
<span data-ttu-id="c27e8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c27e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
