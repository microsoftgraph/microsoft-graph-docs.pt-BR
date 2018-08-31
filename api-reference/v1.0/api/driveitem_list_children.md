---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar o conteúdo de uma pasta
ms.openlocfilehash: 31e20780379055b9ec8217bb90b4da26414a64e5
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265215"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="16eff-102">Listar os filhos de um driveItem</span><span class="sxs-lookup"><span data-stu-id="16eff-102">List children of a driveItem</span></span>

<span data-ttu-id="16eff-103">Retorne uma coleção de [DriveItems](../resources/driveitem.md) na relação **children** de um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="16eff-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="16eff-104">DriveItems com uma faceta **folder** ou **package** não nula podem ter um ou mais DriveItems filhos.</span><span class="sxs-lookup"><span data-stu-id="16eff-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="16eff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="16eff-105">Permissions</span></span>

<span data-ttu-id="16eff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16eff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16eff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16eff-108">Permission type</span></span>      | <span data-ttu-id="16eff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16eff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16eff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16eff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16eff-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16eff-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="16eff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16eff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16eff-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16eff-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="16eff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16eff-114">Application</span></span> | <span data-ttu-id="16eff-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16eff-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16eff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16eff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16eff-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16eff-117">Optional query parameters</span></span>

<span data-ttu-id="16eff-118">Este método oferece suporte aos [Parâmetros de consulta OData](../../../concepts/query_parameters.md) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16eff-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="16eff-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="16eff-119">Optional request headers</span></span>

| <span data-ttu-id="16eff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="16eff-120">Name</span></span>     | <span data-ttu-id="16eff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16eff-121">Value</span></span> | <span data-ttu-id="16eff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="16eff-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="16eff-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="16eff-123">_if-none-match_</span></span> | <span data-ttu-id="16eff-124">etag</span><span class="sxs-lookup"><span data-stu-id="16eff-124">etag</span></span>  | <span data-ttu-id="16eff-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="16eff-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="16eff-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16eff-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="16eff-127">Filhos de lista na raiz da unidade do usuário atual</span><span class="sxs-lookup"><span data-stu-id="16eff-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="16eff-128">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="16eff-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="16eff-129">Filhos da lista de um DriveItem com uma ID conhecida</span><span class="sxs-lookup"><span data-stu-id="16eff-129">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="16eff-130">Para recuperar arquivos na raiz da unidade, use a relação `root` na unidade e acesse a relação de filhos.</span><span class="sxs-lookup"><span data-stu-id="16eff-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="16eff-131">Filhos da lista de um DriveItem com um caminho conhecido</span><span class="sxs-lookup"><span data-stu-id="16eff-131">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="16eff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="16eff-132">Response</span></span>

<span data-ttu-id="16eff-133">Se tiver êxito, esse método retornará a lista de itens no conjunto de filhos do item de destino.</span><span class="sxs-lookup"><span data-stu-id="16eff-133">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="16eff-134">A coleção de filhos será composta de recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="16eff-134">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="16eff-135">**Observação:** Se uma coleção exceder o tamanho de página padrão (200 itens), a propriedade **@odata.nextLink** será retornada na resposta para indicar que mais itens estão disponíveis e fornecer a URL da solicitação para a próxima página de itens.</span><span class="sxs-lookup"><span data-stu-id="16eff-135">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="16eff-136">Você pode controlar o tamanho da página por meio de [parâmetros de cadeia de consulta opcionais](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="16eff-136">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="16eff-137">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="16eff-137">Error responses</span></span>

<span data-ttu-id="16eff-138">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="16eff-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children"
} -->
