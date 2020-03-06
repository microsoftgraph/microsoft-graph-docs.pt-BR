---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Mover um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
description: Para mover um DriveItem para um novo item pai, o aplicativo solicita a atualização de parentReference do DriveItem a ser movido.
doc_type: apiPageType
ms.openlocfilehash: 16c4c68ec4224313cf30d88cb00ee1abb58c5e76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517696"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="12f3c-103">Mover um DriveItem para uma nova pasta</span><span class="sxs-lookup"><span data-stu-id="12f3c-103">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="12f3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12f3c-105">Para mover um DriveItem para um novo item pai, o aplicativo solicita a atualização de **parentReference** do DriveItem a ser movido.</span><span class="sxs-lookup"><span data-stu-id="12f3c-105">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="12f3c-106">Este é um caso especial do método [Update](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="12f3c-106">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="12f3c-107">O aplicativo pode combinar a movimentação de um item para um novo contêiner e a atualização de outras propriedades do item em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="12f3c-107">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="12f3c-108">Não é possível mover itens entre [Unidades](../resources/drive.md) usando esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="12f3c-108">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="12f3c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="12f3c-109">Permissions</span></span>
<span data-ttu-id="12f3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12f3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f3c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12f3c-112">Permission type</span></span>      | <span data-ttu-id="12f3c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12f3c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12f3c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12f3c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="12f3c-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f3c-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="12f3c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12f3c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12f3c-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f3c-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="12f3c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12f3c-118">Application</span></span> | <span data-ttu-id="12f3c-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f3c-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12f3c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12f3c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="12f3c-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="12f3c-121">Optional request headers</span></span>

| <span data-ttu-id="12f3c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="12f3c-122">Name</span></span>          | <span data-ttu-id="12f3c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="12f3c-123">Type</span></span>   | <span data-ttu-id="12f3c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f3c-124">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="12f3c-125">if-match</span><span class="sxs-lookup"><span data-stu-id="12f3c-125">if-match</span></span>      | <span data-ttu-id="12f3c-126">String</span><span class="sxs-lookup"><span data-stu-id="12f3c-126">String</span></span> | <span data-ttu-id="12f3c-127">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="12f3c-127">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12f3c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12f3c-128">Request body</span></span>

<span data-ttu-id="12f3c-p103">No corpo da solicitação, forneça o novo valor para a propriedade **parentReference**. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="12f3c-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="12f3c-132">**Observação:** Ao mover itens para a raiz de uma unidade, seu aplicativo não pode usar a sintaxe `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="12f3c-132">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="12f3c-133">Seu aplicativo precisa fornecer a ID real da pasta raiz para referência do pai.</span><span class="sxs-lookup"><span data-stu-id="12f3c-133">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="12f3c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="12f3c-134">Response</span></span>

<span data-ttu-id="12f3c-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12f3c-135">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f3c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12f3c-136">Example</span></span>

<span data-ttu-id="12f3c-137">Este exemplo move um item especificado por {item-id} para uma pasta na unidade do usuário com a ID `new-parent-folder-id`.</span><span class="sxs-lookup"><span data-stu-id="12f3c-137">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="http"></a>[<span data-ttu-id="12f3c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="12f3c-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="12f3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="12f3c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12f3c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12f3c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12f3c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12f3c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12f3c-142">Java</span><span class="sxs-lookup"><span data-stu-id="12f3c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12f3c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="12f3c-143">Response</span></span>

<span data-ttu-id="12f3c-144">O exemplo a seguir mostra a resposta para este pedido de movimentação.</span><span class="sxs-lookup"><span data-stu-id="12f3c-144">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="12f3c-145">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="12f3c-145">Error responses</span></span>

<span data-ttu-id="12f3c-146">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="12f3c-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
