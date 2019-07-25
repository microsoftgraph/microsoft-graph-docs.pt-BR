---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Mover um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: dd5c38420d33a70d056cf4e7189f0d368800b37a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881683"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="b5e48-102">Mover um DriveItem para uma nova pasta</span><span class="sxs-lookup"><span data-stu-id="b5e48-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="b5e48-103">Para mover um DriveItem para um novo item pai, o aplicativo solicita a atualização de **parentReference** do DriveItem a ser movido.</span><span class="sxs-lookup"><span data-stu-id="b5e48-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="b5e48-104">Este é um caso especial do método [Update](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="b5e48-104">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="b5e48-105">O aplicativo pode combinar a movimentação de um item para um novo contêiner e a atualização de outras propriedades do item em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5e48-105">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="b5e48-106">Não é possível mover itens entre [Unidades](../resources/drive.md) usando esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5e48-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e48-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5e48-107">Permissions</span></span>
<span data-ttu-id="b5e48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e48-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5e48-110">Permission type</span></span>      | <span data-ttu-id="b5e48-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5e48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5e48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e48-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e48-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5e48-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5e48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e48-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e48-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5e48-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5e48-116">Application</span></span> | <span data-ttu-id="b5e48-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e48-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e48-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e48-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b5e48-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b5e48-119">Optional request headers</span></span>

| <span data-ttu-id="b5e48-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b5e48-120">Name</span></span>          | <span data-ttu-id="b5e48-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e48-121">Type</span></span>   | <span data-ttu-id="b5e48-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e48-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b5e48-123">if-match</span><span class="sxs-lookup"><span data-stu-id="b5e48-123">if-match</span></span>      | <span data-ttu-id="b5e48-124">String</span><span class="sxs-lookup"><span data-stu-id="b5e48-124">String</span></span> | <span data-ttu-id="b5e48-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="b5e48-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e48-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e48-126">Request body</span></span>

<span data-ttu-id="b5e48-p103">No corpo da solicitação, forneça o novo valor para a propriedade **parentReference**. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b5e48-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="b5e48-130">**Observação:** Ao mover itens para a raiz de uma unidade, seu aplicativo não pode usar a sintaxe `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="b5e48-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="b5e48-131">Seu aplicativo precisa fornecer a ID real da pasta raiz para referência do pai.</span><span class="sxs-lookup"><span data-stu-id="b5e48-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="b5e48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e48-132">Response</span></span>

<span data-ttu-id="b5e48-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5e48-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e48-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5e48-134">Example</span></span>

<span data-ttu-id="b5e48-135">Este exemplo move um item especificado por {item-id} para uma pasta na unidade do usuário com a ID `new-parent-folder-id`.</span><span class="sxs-lookup"><span data-stu-id="b5e48-135">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5e48-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e48-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "{new-parent-folder-id}"
  },
  "name": "new-item-name.txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5e48-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5e48-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5e48-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5e48-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5e48-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b5e48-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5e48-140">Java</span><span class="sxs-lookup"><span data-stu-id="b5e48-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5e48-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e48-141">Response</span></span>

<span data-ttu-id="b5e48-142">O exemplo a seguir mostra a resposta para este pedido de movimentação.</span><span class="sxs-lookup"><span data-stu-id="b5e48-142">The following example shows the response for this move request.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a><span data-ttu-id="b5e48-143">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="b5e48-143">Error responses</span></span>

<span data-ttu-id="b5e48-144">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="b5e48-144">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
  ]
} -->
