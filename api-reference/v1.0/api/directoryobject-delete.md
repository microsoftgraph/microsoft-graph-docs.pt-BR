---
title: Excluir directoryObject
description: Exclui um directoryObject.
author: lleonard-msft
ms.openlocfilehash: dec525e72b523e7bbe95996d4c863c68e01baa15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313199"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="85873-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="85873-103">Delete directoryObject</span></span>

<span data-ttu-id="85873-104">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="85873-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="85873-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85873-105">Permissions</span></span>
<span data-ttu-id="85873-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="85873-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85873-108">Permission type</span></span>      | <span data-ttu-id="85873-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85873-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85873-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85873-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85873-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85873-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85873-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85873-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85873-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85873-113">Not supported.</span></span>    |
|<span data-ttu-id="85873-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85873-114">Application</span></span> | <span data-ttu-id="85873-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85873-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85873-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85873-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="85873-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85873-117">Request headers</span></span>
| <span data-ttu-id="85873-118">Nome</span><span class="sxs-lookup"><span data-stu-id="85873-118">Name</span></span>       | <span data-ttu-id="85873-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="85873-119">Type</span></span> | <span data-ttu-id="85873-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="85873-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85873-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85873-121">Authorization</span></span>  | <span data-ttu-id="85873-122">string</span><span class="sxs-lookup"><span data-stu-id="85873-122">string</span></span>  | <span data-ttu-id="85873-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85873-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85873-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85873-125">Request body</span></span>
<span data-ttu-id="85873-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85873-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85873-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="85873-127">Response</span></span>

<span data-ttu-id="85873-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85873-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85873-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85873-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85873-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85873-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="85873-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="85873-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->