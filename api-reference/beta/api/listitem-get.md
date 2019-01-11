---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.openlocfilehash: f023743f0780a0f79aff3c3235e139166dc90be1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846505"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="d1173-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="d1173-102">Get an item in a list</span></span>

> <span data-ttu-id="d1173-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1173-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1173-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1173-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1173-105">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="d1173-105">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="d1173-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1173-108">Permissions</span></span>

<span data-ttu-id="d1173-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1173-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1173-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1173-111">Permission type</span></span>      | <span data-ttu-id="d1173-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1173-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1173-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1173-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1173-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1173-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1173-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1173-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1173-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1173-116">Not supported.</span></span>    |
|<span data-ttu-id="d1173-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1173-117">Application</span></span> | <span data-ttu-id="d1173-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1173-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1173-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1173-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="d1173-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1173-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d1173-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1173-121">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="d1173-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1173-122">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
