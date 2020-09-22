---
author: JeremyKelley
description: O SharePoint pode ser configurado para manter o histórico para itens da lista.
ms.date: 09/10/2017
title: Obtenha uma versão anterior de um registro de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 731a6b2a71fd03790e447dfb331c7cf4e6f5f482
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972025"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="932bb-103">Listar versões de um item de lista (prévia)</span><span class="sxs-lookup"><span data-stu-id="932bb-103">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="932bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="932bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="932bb-105">O SharePoint pode ser configurado para manter o histórico para itens da lista.</span><span class="sxs-lookup"><span data-stu-id="932bb-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="932bb-106">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="932bb-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="932bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="932bb-107">Permissions</span></span>

<span data-ttu-id="932bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="932bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="932bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="932bb-110">Permission type</span></span>             | <span data-ttu-id="932bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="932bb-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="932bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="932bb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="932bb-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="932bb-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="932bb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="932bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="932bb-115">n/d</span><span class="sxs-lookup"><span data-stu-id="932bb-115">n/a</span></span>                                         |
| <span data-ttu-id="932bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="932bb-116">Application</span></span>                            | <span data-ttu-id="932bb-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="932bb-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="932bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="932bb-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="932bb-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="932bb-119">Response</span></span>

<span data-ttu-id="932bb-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="932bb-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="932bb-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="932bb-121">Example</span></span>

<span data-ttu-id="932bb-122">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="932bb-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="932bb-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="932bb-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="932bb-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="932bb-124">Response</span></span>

<span data-ttu-id="932bb-125">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="932bb-125">This returns a collection of versions:</span></span>

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


