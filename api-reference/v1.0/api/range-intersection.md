---
title: 'Range: Intersection'
description: Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 309d2a8935e796ea4897ffbdebb6737f6faee98e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039080"
---
# <a name="range-intersection"></a><span data-ttu-id="d4095-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="d4095-103">Range: Intersection</span></span>

<span data-ttu-id="d4095-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4095-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4095-105">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="d4095-105">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4095-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4095-106">Permissions</span></span>
<span data-ttu-id="d4095-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4095-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4095-109">Permission type</span></span>      | <span data-ttu-id="d4095-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4095-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4095-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4095-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4095-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4095-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d4095-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4095-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4095-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4095-114">Not supported.</span></span>    |
|<span data-ttu-id="d4095-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4095-115">Application</span></span> | <span data-ttu-id="d4095-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4095-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4095-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4095-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/intersection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="d4095-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4095-118">Request headers</span></span>
| <span data-ttu-id="d4095-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d4095-119">Name</span></span>       | <span data-ttu-id="d4095-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4095-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4095-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4095-121">Authorization</span></span>  | <span data-ttu-id="d4095-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4095-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4095-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d4095-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d4095-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d4095-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4095-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4095-127">Request body</span></span>
<span data-ttu-id="d4095-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4095-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4095-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4095-129">Parameter</span></span>    | <span data-ttu-id="d4095-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4095-130">Type</span></span>   |<span data-ttu-id="d4095-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4095-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4095-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="d4095-132">anotherRange</span></span>|<span data-ttu-id="d4095-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4095-133">string</span></span>|<span data-ttu-id="d4095-134">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="d4095-134">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="d4095-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4095-135">Response</span></span>

<span data-ttu-id="d4095-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4095-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4095-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4095-137">Example</span></span>
<span data-ttu-id="d4095-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d4095-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4095-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4095-139">Request</span></span>
<span data-ttu-id="d4095-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4095-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="d4095-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4095-141">Response</span></span>
<span data-ttu-id="d4095-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4095-142">Here is an example of the response.</span></span> <span data-ttu-id="d4095-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4095-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

