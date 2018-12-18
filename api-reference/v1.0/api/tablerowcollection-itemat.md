---
title: 'TableRowCollection: ItemAt'
description: Obtém uma linha com base em sua posição na coleção.
author: lumine2008
ms.openlocfilehash: 653f6154b36036f851ffc39d32e2e551b810dbfd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346813"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="17b56-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="17b56-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="17b56-104">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="17b56-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="17b56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17b56-105">Permissions</span></span>
<span data-ttu-id="17b56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b56-108">Permission type</span></span>      | <span data-ttu-id="17b56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17b56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17b56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17b56-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17b56-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17b56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17b56-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b56-113">Not supported.</span></span>    |
|<span data-ttu-id="17b56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17b56-114">Application</span></span> | <span data-ttu-id="17b56-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="17b56-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b56-117">Request headers</span></span>
| <span data-ttu-id="17b56-118">Nome</span><span class="sxs-lookup"><span data-stu-id="17b56-118">Name</span></span>       | <span data-ttu-id="17b56-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b56-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="17b56-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b56-120">Authorization</span></span>  | <span data-ttu-id="17b56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17b56-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="17b56-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="17b56-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="17b56-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b56-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b56-126">Request body</span></span>
<span data-ttu-id="17b56-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b56-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="17b56-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17b56-128">Parameter</span></span>    | <span data-ttu-id="17b56-129">Type</span><span class="sxs-lookup"><span data-stu-id="17b56-129">Type</span></span>   |<span data-ttu-id="17b56-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b56-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17b56-131">índice</span><span class="sxs-lookup"><span data-stu-id="17b56-131">index</span></span>|<span data-ttu-id="17b56-132">Int32</span><span class="sxs-lookup"><span data-stu-id="17b56-132">Int32</span></span>|<span data-ttu-id="17b56-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="17b56-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="17b56-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b56-135">Response</span></span>

<span data-ttu-id="17b56-136">Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b56-136">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b56-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17b56-137">Example</span></span>
<span data-ttu-id="17b56-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="17b56-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="17b56-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b56-139">Request</span></span>
<span data-ttu-id="17b56-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17b56-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerowcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 4
}
```

##### <a name="response"></a><span data-ttu-id="17b56-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b56-141">Response</span></span>
<span data-ttu-id="17b56-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17b56-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->