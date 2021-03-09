---
title: 'RangeBorderCollection: ItemAt'
description: Obtém um objeto de borda usando seu índice.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 819b5f74981143ed2f784f89f957d66702e81d26
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576950"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="4386e-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="4386e-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="4386e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4386e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4386e-105">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="4386e-105">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="4386e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4386e-106">Permissions</span></span>
<span data-ttu-id="4386e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4386e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4386e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4386e-109">Permission type</span></span>      | <span data-ttu-id="4386e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4386e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4386e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4386e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4386e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4386e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4386e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4386e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4386e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4386e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4386e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4386e-115">Application</span></span> | <span data-ttu-id="4386e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4386e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4386e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4386e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="4386e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4386e-118">Request headers</span></span>
| <span data-ttu-id="4386e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4386e-119">Name</span></span>       | <span data-ttu-id="4386e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4386e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4386e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4386e-121">Authorization</span></span>  | <span data-ttu-id="4386e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4386e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4386e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4386e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4386e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4386e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4386e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4386e-127">Request body</span></span>
<span data-ttu-id="4386e-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4386e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4386e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4386e-129">Parameter</span></span>    | <span data-ttu-id="4386e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4386e-130">Type</span></span>   |<span data-ttu-id="4386e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4386e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4386e-132">index</span><span class="sxs-lookup"><span data-stu-id="4386e-132">index</span></span>|<span data-ttu-id="4386e-133">number</span><span class="sxs-lookup"><span data-stu-id="4386e-133">number</span></span>|<span data-ttu-id="4386e-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="4386e-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="4386e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4386e-136">Response</span></span>

<span data-ttu-id="4386e-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [workbookRangeBorder](../resources/workbookrangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4386e-137">If successful, this method returns `200 OK` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4386e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4386e-138">Example</span></span>
<span data-ttu-id="4386e-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4386e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4386e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4386e-140">Request</span></span>
<span data-ttu-id="4386e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4386e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4386e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4386e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="4386e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4386e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4386e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4386e-144">Response</span></span>
<span data-ttu-id="4386e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4386e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


