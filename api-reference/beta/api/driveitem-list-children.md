---
author: JeremyKelley
description: Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.
ms.date: 09/10/2017
title: Listar o conteúdo de uma pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3a3e6a33f80675cfdb4a34c347814012e6320227
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458287"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="00f71-103">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="00f71-103">List children of a driveItem</span></span>

<span data-ttu-id="00f71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f71-105">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="00f71-105">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="00f71-106">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="00f71-106">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="00f71-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="00f71-107">Permissions</span></span>

<span data-ttu-id="00f71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f71-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00f71-110">Permission type</span></span>      | <span data-ttu-id="00f71-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00f71-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00f71-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00f71-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00f71-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f71-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="00f71-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00f71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f71-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f71-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="00f71-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00f71-116">Application</span></span> | <span data-ttu-id="00f71-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f71-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f71-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00f71-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00f71-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00f71-119">Optional query parameters</span></span>

<span data-ttu-id="00f71-120">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00f71-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="00f71-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="00f71-121">Optional request headers</span></span>

| <span data-ttu-id="00f71-122">Nome de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00f71-122">Header name</span></span>     | <span data-ttu-id="00f71-123">Valor</span><span class="sxs-lookup"><span data-stu-id="00f71-123">Value</span></span> | <span data-ttu-id="00f71-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="00f71-124">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="00f71-125">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="00f71-125">_if-none-match_</span></span> | <span data-ttu-id="00f71-126">etag</span><span class="sxs-lookup"><span data-stu-id="00f71-126">etag</span></span>  | <span data-ttu-id="00f71-127">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="00f71-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="00f71-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00f71-128">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="00f71-129">Filhos de lista na raiz da unidade do usuário atual</span><span class="sxs-lookup"><span data-stu-id="00f71-129">List children in the root of the current user's drive</span></span>

<span data-ttu-id="00f71-130">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="00f71-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="http"></a>[<span data-ttu-id="00f71-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="00f71-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/root/children
```
# <a name="c"></a>[<span data-ttu-id="00f71-132">C#</span><span class="sxs-lookup"><span data-stu-id="00f71-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00f71-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00f71-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00f71-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00f71-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="00f71-135">Filhos da lista de um DriveItem com uma ID conhecida</span><span class="sxs-lookup"><span data-stu-id="00f71-135">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="00f71-136">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="00f71-136">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="http"></a>[<span data-ttu-id="00f71-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="00f71-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="c"></a>[<span data-ttu-id="00f71-138">C#</span><span class="sxs-lookup"><span data-stu-id="00f71-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00f71-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00f71-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00f71-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00f71-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="00f71-141">Filhos da lista de um DriveItem com um caminho conhecido</span><span class="sxs-lookup"><span data-stu-id="00f71-141">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="00f71-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="00f71-142">Response</span></span>

<span data-ttu-id="00f71-143">Se tiver êxito, esse método retornará a lista de itens no conjunto de filhos do item de destino.</span><span class="sxs-lookup"><span data-stu-id="00f71-143">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="00f71-144">A coleção secundária será composta de recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="00f71-144">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

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

<span data-ttu-id="00f71-145">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **\@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="00f71-145">**Note:** If a collection exceeds the default page size (200 items), the **\@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="00f71-146">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de caracteres de consulta opcional](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="00f71-146">You can control the page size through [optional query string parameters](/graph/query-parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="00f71-147">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="00f71-147">Error responses</span></span>

<span data-ttu-id="00f71-148">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="00f71-148">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
}
-->
