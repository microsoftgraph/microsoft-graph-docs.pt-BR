---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 47d068dd00223513ad0f49a784916e8a8185ea91
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466482"
---
# <a name="get-drive"></a><span data-ttu-id="1a252-102">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="1a252-102">Get Drive</span></span>

<span data-ttu-id="1a252-103">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="1a252-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="1a252-104">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1a252-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a252-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a252-105">Permissions</span></span>

<span data-ttu-id="1a252-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a252-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a252-108">Permission type</span></span>      | <span data-ttu-id="1a252-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a252-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a252-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a252-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a252-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a252-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a252-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a252-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a252-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a252-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a252-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a252-114">Application</span></span> | <span data-ttu-id="1a252-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a252-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="1a252-116">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="1a252-116">Get current user's OneDrive</span></span>

<span data-ttu-id="1a252-117">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="1a252-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="1a252-118">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="1a252-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a252-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a252-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a252-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1a252-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a252-121">C#</span><span class="sxs-lookup"><span data-stu-id="1a252-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a252-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a252-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="1a252-123">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="1a252-123">Get a user's OneDrive</span></span>

<span data-ttu-id="1a252-124">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="1a252-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="1a252-125">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="1a252-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a252-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a252-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a252-127">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1a252-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a252-128">C#</span><span class="sxs-lookup"><span data-stu-id="1a252-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a252-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a252-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="1a252-130">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1a252-130">Path parameters</span></span>

| <span data-ttu-id="1a252-131">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a252-131">Parameter name</span></span> | <span data-ttu-id="1a252-132">Valor</span><span class="sxs-lookup"><span data-stu-id="1a252-132">Value</span></span>  | <span data-ttu-id="1a252-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a252-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="1a252-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="1a252-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="1a252-135">string</span><span class="sxs-lookup"><span data-stu-id="1a252-135">string</span></span> | <span data-ttu-id="1a252-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a252-136">Required.</span></span> <span data-ttu-id="1a252-137">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1a252-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="1a252-138">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="1a252-138">Get the document library associated with a group</span></span>

<span data-ttu-id="1a252-139">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="1a252-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a252-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a252-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a252-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1a252-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a252-142">C#</span><span class="sxs-lookup"><span data-stu-id="1a252-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a252-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a252-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="1a252-144">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1a252-144">Path parameters</span></span>

| <span data-ttu-id="1a252-145">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a252-145">Parameter name</span></span> | <span data-ttu-id="1a252-146">Valor</span><span class="sxs-lookup"><span data-stu-id="1a252-146">Value</span></span>  | <span data-ttu-id="1a252-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a252-147">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="1a252-148">_groupId_</span><span class="sxs-lookup"><span data-stu-id="1a252-148">_groupId_</span></span>      | <span data-ttu-id="1a252-149">string</span><span class="sxs-lookup"><span data-stu-id="1a252-149">string</span></span> | <span data-ttu-id="1a252-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a252-150">Required.</span></span> <span data-ttu-id="1a252-151">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="1a252-151">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="1a252-152">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="1a252-152">Get the document library for a site</span></span>

<span data-ttu-id="1a252-153">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="1a252-153">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a252-154">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a252-154">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a252-155">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1a252-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a252-156">C#</span><span class="sxs-lookup"><span data-stu-id="1a252-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a252-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a252-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="1a252-158">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1a252-158">Path parameters</span></span>

| <span data-ttu-id="1a252-159">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a252-159">Parameter name</span></span> | <span data-ttu-id="1a252-160">Valor</span><span class="sxs-lookup"><span data-stu-id="1a252-160">Value</span></span>  | <span data-ttu-id="1a252-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a252-161">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="1a252-162">_siteId_</span><span class="sxs-lookup"><span data-stu-id="1a252-162">_siteId_</span></span>       | <span data-ttu-id="1a252-163">string</span><span class="sxs-lookup"><span data-stu-id="1a252-163">string</span></span> | <span data-ttu-id="1a252-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a252-164">Required.</span></span> <span data-ttu-id="1a252-165">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="1a252-165">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="1a252-166">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="1a252-166">Get a drive by ID</span></span>

<span data-ttu-id="1a252-167">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="1a252-167">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a252-168">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a252-168">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="1a252-169">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1a252-169">Path parameters</span></span>

| <span data-ttu-id="1a252-170">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a252-170">Parameter name</span></span> | <span data-ttu-id="1a252-171">Valor</span><span class="sxs-lookup"><span data-stu-id="1a252-171">Value</span></span>  | <span data-ttu-id="1a252-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a252-172">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="1a252-173">_driveId_</span><span class="sxs-lookup"><span data-stu-id="1a252-173">_driveId_</span></span>      | <span data-ttu-id="1a252-174">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a252-174">string</span></span> | <span data-ttu-id="1a252-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="1a252-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1a252-177">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a252-177">Optional query parameters</span></span>

<span data-ttu-id="1a252-178">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a252-178">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="1a252-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a252-179">Response</span></span>

<span data-ttu-id="1a252-180">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a252-180">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a252-181">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1a252-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a252-182">C#</span><span class="sxs-lookup"><span data-stu-id="1a252-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a252-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a252-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="1a252-184">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="1a252-184">Error response codes</span></span>

<span data-ttu-id="1a252-185">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="1a252-185">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
