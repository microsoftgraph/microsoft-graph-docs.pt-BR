---
author: JeremyKelley
description: Atualizar as propriedades de um listItem.
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4c97e9fbb9957a7d0f652c106d1bf427d16d0898
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475839"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="86c25-103">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="86c25-103">Update an item in a list</span></span>

<span data-ttu-id="86c25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c25-105">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="86c25-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="86c25-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86c25-106">Permissions</span></span>

<span data-ttu-id="86c25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86c25-109">Permission type</span></span>      | <span data-ttu-id="86c25-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86c25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86c25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86c25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86c25-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c25-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="86c25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86c25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86c25-114">Not supported.</span></span>    |
|<span data-ttu-id="86c25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86c25-115">Application</span></span> | <span data-ttu-id="86c25-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c25-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86c25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86c25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="86c25-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="86c25-118">Optional request headers</span></span>

| <span data-ttu-id="86c25-119">Nome</span><span class="sxs-lookup"><span data-stu-id="86c25-119">Name</span></span>       | <span data-ttu-id="86c25-120">Valor</span><span class="sxs-lookup"><span data-stu-id="86c25-120">Value</span></span> | <span data-ttu-id="86c25-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c25-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="86c25-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="86c25-122">_if-match_</span></span> | <span data-ttu-id="86c25-123">etag</span><span class="sxs-lookup"><span data-stu-id="86c25-123">etag</span></span>  | <span data-ttu-id="86c25-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="86c25-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="86c25-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86c25-125">Request body</span></span>

<span data-ttu-id="86c25-126">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="86c25-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="86c25-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86c25-127">Example</span></span>

<span data-ttu-id="86c25-128">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="86c25-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="86c25-129">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="86c25-129">All other values on the listItem are left alone.</span></span> 


# <a name="http"></a>[<span data-ttu-id="86c25-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="86c25-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="86c25-131">C#</span><span class="sxs-lookup"><span data-stu-id="86c25-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86c25-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86c25-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86c25-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86c25-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="86c25-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c25-134">Response</span></span>

<span data-ttu-id="86c25-135">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="86c25-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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


