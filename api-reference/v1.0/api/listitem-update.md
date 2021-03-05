---
author: JeremyKelley
title: Atualizar o listItem
description: Atualize as propriedades em um **[listItem][]**.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b1801539278f2a68bd7ebd3ab0cf505f9ecf1055
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474831"
---
# <a name="update-listitem"></a><span data-ttu-id="e432c-103">Atualizar o listItem</span><span class="sxs-lookup"><span data-stu-id="e432c-103">Update listItem</span></span>

<span data-ttu-id="e432c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e432c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e432c-105">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e432c-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e432c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e432c-106">Permissions</span></span>

<span data-ttu-id="e432c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e432c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e432c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e432c-109">Permission type</span></span>      | <span data-ttu-id="e432c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e432c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e432c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e432c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e432c-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e432c-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e432c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e432c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e432c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e432c-114">Not supported.</span></span>    |
|<span data-ttu-id="e432c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e432c-115">Application</span></span> | <span data-ttu-id="e432c-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e432c-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e432c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e432c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e432c-118">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="e432c-118">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="e432c-119">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="e432c-119">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="e432c-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e432c-120">Optional request headers</span></span>

| <span data-ttu-id="e432c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e432c-121">Name</span></span>       | <span data-ttu-id="e432c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e432c-122">Value</span></span> | <span data-ttu-id="e432c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e432c-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="e432c-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="e432c-124">_if-match_</span></span> | <span data-ttu-id="e432c-125">etag</span><span class="sxs-lookup"><span data-stu-id="e432c-125">etag</span></span>  | <span data-ttu-id="e432c-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="e432c-126">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="e432c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e432c-127">Request body</span></span> 
<span data-ttu-id="e432c-128">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="e432c-128">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="e432c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e432c-129">Response</span></span> 

<span data-ttu-id="e432c-130">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um [fieldValueSet][] no corpo da resposta para o item de lista atualizado.</span><span class="sxs-lookup"><span data-stu-id="e432c-130">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="e432c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e432c-131">Example</span></span>

<span data-ttu-id="e432c-132">O exemplo a seguir atualiza os campos **Cor** e **Quantidade** do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="e432c-132">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="e432c-133">Todos os outros valores em **listItem** são deixados de lado.</span><span class="sxs-lookup"><span data-stu-id="e432c-133">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="e432c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e432c-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="e432c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e432c-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="e432c-136">C#</span><span class="sxs-lookup"><span data-stu-id="e432c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e432c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e432c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e432c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e432c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e432c-139">Java</span><span class="sxs-lookup"><span data-stu-id="e432c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e432c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e432c-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
} -->

