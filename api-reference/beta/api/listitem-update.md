---
author: JeremyKelley
description: Atualizar as propriedades de um listItem.
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c46206a77359a6a60aaa4193f1d5ff7395a597d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942380"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="0f3d6-103">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="0f3d6-103">Update an item in a list</span></span>

<span data-ttu-id="0f3d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f3d6-105">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f3d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f3d6-106">Permissions</span></span>

<span data-ttu-id="0f3d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f3d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f3d6-109">Permission type</span></span>      | <span data-ttu-id="0f3d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f3d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f3d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f3d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f3d6-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f3d6-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f3d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f3d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f3d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-114">Not supported.</span></span>    |
|<span data-ttu-id="0f3d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f3d6-115">Application</span></span> | <span data-ttu-id="0f3d6-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f3d6-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f3d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="0f3d6-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0f3d6-118">Optional request headers</span></span>

| <span data-ttu-id="0f3d6-119">Name</span><span class="sxs-lookup"><span data-stu-id="0f3d6-119">Name</span></span>       | <span data-ttu-id="0f3d6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0f3d6-120">Value</span></span> | <span data-ttu-id="0f3d6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f3d6-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="0f3d6-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="0f3d6-122">_if-match_</span></span> | <span data-ttu-id="0f3d6-123">etag</span><span class="sxs-lookup"><span data-stu-id="0f3d6-123">etag</span></span>  | <span data-ttu-id="0f3d6-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="0f3d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3d6-125">Request body</span></span>

<span data-ttu-id="0f3d6-126">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="0f3d6-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f3d6-127">Example</span></span>

<span data-ttu-id="0f3d6-128">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="0f3d6-129">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-129">All other values on the listItem are left alone.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0f3d6-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3d6-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem-2", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="0f3d6-131">C#</span><span class="sxs-lookup"><span data-stu-id="0f3d6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f3d6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f3d6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f3d6-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f3d6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="0f3d6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f3d6-134">Response</span></span>

<span data-ttu-id="0f3d6-135">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="0f3d6-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
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


