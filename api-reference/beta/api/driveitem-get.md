---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 977209dba7284bb8f4f1abe5037d229f4a5a34c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945458"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="8bf57-102">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="8bf57-102">Get a DriveItem resource</span></span>

> <span data-ttu-id="8bf57-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8bf57-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bf57-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8bf57-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bf57-105">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="8bf57-105">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bf57-106">Permissions</span></span>

<span data-ttu-id="8bf57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bf57-109">Permission type</span></span>      | <span data-ttu-id="8bf57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bf57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bf57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bf57-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8bf57-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf57-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bf57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bf57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf57-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf57-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bf57-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bf57-115">Application</span></span> | <span data-ttu-id="8bf57-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf57-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bf57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bf57-117">HTTP request</span></span>

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

## <a name="optional-query-parameters"></a><span data-ttu-id="8bf57-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8bf57-118">Optional query parameters</span></span>

<span data-ttu-id="8bf57-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf57-119">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="8bf57-120">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="8bf57-120">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="8bf57-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8bf57-121">Optional request headers</span></span>

| <span data-ttu-id="8bf57-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8bf57-122">Name</span></span>          | <span data-ttu-id="8bf57-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8bf57-123">Value</span></span>  | <span data-ttu-id="8bf57-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bf57-124">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8bf57-125">if-none-match</span><span class="sxs-lookup"><span data-stu-id="8bf57-125">if-none-match</span></span> | <span data-ttu-id="8bf57-126">String</span><span class="sxs-lookup"><span data-stu-id="8bf57-126">String</span></span> | <span data-ttu-id="8bf57-127">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="8bf57-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="8bf57-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf57-128">Response</span></span>

<span data-ttu-id="8bf57-129">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf57-129">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf57-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bf57-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bf57-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf57-131">Request</span></span>

<span data-ttu-id="8bf57-132">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="8bf57-132">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="8bf57-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf57-133">Response</span></span>

<span data-ttu-id="8bf57-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf57-134">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="8bf57-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="8bf57-135">Remarks</span></span>

<span data-ttu-id="8bf57-136">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="8bf57-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
