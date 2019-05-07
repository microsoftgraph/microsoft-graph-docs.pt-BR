---
title: Baixar o conteúdo de um recurso do DriveItemVersion
description: Recuperar o conteúdo de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 85ec476ae683bb670245328d4e671855b62080d9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616248"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="8fec3-103">Baixar o conteúdo de um recurso do DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="8fec3-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="8fec3-104">Recuperar o conteúdo de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8fec3-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8fec3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fec3-105">Permissions</span></span>

<span data-ttu-id="8fec3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fec3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fec3-108">Permission type</span></span>      | <span data-ttu-id="8fec3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fec3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fec3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fec3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fec3-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec3-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fec3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fec3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fec3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fec3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fec3-114">Application</span></span> | <span data-ttu-id="8fec3-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec3-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="8fec3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fec3-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="8fec3-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec3-117">Response</span></span>

<span data-ttu-id="8fec3-118">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8fec3-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="8fec3-p102">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="8fec3-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="8fec3-121">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="8fec3-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="8fec3-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fec3-122">Example</span></span>

<span data-ttu-id="8fec3-123">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="8fec3-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="8fec3-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fec3-124">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="8fec3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec3-125">Response</span></span>

<span data-ttu-id="8fec3-126">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="8fec3-126">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8fec3-127">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8fec3-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8fec3-128">Basic</span><span class="sxs-lookup"><span data-stu-id="8fec3-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-version-contents-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fec3-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fec3-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-version-contents-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="remarks"></a><span data-ttu-id="8fec3-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="8fec3-130">Remarks</span></span>

<span data-ttu-id="8fec3-131">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="8fec3-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="8fec3-132">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="8fec3-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
