---
title: Excluir página
description: Exclua uma página do OneNote.
ms.openlocfilehash: 574fa3a84a3ca18a788035e4a90bcc833907014e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005343"
---
# <a name="delete-page"></a><span data-ttu-id="f3e85-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="f3e85-103">Delete page</span></span>

<span data-ttu-id="f3e85-104">Exclua uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f3e85-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3e85-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3e85-105">Permissions</span></span>
<span data-ttu-id="f3e85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e85-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3e85-108">Permission type</span></span>      | <span data-ttu-id="f3e85-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3e85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e85-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3e85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3e85-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e85-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3e85-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3e85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3e85-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3e85-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f3e85-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3e85-114">Application</span></span> | <span data-ttu-id="f3e85-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e85-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3e85-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3e85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f3e85-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e85-117">Request headers</span></span>
| <span data-ttu-id="f3e85-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f3e85-118">Name</span></span>       | <span data-ttu-id="f3e85-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3e85-119">Type</span></span> | <span data-ttu-id="f3e85-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3e85-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3e85-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3e85-121">Authorization</span></span>  | <span data-ttu-id="f3e85-122">string</span><span class="sxs-lookup"><span data-stu-id="f3e85-122">string</span></span>  | <span data-ttu-id="f3e85-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3e85-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f3e85-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e85-125">Response</span></span>

<span data-ttu-id="f3e85-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3e85-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e85-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3e85-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3e85-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e85-129">Request</span></span>
<span data-ttu-id="f3e85-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3e85-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="f3e85-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e85-131">Response</span></span>
<span data-ttu-id="f3e85-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3e85-132">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->