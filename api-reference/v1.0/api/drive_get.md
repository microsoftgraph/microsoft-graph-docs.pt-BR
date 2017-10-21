---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter Unidade
ms.openlocfilehash: 91a140dbcb1550bc850656452a6fa24a84dd5500
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="get-drive"></a><span data-ttu-id="e987c-102">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="e987c-102">Get Drive</span></span>

<span data-ttu-id="e987c-103">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="e987c-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="e987c-104">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e987c-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="e987c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e987c-105">Permissions</span></span>

<span data-ttu-id="e987c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e987c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e987c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e987c-108">Permission type</span></span>      | <span data-ttu-id="e987c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e987c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e987c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e987c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e987c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e987c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e987c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e987c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e987c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e987c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e987c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e987c-114">Application</span></span> | <span data-ttu-id="e987c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e987c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="e987c-116">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="e987c-116">Get a user's OneDrive</span></span>

<span data-ttu-id="e987c-117">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="e987c-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="e987c-118">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="e987c-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e987c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="e987c-120">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="e987c-120">Get a user's OneDrive</span></span>

<span data-ttu-id="e987c-121">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="e987c-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="e987c-122">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="e987c-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e987c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e987c-124">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e987c-124">Path parameters</span></span>

| <span data-ttu-id="e987c-125">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e987c-125">Parameter name</span></span> | <span data-ttu-id="e987c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="e987c-126">Value</span></span>  | <span data-ttu-id="e987c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e987c-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e987c-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="e987c-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="e987c-129">string</span><span class="sxs-lookup"><span data-stu-id="e987c-129">string</span></span> | <span data-ttu-id="e987c-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e987c-130">Required.</span></span> <span data-ttu-id="e987c-131">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e987c-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="e987c-132">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="e987c-132">Get the document library associated with a group</span></span>

<span data-ttu-id="e987c-133">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="e987c-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="e987c-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e987c-135">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e987c-135">Path parameters</span></span>

| <span data-ttu-id="e987c-136">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e987c-136">Parameter name</span></span> | <span data-ttu-id="e987c-137">Valor</span><span class="sxs-lookup"><span data-stu-id="e987c-137">Value</span></span>  | <span data-ttu-id="e987c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e987c-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e987c-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="e987c-139">_groupId_</span></span>      | <span data-ttu-id="e987c-140">string</span><span class="sxs-lookup"><span data-stu-id="e987c-140">string</span></span> | <span data-ttu-id="e987c-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e987c-141">Required.</span></span> <span data-ttu-id="e987c-142">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="e987c-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="e987c-143">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="e987c-143">Get the document library for a site</span></span>

<span data-ttu-id="e987c-144">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="e987c-144">To access a [Group's](../resources/site.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="e987c-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="e987c-146">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e987c-146">Path parameters</span></span>

| <span data-ttu-id="e987c-147">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e987c-147">Parameter name</span></span> | <span data-ttu-id="e987c-148">Valor</span><span class="sxs-lookup"><span data-stu-id="e987c-148">Value</span></span>  | <span data-ttu-id="e987c-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="e987c-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e987c-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="e987c-150">_siteId_</span></span>       | <span data-ttu-id="e987c-151">string</span><span class="sxs-lookup"><span data-stu-id="e987c-151">string</span></span> | <span data-ttu-id="e987c-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e987c-152">Required.</span></span> <span data-ttu-id="e987c-153">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="e987c-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="e987c-154">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="e987c-154">Get a drive by ID</span></span>

<span data-ttu-id="e987c-155">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="e987c-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="e987c-156">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="e987c-157">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e987c-157">Path parameters</span></span>

| <span data-ttu-id="e987c-158">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e987c-158">Parameter name</span></span> | <span data-ttu-id="e987c-159">Valor</span><span class="sxs-lookup"><span data-stu-id="e987c-159">Value</span></span>  | <span data-ttu-id="e987c-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="e987c-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e987c-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="e987c-161">_drive-id_</span></span>      | <span data-ttu-id="e987c-162">string</span><span class="sxs-lookup"><span data-stu-id="e987c-162">string</span></span> | <span data-ttu-id="e987c-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e987c-163">Required.</span></span> <span data-ttu-id="e987c-164">O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="e987c-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e987c-165">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e987c-165">Optional query parameters</span></span>

<span data-ttu-id="e987c-166">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e987c-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="e987c-167">Resposta HTTP</span><span class="sxs-lookup"><span data-stu-id="e987c-167">HTTP response</span></span>

<span data-ttu-id="e987c-168">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e987c-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="e987c-169">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="e987c-169">Error response codes</span></span>

<span data-ttu-id="e987c-170">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="e987c-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: ../../../concepts/query_parameters.md

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
