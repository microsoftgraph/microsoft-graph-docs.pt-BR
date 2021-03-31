---
author: swapnil1993
title: Atualizar columnDefinition
description: Atualizar uma coluna de site, lista ou tipo de conteúdo
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0a18f128b92496fa956600557a4a8923efc8d117
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468904"
---
# <a name="update-columndefinition"></a><span data-ttu-id="5801f-103">Atualizar columnDefinition</span><span class="sxs-lookup"><span data-stu-id="5801f-103">Update columnDefinition</span></span>
<span data-ttu-id="5801f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5801f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="5801f-105">Atualizar um [site,][] [lista ou][] [tipo de conteúdo.][contentType] [column][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="5801f-105">Update a [site][], [list][] or [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="5801f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5801f-106">Permissions</span></span>  

<span data-ttu-id="5801f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5801f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="5801f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5801f-109">Permission type</span></span> | <span data-ttu-id="5801f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5801f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5801f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5801f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5801f-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5801f-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="5801f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5801f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5801f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5801f-114">Not supported.</span></span> |
|<span data-ttu-id="5801f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5801f-115">Application</span></span> | <span data-ttu-id="5801f-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5801f-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="5801f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5801f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="5801f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5801f-118">Request headers</span></span>
|<span data-ttu-id="5801f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5801f-119">Name</span></span>|<span data-ttu-id="5801f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5801f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5801f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5801f-121">Authorization</span></span>|<span data-ttu-id="5801f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5801f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5801f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5801f-124">Content-Type</span></span>|<span data-ttu-id="5801f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5801f-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="5801f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5801f-127">Request body</span></span>

<span data-ttu-id="5801f-128">No corpo da solicitação, fornece uma representação JSON dessas propriedades de um [recurso columnDefinition][] a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="5801f-128">In the request body, supply a JSON representation of those properties of a [columnDefinition][] resource to update.</span></span> <span data-ttu-id="5801f-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5801f-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="5801f-130">Para colunas no **site** ou **lista**, você pode atualizar qualquer propriedade **de columnDefinition** diferente da **propriedade id.**</span><span class="sxs-lookup"><span data-stu-id="5801f-130">For columns in **site** or **list**, you can update any property of **columnDefinition** other than the **id** property.</span></span>

<span data-ttu-id="5801f-131">Para colunas em **contentType**, você pode atualizar apenas **a propriedade necessária** **ou** oculta.</span><span class="sxs-lookup"><span data-stu-id="5801f-131">For columns in **contentType**, you can update only the **required** or **hidden** property.</span></span>

## <a name="response"></a><span data-ttu-id="5801f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5801f-132">Response</span></span>

<span data-ttu-id="5801f-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [columnDefinition][] atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5801f-133">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5801f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5801f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5801f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5801f-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5801f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5801f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype_column"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```
# <a name="c"></a>[<span data-ttu-id="5801f-137">C#</span><span class="sxs-lookup"><span data-stu-id="5801f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5801f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5801f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5801f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5801f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5801f-140">Java</span><span class="sxs-lookup"><span data-stu-id="5801f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5801f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5801f-141">Response</span></span>
><span data-ttu-id="5801f-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5801f-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
[site]: ../resources/site.md

