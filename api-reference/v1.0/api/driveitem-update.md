---
author: JeremyKelley
ms.date: 09/10/2017
title: Atualizar um arquivo ou uma pasta
localization_priority: Priority
ms.prod: sharepoint
description: Atualize os metadados de um DriveItem por ID ou caminho.
doc_type: apiPageType
ms.openlocfilehash: 01456ff44b20641b13b2718c20e87ae601ef764f
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240185"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="bcdb1-103">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="bcdb1-103">Update DriveItem properties</span></span>

<span data-ttu-id="bcdb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcdb1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcdb1-105">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="bcdb1-106">Também é possível usar a atualização para [mover um item](driveitem-move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcdb1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcdb1-107">Permissions</span></span>

<span data-ttu-id="bcdb1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcdb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcdb1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcdb1-110">Permission type</span></span>      | <span data-ttu-id="bcdb1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcdb1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcdb1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcdb1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcdb1-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdb1-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcdb1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcdb1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcdb1-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdb1-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcdb1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcdb1-116">Application</span></span> | <span data-ttu-id="bcdb1-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdb1-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcdb1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcdb1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="bcdb1-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bcdb1-119">Optional request headers</span></span>

| <span data-ttu-id="bcdb1-120">Name</span><span class="sxs-lookup"><span data-stu-id="bcdb1-120">Name</span></span>          | <span data-ttu-id="bcdb1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcdb1-121">Type</span></span>   | <span data-ttu-id="bcdb1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcdb1-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bcdb1-123">if-match</span><span class="sxs-lookup"><span data-stu-id="bcdb1-123">if-match</span></span>      | <span data-ttu-id="bcdb1-124">String</span><span class="sxs-lookup"><span data-stu-id="bcdb1-124">String</span></span> | <span data-ttu-id="bcdb1-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcdb1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcdb1-126">Request body</span></span>

<span data-ttu-id="bcdb1-127">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="bcdb1-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="bcdb1-129">Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="bcdb1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcdb1-130">Response</span></span>

<span data-ttu-id="bcdb1-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcdb1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcdb1-132">Example</span></span>

<span data-ttu-id="bcdb1-133">Este exemplo renomeia o recurso DriveItem como "new-file-name.docx".</span><span class="sxs-lookup"><span data-stu-id="bcdb1-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="http"></a>[<span data-ttu-id="bcdb1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcdb1-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="c"></a>[<span data-ttu-id="bcdb1-135">C#</span><span class="sxs-lookup"><span data-stu-id="bcdb1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcdb1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcdb1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcdb1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcdb1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcdb1-138">Java</span><span class="sxs-lookup"><span data-stu-id="bcdb1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bcdb1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcdb1-139">Response</span></span>

<span data-ttu-id="bcdb1-140">Se tiver êxito, esse método retornará um recurso [driveItem][item-resource]no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-140">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="bcdb1-141">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="bcdb1-141">Error responses</span></span>

<span data-ttu-id="bcdb1-142">Confira [Respostas de erro][error-response] para saber mais detalhes sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="bcdb1-142">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
} -->

