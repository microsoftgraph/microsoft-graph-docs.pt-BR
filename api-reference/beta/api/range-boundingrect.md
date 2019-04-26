---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483aa57cc4781d4d6e8a0e65537eb5b8b6e4526d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337254"
---
# <a name="range-boundingrect"></a><span data-ttu-id="b0703-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="b0703-103">Range: BoundingRect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0703-p101">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="b0703-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="b0703-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0703-106">Permissions</span></span>
<span data-ttu-id="b0703-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0703-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0703-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0703-109">Permission type</span></span>      | <span data-ttu-id="b0703-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0703-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0703-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0703-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0703-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0703-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0703-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0703-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0703-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0703-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0703-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0703-115">Application</span></span> | <span data-ttu-id="b0703-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0703-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0703-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0703-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="b0703-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0703-118">Request headers</span></span>
| <span data-ttu-id="b0703-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b0703-119">Name</span></span>       | <span data-ttu-id="b0703-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0703-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0703-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0703-121">Authorization</span></span>  | <span data-ttu-id="b0703-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0703-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0703-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0703-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0703-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b0703-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0703-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0703-127">Request body</span></span>
<span data-ttu-id="b0703-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0703-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b0703-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b0703-129">Parameter</span></span>    | <span data-ttu-id="b0703-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0703-130">Type</span></span>   |<span data-ttu-id="b0703-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0703-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0703-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="b0703-132">anotherRange</span></span>|<span data-ttu-id="b0703-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0703-133">string</span></span>|<span data-ttu-id="b0703-134">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="b0703-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="b0703-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0703-135">Response</span></span>

<span data-ttu-id="b0703-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0703-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0703-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0703-137">Example</span></span>
<span data-ttu-id="b0703-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b0703-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0703-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0703-139">Request</span></span>
<span data-ttu-id="b0703-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0703-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="b0703-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0703-141">Response</span></span>
<span data-ttu-id="b0703-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0703-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
