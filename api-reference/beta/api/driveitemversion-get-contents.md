---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Baixar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 953bcb542f37bc59937a90f41dc82812ae9e691c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588184"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="e9ed8-102">Baixar o conteúdo de um recurso de DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="e9ed8-102">Download contents of a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9ed8-103">Recuperar o conteúdo de uma versão específica de um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e9ed8-103">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="e9ed8-104">**Observação:** Não há suporte para obter o conteúdo da versão atual.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-104">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="e9ed8-105">Em vez disso, use o [ponto de extremidade de conteúdo driveItem](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="e9ed8-105">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9ed8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9ed8-106">Permissions</span></span>

<span data-ttu-id="e9ed8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ed8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9ed8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9ed8-109">Permission type</span></span>      | <span data-ttu-id="e9ed8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9ed8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9ed8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9ed8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9ed8-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ed8-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9ed8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9ed8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9ed8-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ed8-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9ed8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9ed8-115">Application</span></span> | <span data-ttu-id="e9ed8-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ed8-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="e9ed8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ed8-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="e9ed8-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ed8-118">Response</span></span>

<span data-ttu-id="e9ed8-119">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-119">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="e9ed8-p103">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="e9ed8-122">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-122">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="e9ed8-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9ed8-123">Example</span></span>

<span data-ttu-id="e9ed8-124">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-124">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="e9ed8-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ed8-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="e9ed8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ed8-126">Response</span></span>

<span data-ttu-id="e9ed8-127">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-127">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ed8-128">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e9ed8-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e9ed8-129">Basic</span><span class="sxs-lookup"><span data-stu-id="e9ed8-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-version-contents-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ed8-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9ed8-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-version-contents-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="remarks"></a><span data-ttu-id="e9ed8-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="e9ed8-131">Remarks</span></span>

<span data-ttu-id="e9ed8-132">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-132">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="e9ed8-133">Quando o aplicativo recupera a lista de versões disponíveis para um arquivo, um recurso [driveItemVersion](../resources/driveitemversion.md) é retornado que fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="e9ed8-133">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
