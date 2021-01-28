---
title: 'TableColumnCollection: ItemAt'
description: Obtém uma coluna com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f1c03853330fcffe216c0aaf5e3a30372373aa94
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034083"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="c70ba-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="c70ba-103">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="c70ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c70ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c70ba-105">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="c70ba-105">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="c70ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c70ba-106">Permissions</span></span>
<span data-ttu-id="c70ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c70ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c70ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c70ba-109">Permission type</span></span>      | <span data-ttu-id="c70ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c70ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c70ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c70ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c70ba-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c70ba-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c70ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c70ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c70ba-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c70ba-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c70ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c70ba-115">Application</span></span> | <span data-ttu-id="c70ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c70ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c70ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c70ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="c70ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c70ba-118">Request headers</span></span>
| <span data-ttu-id="c70ba-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c70ba-119">Name</span></span>       | <span data-ttu-id="c70ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70ba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c70ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c70ba-121">Authorization</span></span>  | <span data-ttu-id="c70ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c70ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c70ba-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c70ba-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c70ba-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c70ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c70ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c70ba-127">Request body</span></span>
<span data-ttu-id="c70ba-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c70ba-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c70ba-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c70ba-129">Parameter</span></span>    | <span data-ttu-id="c70ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c70ba-130">Type</span></span>   |<span data-ttu-id="c70ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70ba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c70ba-132">index</span><span class="sxs-lookup"><span data-stu-id="c70ba-132">index</span></span>|<span data-ttu-id="c70ba-133">number</span><span class="sxs-lookup"><span data-stu-id="c70ba-133">number</span></span>|<span data-ttu-id="c70ba-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="c70ba-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="c70ba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c70ba-136">Response</span></span>

<span data-ttu-id="c70ba-137">Se bem-sucedido, este método retorna o código de resposta e o objeto `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c70ba-137">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c70ba-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c70ba-138">Example</span></span>
<span data-ttu-id="c70ba-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c70ba-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c70ba-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c70ba-140">Request</span></span>
<span data-ttu-id="c70ba-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c70ba-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c70ba-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c70ba-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c70ba-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c70ba-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c70ba-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c70ba-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c70ba-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c70ba-145">Response</span></span>
<span data-ttu-id="c70ba-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c70ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "99",
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


