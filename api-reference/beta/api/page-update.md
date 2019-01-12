---
title: Atualizar página
description: Atualize o conteúdo de uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 91be57e33bba2d90725beaee8607fd3e2eddb84a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960691"
---
# <a name="update-page"></a><span data-ttu-id="93063-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="93063-103">Update page</span></span>

> <span data-ttu-id="93063-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93063-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93063-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93063-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93063-106">Atualize o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="93063-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="93063-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="93063-107">Permissions</span></span>
<span data-ttu-id="93063-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93063-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93063-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93063-110">Permission type</span></span>      | <span data-ttu-id="93063-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93063-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93063-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93063-112">Delegated (work or school account)</span></span> | <span data-ttu-id="93063-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93063-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="93063-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93063-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93063-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93063-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="93063-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93063-116">Application</span></span> | <span data-ttu-id="93063-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93063-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93063-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93063-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="93063-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93063-119">Request headers</span></span>
| <span data-ttu-id="93063-120">Nome</span><span class="sxs-lookup"><span data-stu-id="93063-120">Name</span></span>       | <span data-ttu-id="93063-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="93063-121">Type</span></span> | <span data-ttu-id="93063-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="93063-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93063-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93063-123">Authorization</span></span>  | <span data-ttu-id="93063-124">string</span><span class="sxs-lookup"><span data-stu-id="93063-124">string</span></span>  | <span data-ttu-id="93063-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93063-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93063-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93063-127">Content-Type</span></span> | <span data-ttu-id="93063-128">string</span><span class="sxs-lookup"><span data-stu-id="93063-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="93063-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93063-129">Request body</span></span>
<span data-ttu-id="93063-130">No corpo da solicitação, fornece uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações para a página.</span><span class="sxs-lookup"><span data-stu-id="93063-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="93063-131">Para obter mais informações e exemplos, consulte o [conteúdo de página do OneNote de atualização](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="93063-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="93063-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="93063-132">Response</span></span>

<span data-ttu-id="93063-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="93063-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="93063-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93063-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93063-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93063-136">Request</span></span>
<span data-ttu-id="93063-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93063-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
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
##### <a name="response"></a><span data-ttu-id="93063-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="93063-138">Response</span></span>
<span data-ttu-id="93063-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93063-139">Here is an example of the response.</span></span> 
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
