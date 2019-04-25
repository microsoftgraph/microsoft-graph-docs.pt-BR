---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19155801297caf56a9ba944b4220c4ba8db0bb36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546365"
---
# <a name="range-boundingrect"></a><span data-ttu-id="e3803-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="e3803-103">Range: BoundingRect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3803-p101">Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="e3803-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="e3803-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3803-106">Permissions</span></span>
<span data-ttu-id="e3803-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3803-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3803-109">Permission type</span></span>      | <span data-ttu-id="e3803-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3803-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3803-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3803-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3803-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3803-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e3803-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3803-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3803-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3803-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e3803-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3803-115">Application</span></span> | <span data-ttu-id="e3803-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3803-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3803-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3803-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="e3803-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3803-118">Request headers</span></span>
| <span data-ttu-id="e3803-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e3803-119">Name</span></span>       | <span data-ttu-id="e3803-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3803-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e3803-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3803-121">Authorization</span></span>  | <span data-ttu-id="e3803-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3803-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3803-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e3803-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e3803-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e3803-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3803-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3803-127">Request body</span></span>
<span data-ttu-id="e3803-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3803-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3803-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e3803-129">Parameter</span></span>    | <span data-ttu-id="e3803-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3803-130">Type</span></span>   |<span data-ttu-id="e3803-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3803-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3803-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="e3803-132">anotherRange</span></span>|<span data-ttu-id="e3803-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3803-133">string</span></span>|<span data-ttu-id="e3803-134">O objeto de intervalo, endereço ou nome do intervalo.</span><span class="sxs-lookup"><span data-stu-id="e3803-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="e3803-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3803-135">Response</span></span>

<span data-ttu-id="e3803-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3803-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3803-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3803-137">Example</span></span>
<span data-ttu-id="e3803-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e3803-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e3803-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3803-139">Request</span></span>
<span data-ttu-id="e3803-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3803-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="e3803-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3803-141">Response</span></span>
<span data-ttu-id="e3803-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3803-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "suppressions": [
    "Error: /api-reference/beta/api/range-boundingrect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
