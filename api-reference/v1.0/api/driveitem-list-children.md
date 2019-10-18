---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar o conteúdo de uma pasta
localization_priority: Priority
ms.prod: sharepoint
description: Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 144710d858ced9fd83fb1ed815377f94279736b6
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726372"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="7dc02-103">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="7dc02-103">List children of a driveItem</span></span>

<span data-ttu-id="7dc02-104">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="7dc02-104">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="7dc02-105">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="7dc02-105">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="7dc02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dc02-106">Permissions</span></span>

<span data-ttu-id="7dc02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc02-109">Permission type</span></span>      | <span data-ttu-id="7dc02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dc02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dc02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dc02-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc02-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7dc02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dc02-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc02-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7dc02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dc02-115">Application</span></span> | <span data-ttu-id="7dc02-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc02-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dc02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc02-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dc02-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dc02-118">Optional query parameters</span></span>

<span data-ttu-id="7dc02-119">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7dc02-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="7dc02-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7dc02-120">Optional request headers</span></span>

| <span data-ttu-id="7dc02-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7dc02-121">Name</span></span>     | <span data-ttu-id="7dc02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7dc02-122">Value</span></span> | <span data-ttu-id="7dc02-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc02-123">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7dc02-124">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="7dc02-124">_if-none-match_</span></span> | <span data-ttu-id="7dc02-125">etag</span><span class="sxs-lookup"><span data-stu-id="7dc02-125">etag</span></span>  | <span data-ttu-id="7dc02-126">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="7dc02-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="7dc02-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7dc02-127">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="7dc02-128">Filhos de lista na raiz da unidade do usuário atual</span><span class="sxs-lookup"><span data-stu-id="7dc02-128">List children in the root of the current user's drive</span></span>

<span data-ttu-id="7dc02-129">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="7dc02-129">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7dc02-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc02-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/root/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dc02-131">C#</span><span class="sxs-lookup"><span data-stu-id="7dc02-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dc02-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dc02-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dc02-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dc02-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7dc02-134">Java</span><span class="sxs-lookup"><span data-stu-id="7dc02-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="7dc02-135">Filhos da lista de um DriveItem com uma ID conhecida</span><span class="sxs-lookup"><span data-stu-id="7dc02-135">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="7dc02-136">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="7dc02-136">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7dc02-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc02-137">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-files", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dc02-138">C#</span><span class="sxs-lookup"><span data-stu-id="7dc02-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dc02-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dc02-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dc02-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dc02-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7dc02-141">Java</span><span class="sxs-lookup"><span data-stu-id="7dc02-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="7dc02-142">Filhos da lista de um DriveItem com um caminho conhecido</span><span class="sxs-lookup"><span data-stu-id="7dc02-142">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="7dc02-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc02-143">Response</span></span>

<span data-ttu-id="7dc02-144">Se tiver êxito, esse método retornará a lista de itens no conjunto de filhos do item de destino.</span><span class="sxs-lookup"><span data-stu-id="7dc02-144">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="7dc02-145">A coleção secundária será composta de recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="7dc02-145">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children-files", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="7dc02-146">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **\@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="7dc02-146">Note: If a collection exceeds the default page size (200 items), the @odata.nextLink property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="7dc02-147">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de caracteres de consulta opcional](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="7dc02-147">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="7dc02-148">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="7dc02-148">Error responses</span></span>

<span data-ttu-id="7dc02-149">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="7dc02-149">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
} -->
