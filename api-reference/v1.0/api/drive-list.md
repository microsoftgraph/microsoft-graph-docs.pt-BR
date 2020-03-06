---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar unidades
localization_priority: Priority
ms.prod: sharepoint
description: Recupera a lista de recursos Drive disponíveis para um User, Group ou Site de destino.
doc_type: apiPageType
ms.openlocfilehash: 1b99145f57617d7026f4db34cf53a75bdbf9f295
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517815"
---
# <a name="list-available-drives"></a><span data-ttu-id="e2859-103">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="e2859-103">List available drives</span></span>

<span data-ttu-id="e2859-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2859-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2859-105">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.</span><span class="sxs-lookup"><span data-stu-id="e2859-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2859-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2859-106">Permissions</span></span>

<span data-ttu-id="e2859-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2859-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2859-109">Permission type</span></span>      | <span data-ttu-id="e2859-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2859-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2859-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2859-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2859-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2859-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2859-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2859-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2859-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2859-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2859-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2859-115">Application</span></span> | <span data-ttu-id="e2859-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2859-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="e2859-117">Lista as unidades de um grupo</span><span class="sxs-lookup"><span data-stu-id="e2859-117">List a group's drives</span></span>

<span data-ttu-id="e2859-118">Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.</span><span class="sxs-lookup"><span data-stu-id="e2859-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="e2859-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2859-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e2859-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2859-120">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drives
```
# <a name="c"></a>[<span data-ttu-id="e2859-121">C#</span><span class="sxs-lookup"><span data-stu-id="e2859-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2859-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2859-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2859-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2859-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2859-124">Java</span><span class="sxs-lookup"><span data-stu-id="e2859-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="e2859-125">Lista as unidades do site</span><span class="sxs-lookup"><span data-stu-id="e2859-125">List a site's drives</span></span>

<span data-ttu-id="e2859-126">Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.</span><span class="sxs-lookup"><span data-stu-id="e2859-126">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="http"></a>[<span data-ttu-id="e2859-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2859-127">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /sites/{siteId}/drives
```
# <a name="c"></a>[<span data-ttu-id="e2859-128">C#</span><span class="sxs-lookup"><span data-stu-id="e2859-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2859-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2859-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2859-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2859-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2859-131">Java</span><span class="sxs-lookup"><span data-stu-id="e2859-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="e2859-132">Lista as unidades de um usuário</span><span class="sxs-lookup"><span data-stu-id="e2859-132">List a user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="e2859-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2859-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{userId}/drives
```
# <a name="c"></a>[<span data-ttu-id="e2859-134">C#</span><span class="sxs-lookup"><span data-stu-id="e2859-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2859-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2859-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2859-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2859-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2859-137">Java</span><span class="sxs-lookup"><span data-stu-id="e2859-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="e2859-138">Lista as unidades do usuário atual</span><span class="sxs-lookup"><span data-stu-id="e2859-138">List the current user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="e2859-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2859-139">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drives
```
# <a name="c"></a>[<span data-ttu-id="e2859-140">C#</span><span class="sxs-lookup"><span data-stu-id="e2859-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2859-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2859-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2859-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2859-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2859-143">Java</span><span class="sxs-lookup"><span data-stu-id="e2859-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="e2859-144">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e2859-144">Optional query parameters</span></span>

<span data-ttu-id="e2859-145">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="e2859-145">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="e2859-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2859-146">Response</span></span>

<span data-ttu-id="e2859-147">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2859-147">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="e2859-148">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2859-148">Remarks</span></span>

<span data-ttu-id="e2859-149">A maioria dos usuários só terá um único recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="e2859-149">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="e2859-150">Grupos e Sites podem ter vários recursos de unidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="e2859-150">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="e2859-151">Unidades com a faceta [sistema][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e2859-151">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="e2859-152">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="e2859-152">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
} -->
