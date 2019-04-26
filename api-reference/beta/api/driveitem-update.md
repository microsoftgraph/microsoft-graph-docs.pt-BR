---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Atualizar um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ec7a9c98fa23164ef58340cc5de8fae6a953c773
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325224"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="30f98-102">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="30f98-102">Update DriveItem properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30f98-103">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="30f98-103">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="30f98-104">Também é possível usar a atualização para [mover um item](driveitem-move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="30f98-104">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="30f98-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30f98-105">Permissions</span></span>

<span data-ttu-id="30f98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30f98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30f98-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30f98-108">Permission type</span></span>      | <span data-ttu-id="30f98-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30f98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30f98-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30f98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30f98-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f98-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="30f98-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30f98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30f98-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f98-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="30f98-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30f98-114">Application</span></span> | <span data-ttu-id="30f98-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f98-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30f98-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30f98-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="30f98-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="30f98-117">Optional request headers</span></span>

| <span data-ttu-id="30f98-118">Name</span><span class="sxs-lookup"><span data-stu-id="30f98-118">Name</span></span>          | <span data-ttu-id="30f98-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="30f98-119">Type</span></span>   | <span data-ttu-id="30f98-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30f98-120">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="30f98-121">if-match</span><span class="sxs-lookup"><span data-stu-id="30f98-121">if-match</span></span>      | <span data-ttu-id="30f98-122">String</span><span class="sxs-lookup"><span data-stu-id="30f98-122">String</span></span> | <span data-ttu-id="30f98-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="30f98-123">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30f98-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30f98-124">Request body</span></span>

<span data-ttu-id="30f98-125">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="30f98-125">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="30f98-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="30f98-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="30f98-127">Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="30f98-127">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="30f98-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="30f98-128">Response</span></span>

<span data-ttu-id="30f98-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30f98-129">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30f98-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30f98-130">Example</span></span>

<span data-ttu-id="30f98-131">Este exemplo renomeia o recurso DriveItem como "new-file-name.docx".</span><span class="sxs-lookup"><span data-stu-id="30f98-131">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="30f98-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="30f98-132">Response</span></span>

<span data-ttu-id="30f98-133">Se tiver êxito, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30f98-133">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="30f98-134">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="30f98-134">Error responses</span></span>

<span data-ttu-id="30f98-135">Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="30f98-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": []
}
-->
