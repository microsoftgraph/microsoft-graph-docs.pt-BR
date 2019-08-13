---
title: 'TableColumnCollection: ItemAt'
description: Obtém uma coluna com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e4544324ded67196d1b345e91f1fdda113684901
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363029"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="5d68b-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5d68b-103">TableColumnCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d68b-104">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="5d68b-104">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d68b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d68b-105">Permissions</span></span>
<span data-ttu-id="5d68b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d68b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d68b-108">Permission type</span></span>      | <span data-ttu-id="5d68b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d68b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d68b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d68b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d68b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d68b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d68b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d68b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d68b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d68b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d68b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d68b-114">Application</span></span> | <span data-ttu-id="5d68b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d68b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d68b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d68b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="5d68b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d68b-117">Request headers</span></span>
| <span data-ttu-id="5d68b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5d68b-118">Name</span></span>       | <span data-ttu-id="5d68b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d68b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d68b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d68b-120">Authorization</span></span>  | <span data-ttu-id="5d68b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d68b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d68b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5d68b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5d68b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d68b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d68b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d68b-126">Request body</span></span>
<span data-ttu-id="5d68b-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d68b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d68b-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d68b-128">Parameter</span></span>    | <span data-ttu-id="5d68b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d68b-129">Type</span></span>   |<span data-ttu-id="5d68b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d68b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d68b-131">index</span><span class="sxs-lookup"><span data-stu-id="5d68b-131">index</span></span>|<span data-ttu-id="5d68b-132">number</span><span class="sxs-lookup"><span data-stu-id="5d68b-132">number</span></span>|<span data-ttu-id="5d68b-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5d68b-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5d68b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d68b-135">Response</span></span>

<span data-ttu-id="5d68b-136">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d68b-136">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d68b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d68b-137">Example</span></span>
<span data-ttu-id="5d68b-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5d68b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d68b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d68b-139">Request</span></span>
<span data-ttu-id="5d68b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d68b-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5d68b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d68b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d68b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d68b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d68b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5d68b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d68b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d68b-144">Response</span></span>
<span data-ttu-id="5d68b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d68b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
