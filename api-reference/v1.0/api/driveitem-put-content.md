---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Carregar arquivos pequenos
localization_priority: Priority
ms.prod: sharepoint
description: 'A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. '
doc_type: apiPageType
ms.openlocfilehash: 0653cf59ca3c67a3a941b2df0d654439da950bc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015359"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="270a3-103">Carregar ou substituir o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="270a3-103">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="270a3-p101">A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.</span><span class="sxs-lookup"><span data-stu-id="270a3-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="270a3-106">Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="270a3-106">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="270a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="270a3-107">Permissions</span></span>

<span data-ttu-id="270a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="270a3-110">Permission type</span></span>      | <span data-ttu-id="270a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="270a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="270a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="270a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="270a3-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270a3-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="270a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="270a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="270a3-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270a3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="270a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="270a3-116">Application</span></span> | <span data-ttu-id="270a3-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270a3-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="270a3-118">Solicitação HTTP (para substituir um item existente)</span><span class="sxs-lookup"><span data-stu-id="270a3-118">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="270a3-119">Solicitação HTTP (para carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="270a3-119">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="270a3-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="270a3-120">Request body</span></span>

<span data-ttu-id="270a3-121">O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="270a3-121">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="270a3-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="270a3-122">Response</span></span>

<span data-ttu-id="270a3-123">Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="270a3-123">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="270a3-124">Exemplo (carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="270a3-124">Example (upload a new file)</span></span>

<span data-ttu-id="270a3-125">Este exemplo carrega a cadeia de caracteres "O conteúdo do arquivo fica aqui".</span><span class="sxs-lookup"><span data-stu-id="270a3-125">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="270a3-126">para um arquivo na unidade do usuário conectado em FolderA chamado FileB.txt.</span><span class="sxs-lookup"><span data-stu-id="270a3-126">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="270a3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="270a3-127">Response</span></span>

<span data-ttu-id="270a3-128">Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="270a3-128">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="270a3-129">Exemplo (atualizando um arquivo existente)</span><span class="sxs-lookup"><span data-stu-id="270a3-129">Example (updating an existing file)</span></span>

<span data-ttu-id="270a3-130">Este exemplo substitui o conteúdo de um arquivo com uma ID conhecida.</span><span class="sxs-lookup"><span data-stu-id="270a3-130">This example replaces the contents of a file with a known ID.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="270a3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="270a3-131">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="270a3-132">C#</span><span class="sxs-lookup"><span data-stu-id="270a3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="270a3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="270a3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="270a3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="270a3-134">Response</span></span>

<span data-ttu-id="270a3-135">Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="270a3-135">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="270a3-136">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="270a3-136">Error responses</span></span>

<span data-ttu-id="270a3-137">Confira [Respostas de erro][error-response] para saber mais detalhes sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="270a3-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
} -->
