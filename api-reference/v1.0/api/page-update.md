---
title: Atualizar página
description: Atualize o conteúdo de uma página do OneNote.
ms.openlocfilehash: fd81e2c14db5a60fee9d0c8c5092c09957ed8421
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005578"
---
# <a name="update-page"></a><span data-ttu-id="d1931-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="d1931-103">Update page</span></span>

<span data-ttu-id="d1931-104">Atualize o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d1931-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1931-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1931-105">Permissions</span></span>
<span data-ttu-id="d1931-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1931-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1931-108">Permission type</span></span>      | <span data-ttu-id="d1931-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1931-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1931-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1931-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d1931-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1931-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1931-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1931-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1931-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1931-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d1931-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1931-114">Application</span></span> | <span data-ttu-id="d1931-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1931-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1931-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1931-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="d1931-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1931-117">Request headers</span></span>
| <span data-ttu-id="d1931-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d1931-118">Name</span></span>       | <span data-ttu-id="d1931-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1931-119">Type</span></span> | <span data-ttu-id="d1931-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1931-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1931-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1931-121">Authorization</span></span>  | <span data-ttu-id="d1931-122">string</span><span class="sxs-lookup"><span data-stu-id="d1931-122">string</span></span>  | <span data-ttu-id="d1931-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1931-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1931-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1931-125">Content-Type</span></span> | <span data-ttu-id="d1931-126">string</span><span class="sxs-lookup"><span data-stu-id="d1931-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d1931-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1931-127">Request body</span></span>
<span data-ttu-id="d1931-p103">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representa as alterações da página. Veja mais informações e exemplos em <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Atualizar páginas do OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="d1931-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="d1931-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1931-130">Response</span></span>

<span data-ttu-id="d1931-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="d1931-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="d1931-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1931-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1931-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1931-134">Request</span></span>
<span data-ttu-id="d1931-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1931-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="d1931-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1931-136">Response</span></span>
<span data-ttu-id="d1931-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1931-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
