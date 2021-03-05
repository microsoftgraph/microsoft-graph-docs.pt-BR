---
author: JeremyKelley
title: Criar pacote
description: Criar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8883006a6aa1daf86e4d3b8a6efac31e0ae25376
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471380"
---
# <a name="create-bundle"></a><span data-ttu-id="d2c88-103">Criar pacote</span><span class="sxs-lookup"><span data-stu-id="d2c88-103">Create bundle</span></span>

<span data-ttu-id="d2c88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2c88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2c88-105">Adicione um novo [pacote][] à unidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2c88-105">Add a new [bundle][] to the user's drive.</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="d2c88-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2c88-107">Permissions</span></span>

<span data-ttu-id="d2c88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2c88-110">Permission type</span></span>      | <span data-ttu-id="d2c88-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2c88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2c88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2c88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2c88-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c88-113">Not supported.</span></span>                             |
|<span data-ttu-id="d2c88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2c88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2c88-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c88-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="d2c88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2c88-116">Application</span></span>          | <span data-ttu-id="d2c88-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2c88-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="d2c88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c88-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="d2c88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c88-119">Request headers</span></span>

| <span data-ttu-id="d2c88-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d2c88-120">Name</span></span>          | <span data-ttu-id="d2c88-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2c88-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="d2c88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2c88-122">Authorization</span></span> | <span data-ttu-id="d2c88-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="d2c88-123">Bearer \{token\}.</span></span> <span data-ttu-id="d2c88-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2c88-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2c88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c88-125">Request body</span></span>

<span data-ttu-id="d2c88-126">No corpo da solicitação, fornece uma representação JSON do pacote a ser criado.</span><span class="sxs-lookup"><span data-stu-id="d2c88-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="d2c88-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c88-127">Response</span></span>

<span data-ttu-id="d2c88-128">Se a solicitação for bem-sucedida, [o driveItem](../resources/driveitem.md) que representa o pacote recém-criado será retornado.</span><span class="sxs-lookup"><span data-stu-id="d2c88-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="d2c88-129">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="d2c88-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="d2c88-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2c88-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="d2c88-131">Exemplo 1: Criar um pacote</span><span class="sxs-lookup"><span data-stu-id="d2c88-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="d2c88-132">O exemplo a seguir mostra como criar um novo pacote básico.</span><span class="sxs-lookup"><span data-stu-id="d2c88-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="d2c88-133">Essa solicitação criará um novo pacote chamado e adicionará dois `Just some files` itens existentes ao pacote.</span><span class="sxs-lookup"><span data-stu-id="d2c88-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="d2c88-134">Esse pacote pode ser usado para compartilhar uma coleção de arquivos com outros usuários sem compartilhar a pasta em que esses itens são armazenados.</span><span class="sxs-lookup"><span data-stu-id="d2c88-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="d2c88-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c88-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d2c88-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c88-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d2c88-137">C#</span><span class="sxs-lookup"><span data-stu-id="d2c88-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2c88-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2c88-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2c88-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2c88-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2c88-140">Java</span><span class="sxs-lookup"><span data-stu-id="d2c88-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2c88-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c88-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

<span data-ttu-id="d2c88-142">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c88-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2c88-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2c88-143">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="d2c88-144">Exemplo 2: Criar um álbum</span><span class="sxs-lookup"><span data-stu-id="d2c88-144">Example 2: Create an album</span></span>

<span data-ttu-id="d2c88-145">A solicitação para criar um novo álbum de fotos é semelhante, embora dentro da faceta do pacote, a propriedade do álbum seja definida como um valor não nulo.</span><span class="sxs-lookup"><span data-stu-id="d2c88-145">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="d2c88-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2c88-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d2c88-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c88-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d2c88-148">C#</span><span class="sxs-lookup"><span data-stu-id="d2c88-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2c88-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2c88-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2c88-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2c88-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2c88-151">Java</span><span class="sxs-lookup"><span data-stu-id="d2c88-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2c88-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2c88-152">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

<span data-ttu-id="d2c88-153">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="d2c88-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2c88-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2c88-154">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="d2c88-155">Se _@microsoft.graph.conflictBehavior_ estiver definido para **renomear** e um pacote com o mesmo nome já existir, o novo nome do pacote será atualizado para ser exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d2c88-155">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="d2c88-156">O OneDrive anexa um número ao final do nome do pacote.</span><span class="sxs-lookup"><span data-stu-id="d2c88-156">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="d2c88-157">Por exemplo, `My Day at the Beach` poderia ser renomeado `My Day at the Beach 1`.</span><span class="sxs-lookup"><span data-stu-id="d2c88-157">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="d2c88-158">Se `My Day at the Beach 1` for tomada, o número será incrementado novamente até que um nome de pacote exclusivo seja descoberto.</span><span class="sxs-lookup"><span data-stu-id="d2c88-158">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->


