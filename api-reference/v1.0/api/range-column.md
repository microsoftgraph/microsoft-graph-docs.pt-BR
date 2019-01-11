---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5966e8429d2a0406df3b6774db673d286cc4c8b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870893"
---
# <a name="range-column"></a><span data-ttu-id="0edf0-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="0edf0-103">Range: Column</span></span>

<span data-ttu-id="0edf0-104">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="0edf0-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0edf0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0edf0-105">Permissions</span></span>
<span data-ttu-id="0edf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0edf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0edf0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0edf0-108">Permission type</span></span>      | <span data-ttu-id="0edf0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0edf0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0edf0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0edf0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0edf0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0edf0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0edf0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0edf0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0edf0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0edf0-113">Not supported.</span></span>    |
|<span data-ttu-id="0edf0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0edf0-114">Application</span></span> | <span data-ttu-id="0edf0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0edf0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0edf0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0edf0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="0edf0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0edf0-117">Request headers</span></span>
| <span data-ttu-id="0edf0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0edf0-118">Name</span></span>       | <span data-ttu-id="0edf0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0edf0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0edf0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0edf0-120">Authorization</span></span>  | <span data-ttu-id="0edf0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0edf0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0edf0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0edf0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0edf0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0edf0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="0edf0-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="0edf0-126">Path parameters</span></span>
<span data-ttu-id="0edf0-127">Forneça o caminho da solicitação, os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0edf0-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="0edf0-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0edf0-128">Parameter</span></span>    | <span data-ttu-id="0edf0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0edf0-129">Type</span></span>   |<span data-ttu-id="0edf0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0edf0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0edf0-131">column</span><span class="sxs-lookup"><span data-stu-id="0edf0-131">column</span></span>|<span data-ttu-id="0edf0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0edf0-132">Int32</span></span>|<span data-ttu-id="0edf0-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="0edf0-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0edf0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0edf0-135">Response</span></span>

<span data-ttu-id="0edf0-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0edf0-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0edf0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0edf0-137">Example</span></span>
<span data-ttu-id="0edf0-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0edf0-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0edf0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0edf0-139">Request</span></span>
<span data-ttu-id="0edf0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0edf0-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="0edf0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0edf0-141">Response</span></span>
<span data-ttu-id="0edf0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0edf0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
