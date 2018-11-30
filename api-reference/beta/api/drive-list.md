---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar unidades
ms.openlocfilehash: f2a22e8bd7cca02aad549be5230f2436b3aa1791
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033365"
---
# <a name="list-available-drives"></a><span data-ttu-id="d1f63-102">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="d1f63-102">List available drives</span></span>

> <span data-ttu-id="d1f63-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1f63-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1f63-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1f63-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1f63-105">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.</span><span class="sxs-lookup"><span data-stu-id="d1f63-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1f63-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1f63-106">Permissions</span></span>

<span data-ttu-id="d1f63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1f63-109">Permission type</span></span>      | <span data-ttu-id="d1f63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1f63-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1f63-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1f63-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1f63-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f63-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1f63-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1f63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1f63-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f63-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1f63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1f63-115">Application</span></span> | <span data-ttu-id="d1f63-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f63-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="d1f63-117">Lista as unidades de um grupo</span><span class="sxs-lookup"><span data-stu-id="d1f63-117">List a group's drives</span></span>

<span data-ttu-id="d1f63-118">Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.</span><span class="sxs-lookup"><span data-stu-id="d1f63-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="d1f63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1f63-119">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a><span data-ttu-id="d1f63-120">Lista as unidades do site</span><span class="sxs-lookup"><span data-stu-id="d1f63-120">List a site's drives</span></span>

<span data-ttu-id="d1f63-121">Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.</span><span class="sxs-lookup"><span data-stu-id="d1f63-121">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a><span data-ttu-id="d1f63-122">Lista as unidades de um usuário</span><span class="sxs-lookup"><span data-stu-id="d1f63-122">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a><span data-ttu-id="d1f63-123">Lista as unidades do usuário atual</span><span class="sxs-lookup"><span data-stu-id="d1f63-123">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1f63-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1f63-124">Optional query parameters</span></span>

<span data-ttu-id="d1f63-125">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="d1f63-125">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="d1f63-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1f63-126">Response</span></span>

<span data-ttu-id="d1f63-127">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1f63-127">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="d1f63-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1f63-128">Remarks</span></span>

<span data-ttu-id="d1f63-129">A maioria dos usuários só terá um único recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="d1f63-129">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="d1f63-130">Grupos e Sites podem ter vários recursos de unidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d1f63-130">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="d1f63-131">Unidades com a faceta [sistema][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="d1f63-131">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="d1f63-132">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="d1f63-132">To list them, include `system` in your `$select` statement.</span></span>

[sistema]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
