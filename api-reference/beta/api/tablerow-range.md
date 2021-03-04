---
title: 'TableRow: Range'
description: Retorna o objeto de intervalo associado a toda a linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7fe71bf10a935994f24a5e3c59cff8ef97a6cfe5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440581"
---
# <a name="tablerow-range"></a><span data-ttu-id="7015f-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="7015f-103">TableRow: Range</span></span>

<span data-ttu-id="7015f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7015f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7015f-105">Retorna o objeto de intervalo associado a toda a linha.</span><span class="sxs-lookup"><span data-stu-id="7015f-105">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="7015f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7015f-106">Permissions</span></span>
<span data-ttu-id="7015f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7015f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7015f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7015f-109">Permission type</span></span>      | <span data-ttu-id="7015f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7015f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7015f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7015f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7015f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7015f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7015f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7015f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7015f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7015f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7015f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7015f-115">Application</span></span> | <span data-ttu-id="7015f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7015f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7015f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7015f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/Range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/Range

```
## <a name="request-headers"></a><span data-ttu-id="7015f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7015f-118">Request headers</span></span>
| <span data-ttu-id="7015f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7015f-119">Name</span></span>       | <span data-ttu-id="7015f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7015f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7015f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7015f-121">Authorization</span></span>  | <span data-ttu-id="7015f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7015f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7015f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7015f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7015f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7015f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7015f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7015f-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7015f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7015f-128">Response</span></span>

<span data-ttu-id="7015f-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7015f-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7015f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7015f-130">Example</span></span>
<span data-ttu-id="7015f-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7015f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7015f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7015f-132">Request</span></span>
<span data-ttu-id="7015f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7015f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7015f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7015f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerow_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/Range
```
# <a name="c"></a>[<span data-ttu-id="7015f-135">C#</span><span class="sxs-lookup"><span data-stu-id="7015f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerow-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7015f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7015f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerow-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7015f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7015f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerow-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7015f-138">Java</span><span class="sxs-lookup"><span data-stu-id="7015f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerow-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7015f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7015f-139">Response</span></span>
<span data-ttu-id="7015f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7015f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


