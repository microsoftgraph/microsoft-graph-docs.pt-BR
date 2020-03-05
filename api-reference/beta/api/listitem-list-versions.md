---
author: JeremyKelley
description: O SharePoint pode ser configurado para manter o histórico para itens da lista.
ms.date: 09/10/2017
title: Obtenha uma versão anterior de um registro de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 13dd9e08ae60b4c8ac3b4e9fd1a99bf4f70b53d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457108"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="4f06d-103">Listar versões de um item de lista (prévia)</span><span class="sxs-lookup"><span data-stu-id="4f06d-103">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="4f06d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f06d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f06d-105">O SharePoint pode ser configurado para manter o histórico para itens da lista.</span><span class="sxs-lookup"><span data-stu-id="4f06d-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="4f06d-106">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="4f06d-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f06d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f06d-107">Permissions</span></span>

<span data-ttu-id="4f06d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="4f06d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f06d-110">Permission type</span></span>             | <span data-ttu-id="4f06d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f06d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4f06d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f06d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f06d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f06d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="4f06d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f06d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f06d-115">n/d</span><span class="sxs-lookup"><span data-stu-id="4f06d-115">n/a</span></span>                                         |
| <span data-ttu-id="4f06d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f06d-116">Application</span></span>                            | <span data-ttu-id="4f06d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f06d-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="4f06d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f06d-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="4f06d-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f06d-119">Response</span></span>

<span data-ttu-id="4f06d-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f06d-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="4f06d-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f06d-121">Example</span></span>

<span data-ttu-id="4f06d-122">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="4f06d-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="4f06d-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f06d-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="4f06d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f06d-124">Response</span></span>

<span data-ttu-id="4f06d-125">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="4f06d-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
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
