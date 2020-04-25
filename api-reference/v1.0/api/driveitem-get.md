---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Priority
ms.prod: sharepoint
description: Recupere os metadados de um DriveItem em um Drive por ID ou por caminho do sistema de arquivos.
doc_type: apiPageType
ms.openlocfilehash: ec9c739a0f9426f4876c3b4419b0bbeda66e4a26
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806529"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="8add6-103">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="8add6-103">Get a DriveItem resource</span></span>

<span data-ttu-id="8add6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8add6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8add6-105">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="8add6-105">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8add6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8add6-106">Permissions</span></span>

<span data-ttu-id="8add6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8add6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8add6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8add6-109">Permission type</span></span>      | <span data-ttu-id="8add6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8add6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8add6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8add6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8add6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8add6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8add6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8add6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8add6-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8add6-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8add6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8add6-115">Application</span></span> | <span data-ttu-id="8add6-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8add6-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8add6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8add6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{site-id}/drive/items/{item-id}
GET /sites/{site-id}/drive/root:/{item-path}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem
GET /users/{user-id}/drive/items/{item-id}
GET /users/{user-id}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8add6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8add6-118">Optional query parameters</span></span>

<span data-ttu-id="8add6-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8add6-119">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="8add6-120">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="8add6-120">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="8add6-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8add6-121">Optional request headers</span></span>

| <span data-ttu-id="8add6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8add6-122">Name</span></span>          | <span data-ttu-id="8add6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8add6-123">Value</span></span>  | <span data-ttu-id="8add6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8add6-124">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8add6-125">if-none-match</span><span class="sxs-lookup"><span data-stu-id="8add6-125">if-none-match</span></span> | <span data-ttu-id="8add6-126">String</span><span class="sxs-lookup"><span data-stu-id="8add6-126">String</span></span> | <span data-ttu-id="8add6-127">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="8add6-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="8add6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8add6-128">Response</span></span>

<span data-ttu-id="8add6-129">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8add6-129">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8add6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8add6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8add6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8add6-131">Request</span></span>

<span data-ttu-id="8add6-132">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="8add6-132">Here is an example of the request to the root folder of the user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="8add6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8add6-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/root
```
# <a name="c"></a>[<span data-ttu-id="8add6-134">C#</span><span class="sxs-lookup"><span data-stu-id="8add6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8add6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8add6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8add6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8add6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8add6-137">Java</span><span class="sxs-lookup"><span data-stu-id="8add6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8add6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8add6-138">Response</span></span>

<span data-ttu-id="8add6-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8add6-139">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="8add6-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="8add6-140">Remarks</span></span>

<span data-ttu-id="8add6-141">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="8add6-141">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
} -->
