---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7437986c3da827f0c36fdddfad59653d75fc7f1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510694"
---
# <a name="range-boundingrect"></a><span data-ttu-id="f9334-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="f9334-103">Range: BoundingRect</span></span>

<span data-ttu-id="f9334-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9334-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9334-p101">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="f9334-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="f9334-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9334-107">Permissions</span></span>
<span data-ttu-id="f9334-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9334-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9334-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9334-110">Permission type</span></span>      | <span data-ttu-id="f9334-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9334-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9334-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9334-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9334-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9334-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9334-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9334-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9334-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9334-115">Not supported.</span></span>    |
|<span data-ttu-id="f9334-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9334-116">Application</span></span> | <span data-ttu-id="f9334-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9334-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9334-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9334-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/boundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="f9334-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9334-119">Request headers</span></span>
| <span data-ttu-id="f9334-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f9334-120">Name</span></span>       | <span data-ttu-id="f9334-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9334-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9334-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9334-122">Authorization</span></span>  | <span data-ttu-id="f9334-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9334-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9334-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9334-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9334-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9334-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9334-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9334-128">Request body</span></span>
<span data-ttu-id="f9334-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9334-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9334-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9334-130">Parameter</span></span>    | <span data-ttu-id="f9334-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9334-131">Type</span></span>   |<span data-ttu-id="f9334-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9334-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9334-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="f9334-133">anotherRange</span></span>|<span data-ttu-id="f9334-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9334-134">string</span></span>|<span data-ttu-id="f9334-135">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="f9334-135">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="f9334-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9334-136">Response</span></span>

<span data-ttu-id="f9334-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9334-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9334-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9334-138">Example</span></span>
<span data-ttu-id="f9334-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f9334-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9334-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9334-140">Request</span></span>
<span data-ttu-id="f9334-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9334-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/boundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="f9334-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9334-142">Response</span></span>
<span data-ttu-id="f9334-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9334-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
