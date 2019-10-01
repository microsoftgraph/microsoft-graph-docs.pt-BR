---
author: JeremyKelley
description: Recupere os metadados de um DriveItem em um Drive por ID ou caminho do sistema de arquivos.
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0f7aee77c2a3a97bef8c67789d2a88d14ad0a62f
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333210"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="d6440-103">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="d6440-103">Get a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6440-104">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d6440-104">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6440-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6440-105">Permissions</span></span>

<span data-ttu-id="d6440-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6440-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6440-108">Permission type</span></span>      | <span data-ttu-id="d6440-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6440-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6440-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6440-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6440-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6440-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6440-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6440-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6440-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6440-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6440-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6440-114">Application</span></span> | <span data-ttu-id="d6440-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6440-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6440-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6440-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6440-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6440-117">Optional query parameters</span></span>

<span data-ttu-id="d6440-118">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6440-118">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="d6440-119">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="d6440-119">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<span data-ttu-id="d6440-120">Você também pode usar o `includeDeletedItems=true` parâmetro de consulta para retornar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="d6440-120">You can also use the `includeDeletedItems=true` query parameter to return deleted items.</span></span>
<span data-ttu-id="d6440-121">Esse parâmetro de consulta só é válido ao direcionar um [driveItem](../resources/driveitem.md) por ID e, caso contrário, será ignorado.</span><span class="sxs-lookup"><span data-stu-id="d6440-121">This query parameter is only valid when targeting a [driveItem](../resources/driveitem.md) by ID, and otherwise will be ignored.</span></span>
<span data-ttu-id="d6440-122">No momento, isso só tem suporte no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="d6440-122">This is currently only supported on OneDrive Personal.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="d6440-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d6440-123">Optional request headers</span></span>

| <span data-ttu-id="d6440-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d6440-124">Name</span></span>          | <span data-ttu-id="d6440-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d6440-125">Value</span></span>  | <span data-ttu-id="d6440-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6440-126">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d6440-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="d6440-127">if-none-match</span></span> | <span data-ttu-id="d6440-128">String</span><span class="sxs-lookup"><span data-stu-id="d6440-128">String</span></span> | <span data-ttu-id="d6440-129">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="d6440-129">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="d6440-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6440-130">Response</span></span>

<span data-ttu-id="d6440-131">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6440-131">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6440-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6440-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6440-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6440-133">Request</span></span>

<span data-ttu-id="d6440-134">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6440-134">Here is an example of the request to the root folder of the user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d6440-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6440-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```msgraph-interactive
GET /me/drive/root
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6440-136">C#</span><span class="sxs-lookup"><span data-stu-id="d6440-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6440-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6440-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6440-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6440-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d6440-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6440-139">Response</span></span>

<span data-ttu-id="d6440-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6440-140">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a><span data-ttu-id="d6440-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6440-141">Remarks</span></span>

<span data-ttu-id="d6440-142">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="d6440-142">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
}
-->
