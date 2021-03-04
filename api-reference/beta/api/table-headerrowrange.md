---
title: 'Table: HeaderRowRange'
description: Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 08f96d3b33d612d1498694fdb5db7a547a05e861
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440693"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="89147-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="89147-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="89147-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89147-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89147-105">Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.</span><span class="sxs-lookup"><span data-stu-id="89147-105">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="89147-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89147-106">Permissions</span></span>
<span data-ttu-id="89147-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89147-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89147-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89147-109">Permission type</span></span>      | <span data-ttu-id="89147-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89147-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89147-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89147-111">Delegated (work or school account)</span></span> | <span data-ttu-id="89147-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89147-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89147-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89147-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89147-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89147-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89147-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89147-115">Application</span></span> | <span data-ttu-id="89147-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89147-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89147-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89147-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/HeaderRowRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="89147-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89147-118">Request headers</span></span>
| <span data-ttu-id="89147-119">Nome</span><span class="sxs-lookup"><span data-stu-id="89147-119">Name</span></span>       | <span data-ttu-id="89147-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="89147-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89147-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="89147-121">Authorization</span></span>  | <span data-ttu-id="89147-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89147-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89147-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="89147-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="89147-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="89147-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89147-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89147-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="89147-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="89147-128">Response</span></span>

<span data-ttu-id="89147-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89147-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89147-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89147-130">Example</span></span>
<span data-ttu-id="89147-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="89147-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="89147-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89147-132">Request</span></span>
<span data-ttu-id="89147-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89147-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89147-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="89147-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```
# <a name="c"></a>[<span data-ttu-id="89147-135">C#</span><span class="sxs-lookup"><span data-stu-id="89147-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89147-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89147-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89147-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89147-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89147-138">Java</span><span class="sxs-lookup"><span data-stu-id="89147-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-headerrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="89147-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="89147-139">Response</span></span>
<span data-ttu-id="89147-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89147-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


