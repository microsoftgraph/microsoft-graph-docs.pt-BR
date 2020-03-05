---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 40e20c300d43bfc0190374095ef50952f8c9c54a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454775"
---
# <a name="range-column"></a><span data-ttu-id="5d5db-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="5d5db-103">Range: Column</span></span>

<span data-ttu-id="5d5db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5d5db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d5db-105">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="5d5db-105">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d5db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d5db-106">Permissions</span></span>
<span data-ttu-id="5d5db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d5db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d5db-109">Permission type</span></span>      | <span data-ttu-id="5d5db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d5db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d5db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d5db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d5db-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d5db-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d5db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d5db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d5db-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d5db-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d5db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d5db-115">Application</span></span> | <span data-ttu-id="5d5db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d5db-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d5db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d5db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="5d5db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d5db-118">Request headers</span></span>
| <span data-ttu-id="5d5db-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d5db-119">Name</span></span>       | <span data-ttu-id="5d5db-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d5db-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d5db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d5db-121">Authorization</span></span>  | <span data-ttu-id="5d5db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d5db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d5db-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5d5db-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5d5db-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d5db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d5db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d5db-127">Request body</span></span>
<span data-ttu-id="5d5db-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d5db-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d5db-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d5db-129">Parameter</span></span>    | <span data-ttu-id="5d5db-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d5db-130">Type</span></span>   |<span data-ttu-id="5d5db-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d5db-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d5db-132">column</span><span class="sxs-lookup"><span data-stu-id="5d5db-132">column</span></span>|<span data-ttu-id="5d5db-133">number</span><span class="sxs-lookup"><span data-stu-id="5d5db-133">number</span></span>|<span data-ttu-id="5d5db-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5d5db-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5d5db-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d5db-136">Response</span></span>

<span data-ttu-id="5d5db-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d5db-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d5db-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d5db-138">Example</span></span>
<span data-ttu-id="5d5db-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5d5db-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d5db-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d5db-140">Request</span></span>
<span data-ttu-id="5d5db-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d5db-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="5d5db-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d5db-142">Response</span></span>
<span data-ttu-id="5d5db-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d5db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
