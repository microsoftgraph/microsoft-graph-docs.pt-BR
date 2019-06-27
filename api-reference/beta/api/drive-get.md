---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e099f6ba8bef07cba3406e2deb2cbb8961aa227
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260351"
---
# <a name="get-drive"></a><span data-ttu-id="12deb-102">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="12deb-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12deb-103">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="12deb-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="12deb-104">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="12deb-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="12deb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="12deb-105">Permissions</span></span>

<span data-ttu-id="12deb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12deb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12deb-108">Permission type</span></span>      | <span data-ttu-id="12deb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12deb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12deb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12deb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12deb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12deb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="12deb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12deb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12deb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12deb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="12deb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12deb-114">Application</span></span> | <span data-ttu-id="12deb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12deb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="12deb-116">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="12deb-116">Get current user's OneDrive</span></span>

<span data-ttu-id="12deb-117">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="12deb-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="12deb-118">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="12deb-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="12deb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12deb-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="12deb-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12deb-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12deb-121">C#</span><span class="sxs-lookup"><span data-stu-id="12deb-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12deb-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="12deb-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12deb-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12deb-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="12deb-124">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="12deb-124">Get a user's OneDrive</span></span>

<span data-ttu-id="12deb-125">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="12deb-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="12deb-126">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="12deb-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="12deb-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12deb-127">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="12deb-128">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12deb-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12deb-129">C#</span><span class="sxs-lookup"><span data-stu-id="12deb-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12deb-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="12deb-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12deb-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12deb-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="12deb-132">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="12deb-132">Path parameters</span></span>

| <span data-ttu-id="12deb-133">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="12deb-133">Parameter name</span></span> | <span data-ttu-id="12deb-134">Valor</span><span class="sxs-lookup"><span data-stu-id="12deb-134">Value</span></span>  | <span data-ttu-id="12deb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="12deb-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="12deb-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="12deb-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="12deb-137">string</span><span class="sxs-lookup"><span data-stu-id="12deb-137">string</span></span> | <span data-ttu-id="12deb-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12deb-138">Required.</span></span> <span data-ttu-id="12deb-139">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="12deb-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="12deb-140">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="12deb-140">Get the document library associated with a group</span></span>

<span data-ttu-id="12deb-141">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="12deb-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="12deb-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12deb-142">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="12deb-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12deb-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12deb-144">C#</span><span class="sxs-lookup"><span data-stu-id="12deb-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12deb-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="12deb-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12deb-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12deb-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="12deb-147">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="12deb-147">Path parameters</span></span>

| <span data-ttu-id="12deb-148">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="12deb-148">Parameter name</span></span> | <span data-ttu-id="12deb-149">Valor</span><span class="sxs-lookup"><span data-stu-id="12deb-149">Value</span></span>  | <span data-ttu-id="12deb-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="12deb-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="12deb-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="12deb-151">_groupId_</span></span>      | <span data-ttu-id="12deb-152">string</span><span class="sxs-lookup"><span data-stu-id="12deb-152">string</span></span> | <span data-ttu-id="12deb-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12deb-153">Required.</span></span> <span data-ttu-id="12deb-154">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="12deb-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="12deb-155">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="12deb-155">Get the document library for a site</span></span>

<span data-ttu-id="12deb-156">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="12deb-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="12deb-157">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12deb-157">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="12deb-158">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12deb-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12deb-159">C#</span><span class="sxs-lookup"><span data-stu-id="12deb-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12deb-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="12deb-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12deb-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12deb-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="12deb-162">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="12deb-162">Path parameters</span></span>

| <span data-ttu-id="12deb-163">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="12deb-163">Parameter name</span></span> | <span data-ttu-id="12deb-164">Valor</span><span class="sxs-lookup"><span data-stu-id="12deb-164">Value</span></span>  | <span data-ttu-id="12deb-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="12deb-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="12deb-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="12deb-166">_siteId_</span></span>       | <span data-ttu-id="12deb-167">string</span><span class="sxs-lookup"><span data-stu-id="12deb-167">string</span></span> | <span data-ttu-id="12deb-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12deb-168">Required.</span></span> <span data-ttu-id="12deb-169">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="12deb-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="12deb-170">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="12deb-170">Get a drive by ID</span></span>

<span data-ttu-id="12deb-171">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="12deb-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="12deb-172">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12deb-172">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="12deb-173">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="12deb-173">Path parameters</span></span>

| <span data-ttu-id="12deb-174">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="12deb-174">Parameter name</span></span> | <span data-ttu-id="12deb-175">Valor</span><span class="sxs-lookup"><span data-stu-id="12deb-175">Value</span></span>  | <span data-ttu-id="12deb-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="12deb-176">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="12deb-177">_driveId_</span><span class="sxs-lookup"><span data-stu-id="12deb-177">_driveId_</span></span>      | <span data-ttu-id="12deb-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12deb-178">string</span></span> | <span data-ttu-id="12deb-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="12deb-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="12deb-181">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12deb-181">Optional query parameters</span></span>

<span data-ttu-id="12deb-182">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12deb-182">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="12deb-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="12deb-183">Response</span></span>

<span data-ttu-id="12deb-184">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12deb-184">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id",] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="12deb-185">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12deb-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12deb-186">C#</span><span class="sxs-lookup"><span data-stu-id="12deb-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12deb-187">Javascript</span><span class="sxs-lookup"><span data-stu-id="12deb-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12deb-188">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12deb-188">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="12deb-189">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="12deb-189">Error response codes</span></span>

<span data-ttu-id="12deb-190">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="12deb-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
