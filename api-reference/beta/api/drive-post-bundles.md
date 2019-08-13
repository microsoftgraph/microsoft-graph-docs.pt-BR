---
author: JeremyKelley
ms.author: jeremyke
title: Criar pacote
description: Criar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a43c04aa0710007afdab9788c41df98903011532
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321089"
---
# <a name="create-bundle"></a><span data-ttu-id="d5ce8-103">Criar pacote</span><span class="sxs-lookup"><span data-stu-id="d5ce8-103">Create bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5ce8-104">Adicione um novo [pacote][] à unidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-104">Add a new [bundle][] to the user's drive.</span></span>

[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="d5ce8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5ce8-106">Permissions</span></span>

<span data-ttu-id="d5ce8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ce8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5ce8-109">Permission type</span></span>      | <span data-ttu-id="d5ce8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5ce8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5ce8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5ce8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5ce8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-112">Not supported.</span></span>                             |
|<span data-ttu-id="d5ce8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5ce8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5ce8-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ce8-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="d5ce8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5ce8-115">Application</span></span>          | <span data-ttu-id="d5ce8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="d5ce8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5ce8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="d5ce8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ce8-118">Request headers</span></span>

| <span data-ttu-id="d5ce8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5ce8-119">Name</span></span>          | <span data-ttu-id="d5ce8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5ce8-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="d5ce8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5ce8-121">Authorization</span></span> | <span data-ttu-id="d5ce8-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-122">Bearer \{token\}.</span></span> <span data-ttu-id="d5ce8-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5ce8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ce8-124">Request body</span></span>

<span data-ttu-id="d5ce8-125">No corpo da solicitação, forneça uma representação JSON do pacote a ser criado.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-125">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="d5ce8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5ce8-126">Response</span></span>

<span data-ttu-id="d5ce8-127">Se a solicitação for bem-sucedida, o [driveItem](../resources/driveitem.md) que representa o novo pacote recém-criado será retornado.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-127">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="d5ce8-128">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="d5ce8-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5ce8-129">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="d5ce8-130">Exemplo 1: criar um pacote</span><span class="sxs-lookup"><span data-stu-id="d5ce8-130">Example 1: Create a bundle</span></span>

<span data-ttu-id="d5ce8-131">O exemplo a seguir mostra como criar um novo pacote básico.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-131">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="d5ce8-132">Essa solicitação criará um novo pacote chamado `Just some files` e adicionará dois itens existentes ao pacote.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-132">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="d5ce8-133">Este pacote pode ser usado para compartilhar uma coleção de arquivos com outros usuários sem compartilhar a pasta em que os itens estão armazenados.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-133">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="d5ce8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ce8-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5ce8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5ce8-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@name.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5ce8-136">C#</span><span class="sxs-lookup"><span data-stu-id="d5ce8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5ce8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5ce8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5ce8-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5ce8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5ce8-139">Java</span><span class="sxs-lookup"><span data-stu-id="d5ce8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5ce8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5ce8-140">Response</span></span>

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

<span data-ttu-id="d5ce8-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d5ce8-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-142">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="d5ce8-143">Exemplo 2: criar um álbum</span><span class="sxs-lookup"><span data-stu-id="d5ce8-143">Example 2: Create an album</span></span>

<span data-ttu-id="d5ce8-144">A solicitação para criar um novo álbum de fotografias é semelhante, embora dentro da faceta de pacote, a propriedade Album é definida como um valor não nulo.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="d5ce8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ce8-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5ce8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5ce8-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5ce8-147">C#</span><span class="sxs-lookup"><span data-stu-id="d5ce8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5ce8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5ce8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5ce8-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5ce8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5ce8-150">Java</span><span class="sxs-lookup"><span data-stu-id="d5ce8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5ce8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5ce8-151">Response</span></span>

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

<span data-ttu-id="d5ce8-152">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-152">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d5ce8-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-153">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="d5ce8-154">Se _@microsoft. Graph. conflictBehavior_ for definido como **Rename** e um pacote com o mesmo nome já existir, o novo nome do pacote será atualizado para ser exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-154">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="d5ce8-155">O OneDrive acrescentará um número ao final do nome do pacote.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-155">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="d5ce8-156">Por exemplo, `My Day at the Beach` poderia ser renomeado `My Day at the Beach 1`.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-156">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="d5ce8-157">Se `My Day at the Beach 1` for executado, o número será incrementado novamente até que um nome de pacote exclusivo seja descoberto.</span><span class="sxs-lookup"><span data-stu-id="d5ce8-157">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->
