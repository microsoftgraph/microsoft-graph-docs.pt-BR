---
title: Excluir página
description: Exclua uma página do OneNote.
ms.openlocfilehash: f2e566696937ee6f7808a66f994298802be66a17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034641"
---
# <a name="delete-page"></a><span data-ttu-id="95f2b-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="95f2b-103">Delete page</span></span>

> <span data-ttu-id="95f2b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95f2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95f2b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95f2b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95f2b-106">Exclua uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="95f2b-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="95f2b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95f2b-107">Permissions</span></span>
<span data-ttu-id="95f2b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95f2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95f2b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95f2b-110">Permission type</span></span>      | <span data-ttu-id="95f2b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95f2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95f2b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95f2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95f2b-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2b-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="95f2b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95f2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95f2b-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95f2b-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="95f2b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95f2b-116">Application</span></span> | <span data-ttu-id="95f2b-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f2b-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95f2b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95f2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="95f2b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95f2b-119">Request headers</span></span>
| <span data-ttu-id="95f2b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="95f2b-120">Name</span></span>       | <span data-ttu-id="95f2b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="95f2b-121">Type</span></span> | <span data-ttu-id="95f2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="95f2b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95f2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95f2b-123">Authorization</span></span>  | <span data-ttu-id="95f2b-124">string</span><span class="sxs-lookup"><span data-stu-id="95f2b-124">string</span></span>  | <span data-ttu-id="95f2b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95f2b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="95f2b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f2b-127">Response</span></span>

<span data-ttu-id="95f2b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f2b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f2b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95f2b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95f2b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95f2b-131">Request</span></span>
<span data-ttu-id="95f2b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95f2b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="95f2b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f2b-133">Response</span></span>
<span data-ttu-id="95f2b-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f2b-134">Here is an example of the response.</span></span>
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