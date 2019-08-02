---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Pesquisar arquivos
localization_priority: Priority
ms.prod: sharepoint
description: Pesquise a hierarquia de itens para itens que corresponda a uma consulta.
doc_type: apiPageType
ms.openlocfilehash: 57cc2c15d7bf49d724ec35290a929c5b52cfc475
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015366"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="071e1-103">Pesquisar um DriveItem em uma unidade</span><span class="sxs-lookup"><span data-stu-id="071e1-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="071e1-104">Pesquise a hierarquia de itens para itens que correspondam a uma consulta.</span><span class="sxs-lookup"><span data-stu-id="071e1-104">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="071e1-105">Você pode pesquisar em uma hierarquia de pastas, uma unidade inteira ou arquivos compartilhados com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="071e1-105">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="071e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="071e1-106">Permissions</span></span>

<span data-ttu-id="071e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="071e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="071e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="071e1-109">Permission type</span></span>      | <span data-ttu-id="071e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="071e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="071e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="071e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="071e1-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="071e1-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="071e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="071e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="071e1-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="071e1-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="071e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="071e1-115">Application</span></span> | <span data-ttu-id="071e1-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="071e1-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="071e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="071e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="071e1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="071e1-118">Optional query parameters</span></span>

<span data-ttu-id="071e1-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="071e1-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="071e1-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="071e1-120">Function parameters</span></span>

| <span data-ttu-id="071e1-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="071e1-121">Parameter</span></span> | <span data-ttu-id="071e1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="071e1-122">Type</span></span>  | <span data-ttu-id="071e1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="071e1-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="071e1-124">q</span><span class="sxs-lookup"><span data-stu-id="071e1-124">q</span></span>  | <span data-ttu-id="071e1-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="071e1-125">string</span></span> | <span data-ttu-id="071e1-p103">O texto de consulta usado para pesquisar itens. Os valores podem ser correspondidos em vários campos, incluindo nome do arquivo, metadados e conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="071e1-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="071e1-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="071e1-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="071e1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="071e1-129">Request</span></span>

<span data-ttu-id="071e1-130">Aqui está um exemplo da solicitação de que pesquisa o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="071e1-130">Here is an example of the request searching the current user's OneDrive</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="071e1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="071e1-131">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="071e1-132">C#</span><span class="sxs-lookup"><span data-stu-id="071e1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="071e1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="071e1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="071e1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="071e1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="071e1-135">Java</span><span class="sxs-lookup"><span data-stu-id="071e1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="071e1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="071e1-136">Response</span></span>

<span data-ttu-id="071e1-p104">Este método retorna um objeto que contém uma coleção de [DriveItems](../resources/driveitem.md) que correspondem aos critérios de pesquisa. Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="071e1-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="071e1-p105">Se houver muitas correspondências, a resposta será paginada, e uma propriedade **@odata.nextLink** conterá uma URL para a próxima página de resultados. Você pode usar o parâmetro de consulta `$top` para especificar o número de itens na página.</span><span class="sxs-lookup"><span data-stu-id="071e1-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="071e1-141">Pesquisando itens que um usuário pode acessar</span><span class="sxs-lookup"><span data-stu-id="071e1-141">Searching for items a user can access</span></span>

<span data-ttu-id="071e1-p106">Além de procurar itens em uma unidade, seu aplicativo pode pesquisar amplamente para incluir itens compartilhados com o usuário atual. Para ampliar o escopo da pesquisa, use o método **search** no recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="071e1-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="071e1-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="071e1-144">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="071e1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="071e1-145">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```http
GET /me/drive/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="071e1-146">C#</span><span class="sxs-lookup"><span data-stu-id="071e1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="071e1-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="071e1-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="071e1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="071e1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="071e1-149">Java</span><span class="sxs-lookup"><span data-stu-id="071e1-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="071e1-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="071e1-150">Response</span></span>

<span data-ttu-id="071e1-p107">As respostas ao pesquisar por meio do recurso **drive** podem incluir itens fora da unidade (itens compartilhados com o usuário atual). Estes itens incluirão a faceta [**remoteItem**](../resources/remoteitem.md) para indicar que estão armazenados fora da unidade de destino.</span><span class="sxs-lookup"><span data-stu-id="071e1-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "parentReference": { "driveId": "s!1020101jlkjl12lx" } }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="071e1-153">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="071e1-153">Error responses</span></span>

<span data-ttu-id="071e1-154">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="071e1-154">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
} -->
