---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Mover um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 385c2d9013544b60be5d11fd13ce29df1a6a8ee0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548037"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="538cc-102">Mover um DriveItem para uma nova pasta</span><span class="sxs-lookup"><span data-stu-id="538cc-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="538cc-103">Para mover um DriveItem para um novo item pai, o aplicativo solicita a atualização de **parentReference** do DriveItem a ser movido.</span><span class="sxs-lookup"><span data-stu-id="538cc-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="538cc-104">Este é um caso especial do método [Update](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="538cc-104">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="538cc-105">O aplicativo pode combinar a movimentação de um item para um novo contêiner e a atualização de outras propriedades do item em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="538cc-105">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="538cc-106">Não é possível mover itens entre [Unidades](../resources/drive.md) usando esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="538cc-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="538cc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="538cc-107">Permissions</span></span>
<span data-ttu-id="538cc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="538cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="538cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="538cc-110">Permission type</span></span>      | <span data-ttu-id="538cc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="538cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="538cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="538cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="538cc-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538cc-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="538cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="538cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="538cc-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538cc-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="538cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="538cc-116">Application</span></span> | <span data-ttu-id="538cc-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538cc-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="538cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="538cc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="538cc-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="538cc-119">Optional request headers</span></span>

| <span data-ttu-id="538cc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="538cc-120">Name</span></span>          | <span data-ttu-id="538cc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="538cc-121">Type</span></span>   | <span data-ttu-id="538cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="538cc-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="538cc-123">if-match</span><span class="sxs-lookup"><span data-stu-id="538cc-123">if-match</span></span>      | <span data-ttu-id="538cc-124">String</span><span class="sxs-lookup"><span data-stu-id="538cc-124">String</span></span> | <span data-ttu-id="538cc-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="538cc-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="538cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="538cc-126">Request body</span></span>

<span data-ttu-id="538cc-p103">No corpo da solicitação, forneça o novo valor para a propriedade **parentReference**. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="538cc-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="538cc-130">**Observação:** Ao mover itens para a raiz de uma unidade, seu aplicativo não pode usar a sintaxe `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="538cc-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="538cc-131">Seu aplicativo precisa fornecer a ID real da pasta raiz para referência do pai.</span><span class="sxs-lookup"><span data-stu-id="538cc-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="538cc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="538cc-132">Response</span></span>

<span data-ttu-id="538cc-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="538cc-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538cc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="538cc-134">Example</span></span>

<span data-ttu-id="538cc-135">Este exemplo move um item especificado por {item-id} para uma pasta na unidade do usuário com a ID `new-parent-folder-id`.</span><span class="sxs-lookup"><span data-stu-id="538cc-135">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>

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

### <a name="response"></a><span data-ttu-id="538cc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="538cc-136">Response</span></span>

<span data-ttu-id="538cc-137">O exemplo a seguir mostra a resposta para este pedido de movimentação.</span><span class="sxs-lookup"><span data-stu-id="538cc-137">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="538cc-138">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="538cc-138">Error responses</span></span>

<span data-ttu-id="538cc-139">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="538cc-139">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
