---
author: JeremyKelley
description: Atualize os metadados de um DriveItem por ID ou caminho.
ms.date: 09/10/2017
title: Atualizar um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: cff8bc2d7f5c4daec1da7e26f6f07b873b55dbee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432310"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="e8391-103">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="e8391-103">Update DriveItem properties</span></span>

<span data-ttu-id="e8391-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e8391-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8391-105">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="e8391-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="e8391-106">Também é possível usar a atualização para [mover um item](driveitem-move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="e8391-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8391-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8391-107">Permissions</span></span>

<span data-ttu-id="e8391-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8391-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8391-110">Permission type</span></span>      | <span data-ttu-id="e8391-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8391-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8391-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8391-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8391-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8391-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8391-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8391-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8391-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8391-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8391-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8391-116">Application</span></span> | <span data-ttu-id="e8391-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8391-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8391-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8391-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="e8391-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e8391-119">Optional request headers</span></span>

| <span data-ttu-id="e8391-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e8391-120">Name</span></span>          | <span data-ttu-id="e8391-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8391-121">Type</span></span>   | <span data-ttu-id="e8391-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8391-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e8391-123">if-match</span><span class="sxs-lookup"><span data-stu-id="e8391-123">if-match</span></span>      | <span data-ttu-id="e8391-124">String</span><span class="sxs-lookup"><span data-stu-id="e8391-124">String</span></span> | <span data-ttu-id="e8391-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="e8391-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8391-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8391-126">Request body</span></span>

<span data-ttu-id="e8391-127">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e8391-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="e8391-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8391-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="e8391-129">Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="e8391-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="e8391-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8391-130">Response</span></span>

<span data-ttu-id="e8391-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8391-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8391-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8391-132">Example</span></span>

<span data-ttu-id="e8391-133">Este exemplo renomeia o recurso DriveItem como "new-file-name.docx".</span><span class="sxs-lookup"><span data-stu-id="e8391-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="http"></a>[<span data-ttu-id="e8391-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8391-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="c"></a>[<span data-ttu-id="e8391-135">C#</span><span class="sxs-lookup"><span data-stu-id="e8391-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8391-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8391-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8391-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8391-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8391-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8391-138">Response</span></span>

<span data-ttu-id="e8391-139">Se tiver êxito, esse método retornará um recurso [driveItem][item-resource]no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8391-139">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="e8391-140">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="e8391-140">Error responses</span></span>

<span data-ttu-id="e8391-141">Confira [Respostas de erro][error-response] para saber mais detalhes sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="e8391-141">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
}
-->
