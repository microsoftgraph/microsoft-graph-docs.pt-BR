---
author: JeremyKelley
ms.author: JeremyKelley
title: Atualizar o listItem
description: Atualize as propriedades em um **[listItem][]**.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5584ab4bde08ad0386c545f9041b2a8500c72cb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057238"
---
# <a name="update-listitem"></a><span data-ttu-id="61e70-103">Atualizar o listItem</span><span class="sxs-lookup"><span data-stu-id="61e70-103">Update listItem</span></span>

<span data-ttu-id="61e70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61e70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61e70-105">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="61e70-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="61e70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61e70-106">Permissions</span></span>

<span data-ttu-id="61e70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61e70-109">Permission type</span></span>      | <span data-ttu-id="61e70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61e70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61e70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61e70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61e70-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e70-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="61e70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61e70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61e70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61e70-114">Not supported.</span></span>    |
|<span data-ttu-id="61e70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61e70-115">Application</span></span> | <span data-ttu-id="61e70-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e70-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61e70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61e70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="61e70-118">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="61e70-118">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="61e70-119">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="61e70-119">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="61e70-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="61e70-120">Optional request headers</span></span>

| <span data-ttu-id="61e70-121">Nome</span><span class="sxs-lookup"><span data-stu-id="61e70-121">Name</span></span>       | <span data-ttu-id="61e70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61e70-122">Value</span></span> | <span data-ttu-id="61e70-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="61e70-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="61e70-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="61e70-124">_if-match_</span></span> | <span data-ttu-id="61e70-125">etag</span><span class="sxs-lookup"><span data-stu-id="61e70-125">etag</span></span>  | <span data-ttu-id="61e70-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="61e70-126">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="61e70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61e70-127">Request body</span></span> 
<span data-ttu-id="61e70-128">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="61e70-128">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="61e70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61e70-129">Response</span></span> 

<span data-ttu-id="61e70-130">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um [fieldValueSet][] no corpo da resposta para o item de lista atualizado.</span><span class="sxs-lookup"><span data-stu-id="61e70-130">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="61e70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61e70-131">Example</span></span>

<span data-ttu-id="61e70-132">O exemplo a seguir atualiza os campos **Cor** e **Quantidade** do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="61e70-132">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="61e70-133">Todos os outros valores em **listItem** são deixados de lado.</span><span class="sxs-lookup"><span data-stu-id="61e70-133">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="61e70-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61e70-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="61e70-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="61e70-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="61e70-136">C#</span><span class="sxs-lookup"><span data-stu-id="61e70-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61e70-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61e70-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61e70-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61e70-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61e70-139">Java</span><span class="sxs-lookup"><span data-stu-id="61e70-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61e70-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="61e70-140">Response</span></span>

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

