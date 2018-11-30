---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Criar uma lista do SharePoint
ms.openlocfilehash: a1e247722e9e8874a78a1951619e08bff9bd36e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040523"
---
# <a name="create-a-new-list"></a><span data-ttu-id="60b75-102">Criar uma nova lista</span><span class="sxs-lookup"><span data-stu-id="60b75-102">Create a new list</span></span>

> <span data-ttu-id="60b75-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60b75-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60b75-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60b75-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60b75-105">Criar uma nova [lista][] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="60b75-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="60b75-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60b75-106">Permissions</span></span>

<span data-ttu-id="60b75-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="60b75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60b75-109">Permission type</span></span>             | <span data-ttu-id="60b75-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60b75-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="60b75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60b75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60b75-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="60b75-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="60b75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60b75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60b75-114">Not supported.</span></span>                              |
| <span data-ttu-id="60b75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60b75-115">Application</span></span>                            | <span data-ttu-id="60b75-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b75-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60b75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60b75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="60b75-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60b75-118">Request body</span></span>

<span data-ttu-id="60b75-119">No corpo da solicitação, forneça uma representação JSON do recurso [lista][] a criar.</span><span class="sxs-lookup"><span data-stu-id="60b75-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="60b75-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60b75-120">Example</span></span>

<span data-ttu-id="60b75-121">Aqui está um exemplo de como criar uma nova lista genérica.</span><span class="sxs-lookup"><span data-stu-id="60b75-121">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

<span data-ttu-id="60b75-122">**Observação:** Colunas personalizadas são opcionais.</span><span class="sxs-lookup"><span data-stu-id="60b75-122">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="60b75-123">Além de todas as colunas especificadas aqui, novas listas são criadas com colunas definidas no **modelo** referenciado.</span><span class="sxs-lookup"><span data-stu-id="60b75-123">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="60b75-124">Se a faceta **lista** ou **modelo** não for especificada, a lista considera como padrão o modelo `genericList`, que inclui uma coluna _Título_.</span><span class="sxs-lookup"><span data-stu-id="60b75-124">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="60b75-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b75-125">Response</span></span>

<span data-ttu-id="60b75-126">Se for bem-sucedido, esse método retornará uma [lista][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="60b75-126">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
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

<span data-ttu-id="60b75-127">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="60b75-127">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="60b75-128">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="60b75-128">Default properties will be returned from the actual call.</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
