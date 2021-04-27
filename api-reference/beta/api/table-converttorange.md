---
title: 'Table: convertToRange'
description: Converte a tabela em um intervalo de células normal. Todos os dados são preservados.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af678a145dd0d3f4afdc7aac150f8421cf536b74
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036517"
---
# <a name="table-converttorange"></a><span data-ttu-id="4298f-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="4298f-104">Table: convertToRange</span></span>

<span data-ttu-id="4298f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4298f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4298f-p102">Converte a tabela em um intervalo de células normal. Todos os dados são preservados.</span><span class="sxs-lookup"><span data-stu-id="4298f-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="4298f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4298f-108">Permissions</span></span>
<span data-ttu-id="4298f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4298f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4298f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4298f-111">Permission type</span></span>      | <span data-ttu-id="4298f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4298f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4298f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4298f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4298f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4298f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4298f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4298f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4298f-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4298f-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4298f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4298f-117">Application</span></span> | <span data-ttu-id="4298f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4298f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4298f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4298f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/convertToRange
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/convertToRange
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="4298f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4298f-120">Request headers</span></span>
| <span data-ttu-id="4298f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4298f-121">Name</span></span>       | <span data-ttu-id="4298f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4298f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4298f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4298f-123">Authorization</span></span>  | <span data-ttu-id="4298f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4298f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4298f-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4298f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="4298f-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4298f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4298f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4298f-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4298f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4298f-130">Response</span></span>

<span data-ttu-id="4298f-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4298f-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4298f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4298f-132">Example</span></span>
<span data-ttu-id="4298f-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4298f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4298f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4298f-134">Request</span></span>
<span data-ttu-id="4298f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4298f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4298f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4298f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="c"></a>[<span data-ttu-id="4298f-137">C#</span><span class="sxs-lookup"><span data-stu-id="4298f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4298f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4298f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4298f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4298f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4298f-140">Java</span><span class="sxs-lookup"><span data-stu-id="4298f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-converttorange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4298f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4298f-141">Response</span></span>
<span data-ttu-id="4298f-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4298f-142">Here is an example of the response.</span></span> <span data-ttu-id="4298f-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4298f-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


