---
title: 'Range: Row'
description: Obtém uma linha contida no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 367e7a0642b9da493b0b83d20f368175c0ab7f9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081847"
---
# <a name="range-row"></a><span data-ttu-id="592d0-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="592d0-103">Range: Row</span></span>

<span data-ttu-id="592d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="592d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="592d0-105">Obtém uma linha contida no intervalo.</span><span class="sxs-lookup"><span data-stu-id="592d0-105">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="592d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="592d0-106">Permissions</span></span>
<span data-ttu-id="592d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="592d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="592d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="592d0-109">Permission type</span></span>      | <span data-ttu-id="592d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="592d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="592d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="592d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="592d0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592d0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="592d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="592d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="592d0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592d0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="592d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592d0-115">Application</span></span> | <span data-ttu-id="592d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="592d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="592d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="592d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="592d0-118">Request headers</span></span>
| <span data-ttu-id="592d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="592d0-119">Name</span></span>       | <span data-ttu-id="592d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="592d0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="592d0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="592d0-121">Authorization</span></span>  | <span data-ttu-id="592d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="592d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="592d0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="592d0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="592d0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="592d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="592d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="592d0-127">Request body</span></span>
<span data-ttu-id="592d0-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="592d0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="592d0-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="592d0-129">Parameter</span></span>    | <span data-ttu-id="592d0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="592d0-130">Type</span></span>   |<span data-ttu-id="592d0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="592d0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="592d0-132">row</span><span class="sxs-lookup"><span data-stu-id="592d0-132">row</span></span>|<span data-ttu-id="592d0-133">number</span><span class="sxs-lookup"><span data-stu-id="592d0-133">number</span></span>|<span data-ttu-id="592d0-p104">O número da linha do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="592d0-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="592d0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="592d0-136">Response</span></span>

<span data-ttu-id="592d0-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="592d0-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="592d0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="592d0-138">Example</span></span>
<span data-ttu-id="592d0-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="592d0-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="592d0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="592d0-140">Request</span></span>
<span data-ttu-id="592d0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="592d0-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="592d0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="592d0-142">Response</span></span>
<span data-ttu-id="592d0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="592d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


