---
author: JeremyKelley
ms.author: jeremyke
title: Criar pacote
description: Criar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a586617ed783d737386c3487502e9af14f2348e6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955768"
---
# <a name="create-bundle"></a><span data-ttu-id="c874a-103">Criar pacote</span><span class="sxs-lookup"><span data-stu-id="c874a-103">Create bundle</span></span>

<span data-ttu-id="c874a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c874a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c874a-105">Adicione um novo [pacote][] à unidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="c874a-105">Add a new [bundle][] to the user's drive.</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="c874a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c874a-107">Permissions</span></span>

<span data-ttu-id="c874a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c874a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c874a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c874a-110">Permission type</span></span>      | <span data-ttu-id="c874a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c874a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c874a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c874a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c874a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c874a-113">Not supported.</span></span>                             |
|<span data-ttu-id="c874a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c874a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c874a-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c874a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="c874a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c874a-116">Application</span></span>          | <span data-ttu-id="c874a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c874a-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="c874a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c874a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="c874a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c874a-119">Request headers</span></span>

| <span data-ttu-id="c874a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c874a-120">Name</span></span>          | <span data-ttu-id="c874a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c874a-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="c874a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c874a-122">Authorization</span></span> | <span data-ttu-id="c874a-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="c874a-123">Bearer \{token\}.</span></span> <span data-ttu-id="c874a-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c874a-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c874a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c874a-125">Request body</span></span>

<span data-ttu-id="c874a-126">No corpo da solicitação, forneça uma representação JSON do pacote a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c874a-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="c874a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c874a-127">Response</span></span>

<span data-ttu-id="c874a-128">Se a solicitação for bem-sucedida, o [driveItem](../resources/driveitem.md) que representa o novo pacote recém-criado será retornado.</span><span class="sxs-lookup"><span data-stu-id="c874a-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="c874a-129">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="c874a-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="c874a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c874a-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="c874a-131">Exemplo 1: criar um pacote</span><span class="sxs-lookup"><span data-stu-id="c874a-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="c874a-132">O exemplo a seguir mostra como criar um novo pacote básico.</span><span class="sxs-lookup"><span data-stu-id="c874a-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="c874a-133">Essa solicitação criará um novo pacote chamado `Just some files` e adicionará dois itens existentes ao pacote.</span><span class="sxs-lookup"><span data-stu-id="c874a-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="c874a-134">Este pacote pode ser usado para compartilhar uma coleção de arquivos com outros usuários sem compartilhar a pasta em que os itens estão armazenados.</span><span class="sxs-lookup"><span data-stu-id="c874a-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="c874a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c874a-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c874a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c874a-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
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
# <a name="c"></a>[<span data-ttu-id="c874a-137">C#</span><span class="sxs-lookup"><span data-stu-id="c874a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c874a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c874a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c874a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c874a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c874a-140">Java</span><span class="sxs-lookup"><span data-stu-id="c874a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c874a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c874a-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="c874a-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c874a-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c874a-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c874a-143">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="c874a-144">Exemplo 2: criar um álbum</span><span class="sxs-lookup"><span data-stu-id="c874a-144">Example 2: Create an album</span></span>

<span data-ttu-id="c874a-145">A solicitação para criar um novo álbum de fotografias é semelhante, embora dentro da faceta de pacote, a propriedade Album é definida como um valor não nulo.</span><span class="sxs-lookup"><span data-stu-id="c874a-145">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="c874a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c874a-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c874a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c874a-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
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
# <a name="c"></a>[<span data-ttu-id="c874a-148">C#</span><span class="sxs-lookup"><span data-stu-id="c874a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c874a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c874a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c874a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c874a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c874a-151">Java</span><span class="sxs-lookup"><span data-stu-id="c874a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c874a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c874a-152">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="c874a-153">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c874a-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c874a-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c874a-154">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="c874a-155">Se _@microsoft. Graph. conflictBehavior_ for definido como **Rename** e um pacote com o mesmo nome já existir, o novo nome do pacote será atualizado para ser exclusivo.</span><span class="sxs-lookup"><span data-stu-id="c874a-155">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="c874a-156">O OneDrive acrescentará um número ao final do nome do pacote.</span><span class="sxs-lookup"><span data-stu-id="c874a-156">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="c874a-157">Por exemplo, `My Day at the Beach` poderia ser renomeado `My Day at the Beach 1`.</span><span class="sxs-lookup"><span data-stu-id="c874a-157">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="c874a-158">Se `My Day at the Beach 1` for executado, o número será incrementado novamente até que um nome de pacote exclusivo seja descoberto.</span><span class="sxs-lookup"><span data-stu-id="c874a-158">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->


