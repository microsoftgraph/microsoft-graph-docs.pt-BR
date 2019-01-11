---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Carregar arquivos pequenos
localization_priority: Priority
ms.openlocfilehash: d3a1b504ae50fb09b9776e3f1eb269894d5f1167
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860323"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="715b5-102">Carregar ou substituir o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="715b5-102">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="715b5-p101">A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.</span><span class="sxs-lookup"><span data-stu-id="715b5-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="715b5-105">Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="715b5-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="715b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="715b5-106">Permissions</span></span>

<span data-ttu-id="715b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="715b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="715b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="715b5-109">Permission type</span></span>      | <span data-ttu-id="715b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="715b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="715b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="715b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="715b5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="715b5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="715b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="715b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="715b5-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="715b5-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="715b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="715b5-115">Application</span></span> | <span data-ttu-id="715b5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="715b5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="715b5-117">Solicitação HTTP (para substituir um item existente)</span><span class="sxs-lookup"><span data-stu-id="715b5-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="715b5-118">Solicitação HTTP (para carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="715b5-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="715b5-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="715b5-119">Request body</span></span>

<span data-ttu-id="715b5-120">O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="715b5-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="715b5-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="715b5-121">Response</span></span>

<span data-ttu-id="715b5-122">Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="715b5-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="715b5-123">Exemplo (carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="715b5-123">Example (upload a new file)</span></span>

<span data-ttu-id="715b5-124">Este exemplo carrega a cadeia de caracteres "O conteúdo do arquivo fica aqui".</span><span class="sxs-lookup"><span data-stu-id="715b5-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="715b5-125">para um arquivo na unidade do usuário conectado em FolderA chamado FileB.txt.</span><span class="sxs-lookup"><span data-stu-id="715b5-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="715b5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="715b5-126">Response</span></span>

<span data-ttu-id="715b5-127">Se for bem-sucedido, esse método retornará um [recurso driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="715b5-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="715b5-128">Exemplo (atualizando um arquivo existente)</span><span class="sxs-lookup"><span data-stu-id="715b5-128">Example (updating an existing file)</span></span>

<span data-ttu-id="715b5-129">Este exemplo substitui o conteúdo de um arquivo com uma ID conhecida.</span><span class="sxs-lookup"><span data-stu-id="715b5-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="715b5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="715b5-130">Response</span></span>

<span data-ttu-id="715b5-131">Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="715b5-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="715b5-132">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="715b5-132">Error responses</span></span>

<span data-ttu-id="715b5-133">Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="715b5-133">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
