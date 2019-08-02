---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar unidades
localization_priority: Priority
ms.prod: sharepoint
description: Recupera a lista de recursos Drive disponíveis para um User, Group ou Site de destino.
doc_type: apiPageType
ms.openlocfilehash: bd5663df534b2a56e833340c25227a7852533db9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016521"
---
# <a name="list-available-drives"></a><span data-ttu-id="b432b-103">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="b432b-103">List available drives</span></span>

<span data-ttu-id="b432b-104">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.</span><span class="sxs-lookup"><span data-stu-id="b432b-104">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b432b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b432b-105">Permissions</span></span>

<span data-ttu-id="b432b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b432b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b432b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b432b-108">Permission type</span></span>      | <span data-ttu-id="b432b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b432b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b432b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b432b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b432b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b432b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b432b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b432b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b432b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b432b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b432b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b432b-114">Application</span></span> | <span data-ttu-id="b432b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b432b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="b432b-116">Lista as unidades de um grupo</span><span class="sxs-lookup"><span data-stu-id="b432b-116">List a group's drives</span></span>

<span data-ttu-id="b432b-117">Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.</span><span class="sxs-lookup"><span data-stu-id="b432b-117">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="b432b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b432b-118">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b432b-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="b432b-119">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b432b-120">C#</span><span class="sxs-lookup"><span data-stu-id="b432b-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b432b-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="b432b-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b432b-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b432b-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b432b-123">Java</span><span class="sxs-lookup"><span data-stu-id="b432b-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="b432b-124">Lista as unidades do site</span><span class="sxs-lookup"><span data-stu-id="b432b-124">List a site's drives</span></span>

<span data-ttu-id="b432b-125">Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.</span><span class="sxs-lookup"><span data-stu-id="b432b-125">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b432b-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="b432b-126">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```http
GET /sites/{siteId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b432b-127">C#</span><span class="sxs-lookup"><span data-stu-id="b432b-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b432b-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="b432b-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b432b-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b432b-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b432b-130">Java</span><span class="sxs-lookup"><span data-stu-id="b432b-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="b432b-131">Lista as unidades de um usuário</span><span class="sxs-lookup"><span data-stu-id="b432b-131">List a user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b432b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b432b-132">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /users/{userId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b432b-133">C#</span><span class="sxs-lookup"><span data-stu-id="b432b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b432b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b432b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b432b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b432b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b432b-136">Java</span><span class="sxs-lookup"><span data-stu-id="b432b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="b432b-137">Lista as unidades do usuário atual</span><span class="sxs-lookup"><span data-stu-id="b432b-137">List the current user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b432b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b432b-138">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b432b-139">C#</span><span class="sxs-lookup"><span data-stu-id="b432b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b432b-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="b432b-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b432b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b432b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b432b-142">Java</span><span class="sxs-lookup"><span data-stu-id="b432b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="b432b-143">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b432b-143">Optional query parameters</span></span>

<span data-ttu-id="b432b-144">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="b432b-144">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="b432b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b432b-145">Response</span></span>

<span data-ttu-id="b432b-146">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b432b-146">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b432b-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="b432b-147">Remarks</span></span>

<span data-ttu-id="b432b-148">A maioria dos usuários só terá um único recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="b432b-148">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="b432b-149">Grupos e Sites podem ter vários recursos de unidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b432b-149">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="b432b-150">Unidades com a faceta [sistema][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="b432b-150">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="b432b-151">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="b432b-151">To list them, include `system` in your `$select` statement.</span></span>

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
