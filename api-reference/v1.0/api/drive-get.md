---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Priority
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso Drive.
doc_type: apiPageType
ms.openlocfilehash: 5118dedfde1126a01d445dd5a4c566ac8738902a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365017"
---
# <a name="get-drive"></a><span data-ttu-id="58bf0-103">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="58bf0-103">Get Drive</span></span>

<span data-ttu-id="58bf0-104">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="58bf0-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="58bf0-105">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58bf0-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="58bf0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58bf0-106">Permissions</span></span>

<span data-ttu-id="58bf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58bf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58bf0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58bf0-109">Permission type</span></span>      | <span data-ttu-id="58bf0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58bf0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58bf0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58bf0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58bf0-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf0-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58bf0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58bf0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58bf0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="58bf0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58bf0-115">Application</span></span> | <span data-ttu-id="58bf0-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf0-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="58bf0-117">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="58bf0-117">Get current user's OneDrive</span></span>

<span data-ttu-id="58bf0-118">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="58bf0-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="58bf0-119">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="58bf0-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="58bf0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf0-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf0-122">C#</span><span class="sxs-lookup"><span data-stu-id="58bf0-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf0-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf0-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf0-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf0-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf0-125">Java</span><span class="sxs-lookup"><span data-stu-id="58bf0-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="58bf0-126">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="58bf0-126">Get a user's OneDrive</span></span>

<span data-ttu-id="58bf0-127">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="58bf0-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="58bf0-128">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="58bf0-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="58bf0-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf0-131">C#</span><span class="sxs-lookup"><span data-stu-id="58bf0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf0-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf0-134">Java</span><span class="sxs-lookup"><span data-stu-id="58bf0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="58bf0-135">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="58bf0-135">Path parameters</span></span>

| <span data-ttu-id="58bf0-136">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="58bf0-136">Parameter name</span></span> | <span data-ttu-id="58bf0-137">Valor</span><span class="sxs-lookup"><span data-stu-id="58bf0-137">Value</span></span>  | <span data-ttu-id="58bf0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bf0-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="58bf0-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="58bf0-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="58bf0-140">string</span><span class="sxs-lookup"><span data-stu-id="58bf0-140">string</span></span> | <span data-ttu-id="58bf0-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bf0-141">Required.</span></span> <span data-ttu-id="58bf0-142">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="58bf0-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="58bf0-143">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="58bf0-143">Get the document library associated with a group</span></span>

<span data-ttu-id="58bf0-144">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="58bf0-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="58bf0-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-146">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf0-147">C#</span><span class="sxs-lookup"><span data-stu-id="58bf0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf0-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf0-150">Java</span><span class="sxs-lookup"><span data-stu-id="58bf0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="58bf0-151">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="58bf0-151">Path parameters</span></span>

| <span data-ttu-id="58bf0-152">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="58bf0-152">Parameter name</span></span> | <span data-ttu-id="58bf0-153">Valor</span><span class="sxs-lookup"><span data-stu-id="58bf0-153">Value</span></span>  | <span data-ttu-id="58bf0-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bf0-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="58bf0-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="58bf0-155">_groupId_</span></span>      | <span data-ttu-id="58bf0-156">string</span><span class="sxs-lookup"><span data-stu-id="58bf0-156">string</span></span> | <span data-ttu-id="58bf0-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bf0-157">Required.</span></span> <span data-ttu-id="58bf0-158">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="58bf0-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="58bf0-159">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="58bf0-159">Get the document library for a site</span></span>

<span data-ttu-id="58bf0-160">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="58bf0-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="58bf0-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf0-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-162">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf0-163">C#</span><span class="sxs-lookup"><span data-stu-id="58bf0-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf0-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf0-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf0-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf0-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf0-166">Java</span><span class="sxs-lookup"><span data-stu-id="58bf0-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="58bf0-167">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="58bf0-167">Path parameters</span></span>

| <span data-ttu-id="58bf0-168">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="58bf0-168">Parameter name</span></span> | <span data-ttu-id="58bf0-169">Valor</span><span class="sxs-lookup"><span data-stu-id="58bf0-169">Value</span></span>  | <span data-ttu-id="58bf0-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bf0-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="58bf0-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="58bf0-171">_siteId_</span></span>       | <span data-ttu-id="58bf0-172">string</span><span class="sxs-lookup"><span data-stu-id="58bf0-172">string</span></span> | <span data-ttu-id="58bf0-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bf0-173">Required.</span></span> <span data-ttu-id="58bf0-174">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="58bf0-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="58bf0-175">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="58bf0-175">Get a drive by ID</span></span>

<span data-ttu-id="58bf0-176">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="58bf0-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="58bf0-177">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf0-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf0-178">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf0-179">C#</span><span class="sxs-lookup"><span data-stu-id="58bf0-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf0-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf0-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf0-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf0-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf0-182">Java</span><span class="sxs-lookup"><span data-stu-id="58bf0-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="58bf0-183">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="58bf0-183">Path parameters</span></span>

| <span data-ttu-id="58bf0-184">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="58bf0-184">Parameter name</span></span> | <span data-ttu-id="58bf0-185">Valor</span><span class="sxs-lookup"><span data-stu-id="58bf0-185">Value</span></span>  | <span data-ttu-id="58bf0-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bf0-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="58bf0-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="58bf0-187">_driveId_</span></span>      | <span data-ttu-id="58bf0-188">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58bf0-188">string</span></span> | <span data-ttu-id="58bf0-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="58bf0-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="58bf0-191">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58bf0-191">Optional query parameters</span></span>

<span data-ttu-id="58bf0-192">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58bf0-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="58bf0-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bf0-193">Response</span></span>

<span data-ttu-id="58bf0-194">Cada um desses métodos retorna um [Recurso de Unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58bf0-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="58bf0-195">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="58bf0-195">Error response codes</span></span>

<span data-ttu-id="58bf0-196">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="58bf0-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
