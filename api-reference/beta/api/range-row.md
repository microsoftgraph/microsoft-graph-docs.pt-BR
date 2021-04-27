---
title: 'Range: Row'
description: Obtém uma linha contida no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 83e763e74ed854143035f2893935b61bc0eefc69
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055061"
---
# <a name="range-row"></a><span data-ttu-id="6b888-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="6b888-103">Range: Row</span></span>

<span data-ttu-id="6b888-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b888-105">Obtém uma linha contida no intervalo.</span><span class="sxs-lookup"><span data-stu-id="6b888-105">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b888-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b888-106">Permissions</span></span>
<span data-ttu-id="6b888-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b888-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b888-109">Permission type</span></span>      | <span data-ttu-id="6b888-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b888-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b888-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b888-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b888-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b888-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b888-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b888-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b888-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b888-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b888-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b888-115">Application</span></span> | <span data-ttu-id="6b888-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b888-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b888-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b888-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/Row
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/Row
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Row
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="6b888-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b888-118">Request headers</span></span>
| <span data-ttu-id="6b888-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b888-119">Name</span></span>       | <span data-ttu-id="6b888-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b888-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b888-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b888-121">Authorization</span></span>  | <span data-ttu-id="6b888-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b888-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b888-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6b888-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6b888-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6b888-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b888-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b888-127">Request body</span></span>
<span data-ttu-id="6b888-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b888-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b888-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6b888-129">Parameter</span></span>    | <span data-ttu-id="6b888-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b888-130">Type</span></span>   |<span data-ttu-id="6b888-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b888-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b888-132">row</span><span class="sxs-lookup"><span data-stu-id="6b888-132">row</span></span>|<span data-ttu-id="6b888-133">number</span><span class="sxs-lookup"><span data-stu-id="6b888-133">number</span></span>|<span data-ttu-id="6b888-p104">O número da linha do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="6b888-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="6b888-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b888-136">Response</span></span>

<span data-ttu-id="6b888-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b888-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b888-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b888-138">Example</span></span>
<span data-ttu-id="6b888-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6b888-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b888-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b888-140">Request</span></span>
<span data-ttu-id="6b888-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b888-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="6b888-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b888-142">Response</span></span>
<span data-ttu-id="6b888-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b888-143">Here is an example of the response.</span></span> <span data-ttu-id="6b888-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6b888-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


