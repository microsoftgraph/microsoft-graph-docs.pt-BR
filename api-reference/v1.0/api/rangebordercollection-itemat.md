---
title: 'RangeBorderCollection: ItemAt'
description: Obtém um objeto de borda usando seu índice.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 074314027e4c62c172245056be18a04078c6dfcb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582343"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="55a39-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="55a39-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="55a39-104">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="55a39-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="55a39-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55a39-105">Permissions</span></span>
<span data-ttu-id="55a39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55a39-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55a39-108">Permission type</span></span>      | <span data-ttu-id="55a39-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55a39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55a39-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55a39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55a39-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55a39-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55a39-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55a39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55a39-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a39-113">Not supported.</span></span>    |
|<span data-ttu-id="55a39-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55a39-114">Application</span></span> | <span data-ttu-id="55a39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a39-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55a39-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55a39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="55a39-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55a39-117">Request headers</span></span>
| <span data-ttu-id="55a39-118">Nome</span><span class="sxs-lookup"><span data-stu-id="55a39-118">Name</span></span>       | <span data-ttu-id="55a39-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a39-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="55a39-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="55a39-120">Authorization</span></span>  | <span data-ttu-id="55a39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55a39-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55a39-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="55a39-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="55a39-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="55a39-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55a39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55a39-126">Request body</span></span>
<span data-ttu-id="55a39-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55a39-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55a39-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55a39-128">Parameter</span></span>    | <span data-ttu-id="55a39-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="55a39-129">Type</span></span>   |<span data-ttu-id="55a39-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a39-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55a39-131">índice</span><span class="sxs-lookup"><span data-stu-id="55a39-131">index</span></span>|<span data-ttu-id="55a39-132">Int32</span><span class="sxs-lookup"><span data-stu-id="55a39-132">Int32</span></span>|<span data-ttu-id="55a39-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="55a39-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="55a39-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a39-135">Response</span></span>

<span data-ttu-id="55a39-136">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55a39-136">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55a39-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55a39-137">Example</span></span>
<span data-ttu-id="55a39-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="55a39-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55a39-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55a39-139">Request</span></span>
<span data-ttu-id="55a39-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55a39-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="55a39-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a39-141">Response</span></span>
<span data-ttu-id="55a39-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55a39-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
