---
title: 'Range: EntireRow'
description: Obtém um objeto que representa toda a linha do intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 605378e02755e65f827daf227e96b28c171c515b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309146"
---
# <a name="range-entirerow"></a><span data-ttu-id="21e7e-103">Range: EntireRow</span><span class="sxs-lookup"><span data-stu-id="21e7e-103">Range: EntireRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21e7e-104">Obtém um objeto que representa toda a linha do intervalo.</span><span class="sxs-lookup"><span data-stu-id="21e7e-104">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="21e7e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="21e7e-105">Permissions</span></span>
<span data-ttu-id="21e7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21e7e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21e7e-108">Permission type</span></span>      | <span data-ttu-id="21e7e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21e7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21e7e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21e7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21e7e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21e7e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21e7e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21e7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e7e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21e7e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21e7e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21e7e-114">Application</span></span> | <span data-ttu-id="21e7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21e7e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21e7e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21e7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/EntireRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireRow

```
## <a name="request-headers"></a><span data-ttu-id="21e7e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21e7e-117">Request headers</span></span>
| <span data-ttu-id="21e7e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="21e7e-118">Name</span></span>       | <span data-ttu-id="21e7e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e7e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="21e7e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="21e7e-120">Authorization</span></span>  | <span data-ttu-id="21e7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21e7e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21e7e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="21e7e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="21e7e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="21e7e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21e7e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21e7e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="21e7e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e7e-127">Response</span></span>

<span data-ttu-id="21e7e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21e7e-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e7e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21e7e-129">Example</span></span>
<span data-ttu-id="21e7e-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="21e7e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="21e7e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21e7e-131">Request</span></span>
<span data-ttu-id="21e7e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21e7e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21e7e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="21e7e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/EntireRow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21e7e-134">C#</span><span class="sxs-lookup"><span data-stu-id="21e7e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21e7e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21e7e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21e7e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="21e7e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21e7e-137">Java</span><span class="sxs-lookup"><span data-stu-id="21e7e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="21e7e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e7e-138">Response</span></span>
<span data-ttu-id="21e7e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21e7e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
