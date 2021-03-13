---
author: swapnil1993
title: Atualizar contentType
description: Atualizar um tipo de conteúdo
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 52cdcdc18b106c1b09b69d37cc027dc610630611
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773309"
---
# <a name="update-contenttype"></a><span data-ttu-id="32709-103">Atualizar contentType</span><span class="sxs-lookup"><span data-stu-id="32709-103">Update contentType</span></span>
<span data-ttu-id="32709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32709-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="32709-105">Atualizar um [tipo de conteúdo][contentType].</span><span class="sxs-lookup"><span data-stu-id="32709-105">Update a [content type][contentType].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="32709-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32709-106">Permissions</span></span>

  

<span data-ttu-id="32709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="32709-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32709-109">Permission type</span></span> | <span data-ttu-id="32709-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32709-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32709-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32709-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32709-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="32709-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="32709-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32709-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32709-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32709-114">Not supported.</span></span> |
|<span data-ttu-id="32709-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32709-115">Application</span></span> |<span data-ttu-id="32709-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="32709-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="32709-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32709-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="32709-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32709-118">Request headers</span></span>
|<span data-ttu-id="32709-119">Nome</span><span class="sxs-lookup"><span data-stu-id="32709-119">Name</span></span>|<span data-ttu-id="32709-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="32709-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32709-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="32709-121">Authorization</span></span>|<span data-ttu-id="32709-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32709-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32709-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32709-124">Content-Type</span></span>|<span data-ttu-id="32709-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32709-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32709-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32709-127">Request body</span></span>

<span data-ttu-id="32709-128">No corpo da solicitação, fornece uma representação JSON do [recurso contentType][] a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="32709-128">In the request body, supply a JSON representation of the [contentType][] resource to update.</span></span>  

## <a name="response"></a><span data-ttu-id="32709-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32709-129">Response</span></span>

<span data-ttu-id="32709-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto contentType][] atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32709-130">If successful, this method returns a `200 OK` response code and an updated [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32709-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32709-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32709-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32709-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="32709-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="32709-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
    "name": "updatedCt",
    "documentSet": {
        "shouldPrefixNameToFile": true,
        "allowedContentTypes": [{
            "id": "0x0101",
            "name": "Document"
        }],
        "defaultContents": [{
                "fileName": "a.txt",
                "contentType": {
                    "id": "0x0101"
                }
            },
            {
                "fileName": "b.txt",
                "contentType": {
                    "id": "0x0101"
                }
            }
        ],
        "sharedColumns": [{
                "name": "Description",
                "id": "cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
            },
            {
                "name": "Address",
                "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
            }
        ],
        "welcomePageColumns": [{
            "name": "Address",
            "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
        }]
    }
}

```
# <a name="javascript"></a>[<span data-ttu-id="32709-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32709-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32709-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32709-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32709-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="32709-136">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0x0101009B237E76EF94DC49B4E58139041E7C60",
    "description": "",
    "eTag": "\"7\"",
    "group": "Custom Content Types",
    "hidden": false,
    "name": "testdoc",
    "parentId": "0x0101",
    "base": {
        "id": "0x0101",
        "name": "Document"
    }
}

```

[contentType]: ../resources/contentType.md
