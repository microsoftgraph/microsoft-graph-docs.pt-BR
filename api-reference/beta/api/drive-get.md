---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso Drive.
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0381e4cffc910c9169e57bdd0655041f4b9d3f0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324451"
---
# <a name="get-drive"></a><span data-ttu-id="d5e20-103">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="d5e20-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5e20-104">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="d5e20-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="d5e20-105">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d5e20-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e20-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5e20-106">Permissions</span></span>

<span data-ttu-id="d5e20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5e20-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5e20-109">Permission type</span></span>      | <span data-ttu-id="d5e20-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5e20-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5e20-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5e20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5e20-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5e20-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5e20-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5e20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e20-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5e20-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5e20-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5e20-115">Application</span></span> | <span data-ttu-id="d5e20-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5e20-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="d5e20-117">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="d5e20-117">Get current user's OneDrive</span></span>

<span data-ttu-id="d5e20-118">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="d5e20-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="d5e20-119">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="d5e20-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d5e20-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5e20-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5e20-122">C#</span><span class="sxs-lookup"><span data-stu-id="d5e20-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5e20-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e20-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5e20-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5e20-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5e20-125">Java</span><span class="sxs-lookup"><span data-stu-id="d5e20-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="d5e20-126">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="d5e20-126">Get a user's OneDrive</span></span>

<span data-ttu-id="d5e20-127">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="d5e20-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="d5e20-128">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="d5e20-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="d5e20-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5e20-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5e20-131">C#</span><span class="sxs-lookup"><span data-stu-id="d5e20-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5e20-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e20-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5e20-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5e20-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5e20-134">Java</span><span class="sxs-lookup"><span data-stu-id="d5e20-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="d5e20-135">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d5e20-135">Path parameters</span></span>

| <span data-ttu-id="d5e20-136">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5e20-136">Parameter name</span></span> | <span data-ttu-id="d5e20-137">Valor</span><span class="sxs-lookup"><span data-stu-id="d5e20-137">Value</span></span>  | <span data-ttu-id="d5e20-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e20-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d5e20-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="d5e20-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="d5e20-140">string</span><span class="sxs-lookup"><span data-stu-id="d5e20-140">string</span></span> | <span data-ttu-id="d5e20-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5e20-141">Required.</span></span> <span data-ttu-id="d5e20-142">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d5e20-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="d5e20-143">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="d5e20-143">Get the document library associated with a group</span></span>

<span data-ttu-id="d5e20-144">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="d5e20-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="d5e20-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5e20-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5e20-147">C#</span><span class="sxs-lookup"><span data-stu-id="d5e20-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5e20-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e20-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5e20-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5e20-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5e20-150">Java</span><span class="sxs-lookup"><span data-stu-id="d5e20-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="d5e20-151">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d5e20-151">Path parameters</span></span>

| <span data-ttu-id="d5e20-152">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5e20-152">Parameter name</span></span> | <span data-ttu-id="d5e20-153">Valor</span><span class="sxs-lookup"><span data-stu-id="d5e20-153">Value</span></span>  | <span data-ttu-id="d5e20-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e20-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d5e20-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="d5e20-155">_groupId_</span></span>      | <span data-ttu-id="d5e20-156">string</span><span class="sxs-lookup"><span data-stu-id="d5e20-156">string</span></span> | <span data-ttu-id="d5e20-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5e20-157">Required.</span></span> <span data-ttu-id="d5e20-158">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="d5e20-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="d5e20-159">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="d5e20-159">Get the document library for a site</span></span>

<span data-ttu-id="d5e20-160">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="d5e20-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="d5e20-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5e20-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-162">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5e20-163">C#</span><span class="sxs-lookup"><span data-stu-id="d5e20-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5e20-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e20-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5e20-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5e20-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5e20-166">Java</span><span class="sxs-lookup"><span data-stu-id="d5e20-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="d5e20-167">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d5e20-167">Path parameters</span></span>

| <span data-ttu-id="d5e20-168">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5e20-168">Parameter name</span></span> | <span data-ttu-id="d5e20-169">Valor</span><span class="sxs-lookup"><span data-stu-id="d5e20-169">Value</span></span>  | <span data-ttu-id="d5e20-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e20-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d5e20-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="d5e20-171">_siteId_</span></span>       | <span data-ttu-id="d5e20-172">string</span><span class="sxs-lookup"><span data-stu-id="d5e20-172">string</span></span> | <span data-ttu-id="d5e20-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5e20-173">Required.</span></span> <span data-ttu-id="d5e20-174">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="d5e20-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="d5e20-175">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="d5e20-175">Get a drive by ID</span></span>

<span data-ttu-id="d5e20-176">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="d5e20-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="d5e20-177">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5e20-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e20-178">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5e20-179">C#</span><span class="sxs-lookup"><span data-stu-id="d5e20-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5e20-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e20-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5e20-181">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5e20-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5e20-182">Java</span><span class="sxs-lookup"><span data-stu-id="d5e20-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="d5e20-183">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d5e20-183">Path parameters</span></span>

| <span data-ttu-id="d5e20-184">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5e20-184">Parameter name</span></span> | <span data-ttu-id="d5e20-185">Valor</span><span class="sxs-lookup"><span data-stu-id="d5e20-185">Value</span></span>  | <span data-ttu-id="d5e20-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e20-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="d5e20-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="d5e20-187">_driveId_</span></span>      | <span data-ttu-id="d5e20-188">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5e20-188">string</span></span> | <span data-ttu-id="d5e20-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="d5e20-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d5e20-191">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5e20-191">Optional query parameters</span></span>

<span data-ttu-id="d5e20-192">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5e20-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="d5e20-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5e20-193">Response</span></span>

<span data-ttu-id="d5e20-194">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5e20-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="d5e20-195">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="d5e20-195">Error response codes</span></span>

<span data-ttu-id="d5e20-196">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="d5e20-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
  ]
}
-->
