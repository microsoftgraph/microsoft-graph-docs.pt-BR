---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar o conteúdo de uma pasta
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a280c68561aa764ccab74dc871465fb134e39d79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272846"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="4c680-102">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="4c680-102">List children of a driveItem</span></span>

<span data-ttu-id="4c680-103">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4c680-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="4c680-104">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="4c680-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="4c680-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c680-105">Permissions</span></span>

<span data-ttu-id="4c680-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c680-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c680-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c680-108">Permission type</span></span>      | <span data-ttu-id="4c680-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c680-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c680-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c680-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c680-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c680-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c680-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c680-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c680-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c680-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c680-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c680-114">Application</span></span> | <span data-ttu-id="4c680-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c680-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c680-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c680-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c680-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c680-117">Optional query parameters</span></span>

<span data-ttu-id="4c680-118">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c680-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="4c680-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4c680-119">Optional request headers</span></span>

| <span data-ttu-id="4c680-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4c680-120">Name</span></span>     | <span data-ttu-id="4c680-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c680-121">Value</span></span> | <span data-ttu-id="4c680-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c680-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4c680-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="4c680-123">_if-none-match_</span></span> | <span data-ttu-id="4c680-124">etag</span><span class="sxs-lookup"><span data-stu-id="4c680-124">etag</span></span>  | <span data-ttu-id="4c680-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="4c680-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="4c680-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c680-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="4c680-127">Filhos de lista na raiz da unidade do usuário atual</span><span class="sxs-lookup"><span data-stu-id="4c680-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="4c680-128">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="4c680-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/root/children
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c680-129">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4c680-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c680-130">C#</span><span class="sxs-lookup"><span data-stu-id="4c680-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-children-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c680-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c680-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-children-root-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c680-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c680-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-children-root-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="4c680-133">Filhos da lista de um DriveItem com uma ID conhecida</span><span class="sxs-lookup"><span data-stu-id="4c680-133">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="4c680-134">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="4c680-134">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-files", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c680-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4c680-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c680-136">C#</span><span class="sxs-lookup"><span data-stu-id="4c680-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-children-files-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c680-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c680-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-children-files-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c680-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c680-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-children-files-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="4c680-139">Filhos da lista de um DriveItem com um caminho conhecido</span><span class="sxs-lookup"><span data-stu-id="4c680-139">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="4c680-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c680-140">Response</span></span>

<span data-ttu-id="4c680-141">Se tiver êxito, esse método retornará a lista de itens no conjunto de filhos do item de destino.</span><span class="sxs-lookup"><span data-stu-id="4c680-141">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="4c680-142">A coleção de filhos será composta de recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="4c680-142">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="4c680-143">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="4c680-143">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="4c680-144">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de caracteres de consulta opcional](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="4c680-144">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="4c680-145">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="4c680-145">Error responses</span></span>

<span data-ttu-id="4c680-146">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="4c680-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
