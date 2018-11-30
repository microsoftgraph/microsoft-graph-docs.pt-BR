---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Carregar arquivos pequenos
ms.openlocfilehash: 8a31454e67b1d502721db83a38c733a5235cb8c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036544"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="563c0-102">Carregar ou substituir o conteúdo de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="563c0-102">Upload or replace the contents of a DriveItem</span></span>

> <span data-ttu-id="563c0-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="563c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="563c0-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="563c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="563c0-p102">A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.</span><span class="sxs-lookup"><span data-stu-id="563c0-p102">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="563c0-107">Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="563c0-107">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="563c0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="563c0-108">Permissions</span></span>

<span data-ttu-id="563c0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="563c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="563c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="563c0-111">Permission type</span></span>      | <span data-ttu-id="563c0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="563c0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="563c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="563c0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="563c0-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563c0-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="563c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="563c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="563c0-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563c0-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="563c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="563c0-117">Application</span></span> | <span data-ttu-id="563c0-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563c0-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="563c0-119">Solicitação HTTP (para substituir um item existente)</span><span class="sxs-lookup"><span data-stu-id="563c0-119">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="563c0-120">Solicitação HTTP (para carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="563c0-120">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="563c0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="563c0-121">Request body</span></span>

<span data-ttu-id="563c0-122">O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="563c0-122">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="563c0-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="563c0-123">Response</span></span>

<span data-ttu-id="563c0-124">Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="563c0-124">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="563c0-125">Exemplo (carregar um novo arquivo)</span><span class="sxs-lookup"><span data-stu-id="563c0-125">Example (upload a new file)</span></span>

<span data-ttu-id="563c0-126">Este exemplo carrega a cadeia de caracteres "O conteúdo do arquivo fica aqui".</span><span class="sxs-lookup"><span data-stu-id="563c0-126">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="563c0-127">para um arquivo na unidade do usuário conectado em FolderA chamado FileB.txt.</span><span class="sxs-lookup"><span data-stu-id="563c0-127">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="563c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="563c0-128">Response</span></span>

<span data-ttu-id="563c0-129">Se for bem-sucedido, esse método retornará um [recurso driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="563c0-129">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="563c0-130">Exemplo (atualizando um arquivo existente)</span><span class="sxs-lookup"><span data-stu-id="563c0-130">Example (updating an existing file)</span></span>

<span data-ttu-id="563c0-131">Este exemplo substitui o conteúdo de um arquivo com uma ID conhecida.</span><span class="sxs-lookup"><span data-stu-id="563c0-131">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="563c0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="563c0-132">Response</span></span>

<span data-ttu-id="563c0-133">Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="563c0-133">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="563c0-134">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="563c0-134">Error responses</span></span>

<span data-ttu-id="563c0-135">Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="563c0-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
