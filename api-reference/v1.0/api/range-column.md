---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 21338edb35c8e3e7c060d0f4a03e7e3e77f4e60b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986716"
---
# <a name="range-column"></a><span data-ttu-id="14190-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="14190-103">Range: Column</span></span>

<span data-ttu-id="14190-104">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="14190-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="14190-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="14190-105">Permissions</span></span>
<span data-ttu-id="14190-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14190-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14190-108">Permission type</span></span>      | <span data-ttu-id="14190-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14190-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14190-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14190-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14190-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14190-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14190-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14190-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14190-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14190-113">Not supported.</span></span>    |
|<span data-ttu-id="14190-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14190-114">Application</span></span> | <span data-ttu-id="14190-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14190-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14190-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14190-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="14190-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14190-117">Request headers</span></span>
| <span data-ttu-id="14190-118">Nome</span><span class="sxs-lookup"><span data-stu-id="14190-118">Name</span></span>       | <span data-ttu-id="14190-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="14190-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="14190-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="14190-120">Authorization</span></span>  | <span data-ttu-id="14190-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14190-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14190-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="14190-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="14190-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="14190-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="14190-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="14190-126">Path parameters</span></span>
<span data-ttu-id="14190-127">Forneça o caminho da solicitação, os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="14190-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="14190-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="14190-128">Parameter</span></span>    | <span data-ttu-id="14190-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="14190-129">Type</span></span>   |<span data-ttu-id="14190-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="14190-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14190-131">column</span><span class="sxs-lookup"><span data-stu-id="14190-131">column</span></span>|<span data-ttu-id="14190-132">Int32</span><span class="sxs-lookup"><span data-stu-id="14190-132">Int32</span></span>|<span data-ttu-id="14190-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="14190-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="14190-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="14190-135">Response</span></span>

<span data-ttu-id="14190-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14190-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14190-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14190-137">Example</span></span>
<span data-ttu-id="14190-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="14190-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="14190-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14190-139">Request</span></span>
<span data-ttu-id="14190-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14190-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="14190-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="14190-141">Response</span></span>
<span data-ttu-id="14190-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14190-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
