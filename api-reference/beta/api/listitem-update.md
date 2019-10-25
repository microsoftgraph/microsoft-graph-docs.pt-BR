---
author: JeremyKelley
description: Atualizar as propriedades de um listItem.
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8ddc87113fb94660f11f8f9113ac11c62e389375
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726289"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="a0165-103">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="a0165-103">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0165-104">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="a0165-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0165-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0165-105">Permissions</span></span>

<span data-ttu-id="a0165-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0165-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0165-108">Permission type</span></span>      | <span data-ttu-id="a0165-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0165-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0165-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0165-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0165-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0165-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0165-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0165-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0165-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0165-113">Not supported.</span></span>    |
|<span data-ttu-id="a0165-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0165-114">Application</span></span> | <span data-ttu-id="a0165-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0165-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0165-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0165-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="a0165-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a0165-117">Optional request headers</span></span>

| <span data-ttu-id="a0165-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a0165-118">Name</span></span>       | <span data-ttu-id="a0165-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a0165-119">Value</span></span> | <span data-ttu-id="a0165-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0165-120">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a0165-121">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a0165-121">_if-match_</span></span> | <span data-ttu-id="a0165-122">etag</span><span class="sxs-lookup"><span data-stu-id="a0165-122">etag</span></span>  | <span data-ttu-id="a0165-123">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="a0165-123">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="a0165-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0165-124">Request body</span></span>

<span data-ttu-id="a0165-125">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="a0165-125">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="a0165-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0165-126">Example</span></span>

<span data-ttu-id="a0165-127">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="a0165-127">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="a0165-128">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="a0165-128">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="a0165-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0165-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0165-130">C#</span><span class="sxs-lookup"><span data-stu-id="a0165-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0165-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0165-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0165-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0165-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a0165-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0165-133">Response</span></span>

<span data-ttu-id="a0165-134">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="a0165-134">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
}
-->
