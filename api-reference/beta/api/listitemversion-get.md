---
author: JeremyKelley
description: Recuperar os metadados de uma versão específica de um ListItem.
ms.date: 09/10/2017
title: Obter uma versão anterior de um item de lista - API do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bcd53e58c1b5849cc1e98f57e22244201fd8d085
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972011"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="b6939-103">Obter um recurso ListItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="b6939-103">Get a ListItemVersion resource (preview)</span></span>

<span data-ttu-id="b6939-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6939-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6939-105">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="b6939-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6939-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6939-106">Permissions</span></span>

<span data-ttu-id="b6939-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="b6939-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6939-109">Permission type</span></span>             | <span data-ttu-id="b6939-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6939-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b6939-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6939-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6939-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6939-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="b6939-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6939-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6939-114">n/d</span><span class="sxs-lookup"><span data-stu-id="b6939-114">n/a</span></span>                                         |
| <span data-ttu-id="b6939-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6939-115">Application</span></span>                            | <span data-ttu-id="b6939-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6939-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="b6939-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6939-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="b6939-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6939-118">Response</span></span>

<span data-ttu-id="b6939-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6939-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b6939-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6939-120">Example</span></span>

<span data-ttu-id="b6939-121">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="b6939-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="b6939-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6939-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="b6939-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6939-123">Response</span></span>

<span data-ttu-id="b6939-124">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="b6939-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->


