---
author: JeremyKelley
ms.author: JeremyKelley
title: Atualizar o listItem
description: Atualize as propriedades em um **[listItem][]**.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: ff13cdf8279e5051e3ebf0f650fc73de9270db14
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884508"
---
# <a name="update-listitem"></a><span data-ttu-id="2f6c4-103">Atualizar o listItem</span><span class="sxs-lookup"><span data-stu-id="2f6c4-103">Update listItem</span></span>

<span data-ttu-id="2f6c4-104">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f6c4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f6c4-105">Permissions</span></span>

<span data-ttu-id="2f6c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f6c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f6c4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f6c4-108">Permission type</span></span>      | <span data-ttu-id="2f6c4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f6c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f6c4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f6c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f6c4-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6c4-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f6c4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f6c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f6c4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-113">Not supported.</span></span>    |
|<span data-ttu-id="2f6c4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f6c4-114">Application</span></span> | <span data-ttu-id="2f6c4-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6c4-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f6c4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f6c4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="2f6c4-117">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-117">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="2f6c4-118">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-118">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="2f6c4-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2f6c4-119">Optional request headers</span></span>

| <span data-ttu-id="2f6c4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2f6c4-120">Name</span></span>       | <span data-ttu-id="2f6c4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f6c4-121">Value</span></span> | <span data-ttu-id="2f6c4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f6c4-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="2f6c4-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="2f6c4-123">_if-match_</span></span> | <span data-ttu-id="2f6c4-124">etag</span><span class="sxs-lookup"><span data-stu-id="2f6c4-124">etag</span></span>  | <span data-ttu-id="2f6c4-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-125">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="2f6c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6c4-126">Request body</span></span> 
<span data-ttu-id="2f6c4-127">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-127">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="2f6c4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6c4-128">Response</span></span> 

<span data-ttu-id="2f6c4-129">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um [fieldValueSet][] no corpo da resposta para o item de lista atualizado.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-129">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="2f6c4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f6c4-130">Example</span></span>

<span data-ttu-id="2f6c4-131">O exemplo a seguir atualiza os campos **Cor** e **Quantidade** do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-131">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="2f6c4-132">Todos os outros valores em **listItem** são deixados de lado.</span><span class="sxs-lookup"><span data-stu-id="2f6c4-132">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="2f6c4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6c4-133">Request</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="2f6c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f6c4-134">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f6c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f6c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f6c4-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f6c4-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f6c4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f6c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2f6c4-138">Java</span><span class="sxs-lookup"><span data-stu-id="2f6c4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f6c4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6c4-139">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
} -->
