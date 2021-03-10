---
title: 'Range: Intersection'
description: Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bceba8e704b1a4c3e0ee485b8c10643f9bf84e4c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577706"
---
# <a name="range-intersection"></a><span data-ttu-id="7151b-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="7151b-103">Range: Intersection</span></span>

<span data-ttu-id="7151b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7151b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7151b-105">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="7151b-105">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="7151b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7151b-106">Permissions</span></span>
<span data-ttu-id="7151b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7151b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7151b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7151b-109">Permission type</span></span>      | <span data-ttu-id="7151b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7151b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7151b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7151b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7151b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7151b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7151b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7151b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7151b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7151b-114">Not supported.</span></span>    |
|<span data-ttu-id="7151b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7151b-115">Application</span></span> | <span data-ttu-id="7151b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7151b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7151b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7151b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/intersection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="7151b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7151b-118">Request headers</span></span>
| <span data-ttu-id="7151b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7151b-119">Name</span></span>       | <span data-ttu-id="7151b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7151b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7151b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7151b-121">Authorization</span></span>  | <span data-ttu-id="7151b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7151b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7151b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7151b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7151b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7151b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7151b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7151b-127">Request body</span></span>
<span data-ttu-id="7151b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7151b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7151b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7151b-129">Parameter</span></span>    | <span data-ttu-id="7151b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7151b-130">Type</span></span>   |<span data-ttu-id="7151b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7151b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7151b-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="7151b-132">anotherRange</span></span>|<span data-ttu-id="7151b-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7151b-133">string</span></span>|<span data-ttu-id="7151b-134">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="7151b-134">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="7151b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7151b-135">Response</span></span>

<span data-ttu-id="7151b-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7151b-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7151b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7151b-137">Example</span></span>
<span data-ttu-id="7151b-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7151b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7151b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7151b-139">Request</span></span>
<span data-ttu-id="7151b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7151b-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7151b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7151b-141">Response</span></span>
<span data-ttu-id="7151b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7151b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

