---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
localization_priority: Normal
ms.openlocfilehash: 8268ec362a2ce60686f0ef2467243799cd650a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822544"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="6710f-102">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="6710f-102">Create a new item in a list</span></span>

> <span data-ttu-id="6710f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6710f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6710f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6710f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6710f-105">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="6710f-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6710f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6710f-106">Permissions</span></span>

<span data-ttu-id="6710f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6710f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6710f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6710f-109">Permission type</span></span>      | <span data-ttu-id="6710f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6710f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6710f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6710f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6710f-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6710f-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6710f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6710f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6710f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6710f-114">Not supported.</span></span>    |
|<span data-ttu-id="6710f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6710f-115">Application</span></span> | <span data-ttu-id="6710f-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6710f-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6710f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6710f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="6710f-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6710f-118">Request body</span></span>

<span data-ttu-id="6710f-119">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="6710f-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="6710f-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6710f-120">Example</span></span>

<span data-ttu-id="6710f-121">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="6710f-121">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="6710f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="6710f-122">Response</span></span>

<span data-ttu-id="6710f-123">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="6710f-123">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="6710f-124">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="6710f-124">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="6710f-125">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="6710f-125">Default properties will be returned from the actual call.</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
