---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Atualizar um arquivo ou uma pasta
ms.openlocfilehash: 90fab8a4cfafdbff888e53f968a67fa34c0599d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038061"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="563ff-102">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="563ff-102">Update DriveItem properties</span></span>

> <span data-ttu-id="563ff-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="563ff-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="563ff-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="563ff-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="563ff-105">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="563ff-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="563ff-106">Também é possível usar a atualização para [mover um item](driveitem-move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="563ff-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="563ff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="563ff-107">Permissions</span></span>

<span data-ttu-id="563ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="563ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="563ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="563ff-110">Permission type</span></span>      | <span data-ttu-id="563ff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="563ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="563ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="563ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="563ff-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563ff-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="563ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="563ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="563ff-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563ff-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="563ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="563ff-116">Application</span></span> | <span data-ttu-id="563ff-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563ff-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="563ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="563ff-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="563ff-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="563ff-119">Optional request headers</span></span>

| <span data-ttu-id="563ff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="563ff-120">Name</span></span>          | <span data-ttu-id="563ff-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="563ff-121">Type</span></span>   | <span data-ttu-id="563ff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="563ff-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="563ff-123">if-match</span><span class="sxs-lookup"><span data-stu-id="563ff-123">if-match</span></span>      | <span data-ttu-id="563ff-124">String</span><span class="sxs-lookup"><span data-stu-id="563ff-124">String</span></span> | <span data-ttu-id="563ff-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="563ff-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="563ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="563ff-126">Request body</span></span>

<span data-ttu-id="563ff-127">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="563ff-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="563ff-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="563ff-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="563ff-129">Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="563ff-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="563ff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="563ff-130">Response</span></span>

<span data-ttu-id="563ff-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="563ff-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="563ff-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="563ff-132">Example</span></span>

<span data-ttu-id="563ff-133">Este exemplo renomeia o recurso DriveItem como "new-file-name.docx".</span><span class="sxs-lookup"><span data-stu-id="563ff-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="563ff-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="563ff-134">Response</span></span>

<span data-ttu-id="563ff-135">Se tiver êxito, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="563ff-135">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="563ff-136">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="563ff-136">Error responses</span></span>

<span data-ttu-id="563ff-137">Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="563ff-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update"
} -->
