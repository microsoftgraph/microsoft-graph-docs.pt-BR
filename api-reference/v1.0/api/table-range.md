---
title: 'Table: Range'
description: Obtém o objeto de intervalo associado a toda a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4ea53274f4f529bb054e540e4e838366ac631734
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509637"
---
# <a name="table-range"></a><span data-ttu-id="85339-103">Table: Range</span><span class="sxs-lookup"><span data-stu-id="85339-103">Table: Range</span></span>

<span data-ttu-id="85339-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85339-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85339-105">Obtém o objeto de intervalo associado a toda a tabela.</span><span class="sxs-lookup"><span data-stu-id="85339-105">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="85339-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85339-106">Permissions</span></span>
<span data-ttu-id="85339-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85339-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85339-109">Permission type</span></span>      | <span data-ttu-id="85339-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85339-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85339-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85339-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85339-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85339-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85339-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85339-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85339-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85339-114">Not supported.</span></span>    |
|<span data-ttu-id="85339-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85339-115">Application</span></span> | <span data-ttu-id="85339-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85339-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85339-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85339-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/range
POST /workbook/worksheets/{id|name}/tables/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="85339-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85339-118">Request headers</span></span>
| <span data-ttu-id="85339-119">Nome</span><span class="sxs-lookup"><span data-stu-id="85339-119">Name</span></span>       | <span data-ttu-id="85339-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="85339-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85339-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85339-121">Authorization</span></span>  | <span data-ttu-id="85339-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85339-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85339-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85339-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="85339-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="85339-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85339-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85339-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="85339-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85339-128">Response</span></span>

<span data-ttu-id="85339-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85339-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85339-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85339-130">Example</span></span>
<span data-ttu-id="85339-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="85339-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85339-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85339-132">Request</span></span>
<span data-ttu-id="85339-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85339-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85339-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="85339-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_range",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="85339-135">C#</span><span class="sxs-lookup"><span data-stu-id="85339-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85339-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85339-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85339-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85339-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85339-138">Java</span><span class="sxs-lookup"><span data-stu-id="85339-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85339-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="85339-139">Response</span></span>
<span data-ttu-id="85339-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85339-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
