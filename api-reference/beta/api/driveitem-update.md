---
author: JeremyKelley
description: Atualize os metadados de um DriveItem por ID ou caminho.
ms.date: 09/10/2017
title: Atualizar um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba59a69a9e7fb9ce40f77e206511c1f9d58927a3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324215"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="81159-103">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="81159-103">Update DriveItem properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81159-104">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="81159-104">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="81159-105">Também é possível usar a atualização para [mover um item](driveitem-move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="81159-105">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="81159-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81159-106">Permissions</span></span>

<span data-ttu-id="81159-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81159-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81159-109">Permission type</span></span>      | <span data-ttu-id="81159-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81159-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81159-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81159-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81159-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81159-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="81159-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81159-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81159-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="81159-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81159-115">Application</span></span> | <span data-ttu-id="81159-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81159-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81159-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81159-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="81159-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="81159-118">Optional request headers</span></span>

| <span data-ttu-id="81159-119">Nome</span><span class="sxs-lookup"><span data-stu-id="81159-119">Name</span></span>          | <span data-ttu-id="81159-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="81159-120">Type</span></span>   | <span data-ttu-id="81159-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="81159-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="81159-122">if-match</span><span class="sxs-lookup"><span data-stu-id="81159-122">if-match</span></span>      | <span data-ttu-id="81159-123">String</span><span class="sxs-lookup"><span data-stu-id="81159-123">String</span></span> | <span data-ttu-id="81159-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="81159-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81159-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81159-125">Request body</span></span>

<span data-ttu-id="81159-126">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="81159-126">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="81159-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="81159-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="81159-128">Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="81159-128">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="81159-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81159-129">Response</span></span>

<span data-ttu-id="81159-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81159-130">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81159-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81159-131">Example</span></span>

<span data-ttu-id="81159-132">Este exemplo renomeia o recurso DriveItem como "new-file-name.docx".</span><span class="sxs-lookup"><span data-stu-id="81159-132">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="81159-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="81159-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81159-134">C#</span><span class="sxs-lookup"><span data-stu-id="81159-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81159-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81159-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81159-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="81159-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81159-137">Java</span><span class="sxs-lookup"><span data-stu-id="81159-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81159-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="81159-138">Response</span></span>

<span data-ttu-id="81159-139">Se tiver êxito, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81159-139">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="81159-140">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="81159-140">Error responses</span></span>

<span data-ttu-id="81159-141">Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="81159-141">See [Error Responses][error-response] for details about how errors are returned.</span></span>

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
