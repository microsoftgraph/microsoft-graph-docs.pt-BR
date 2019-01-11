---
title: Atualizar página
description: Atualize o conteúdo de uma página do OneNote.
localization_priority: Normal
ms.openlocfilehash: 78dc12f9eb5c041ae58f49aae137063b8a94bce3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833403"
---
# <a name="update-page"></a><span data-ttu-id="1a33c-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="1a33c-103">Update page</span></span>

> <span data-ttu-id="1a33c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a33c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a33c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a33c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a33c-106">Atualize o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1a33c-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a33c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a33c-107">Permissions</span></span>
<span data-ttu-id="1a33c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a33c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a33c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a33c-110">Permission type</span></span>      | <span data-ttu-id="1a33c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a33c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a33c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a33c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a33c-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a33c-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a33c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a33c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a33c-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a33c-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1a33c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a33c-116">Application</span></span> | <span data-ttu-id="1a33c-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a33c-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a33c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a33c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="1a33c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a33c-119">Request headers</span></span>
| <span data-ttu-id="1a33c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1a33c-120">Name</span></span>       | <span data-ttu-id="1a33c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a33c-121">Type</span></span> | <span data-ttu-id="1a33c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a33c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a33c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a33c-123">Authorization</span></span>  | <span data-ttu-id="1a33c-124">string</span><span class="sxs-lookup"><span data-stu-id="1a33c-124">string</span></span>  | <span data-ttu-id="1a33c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a33c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a33c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a33c-127">Content-Type</span></span> | <span data-ttu-id="1a33c-128">string</span><span class="sxs-lookup"><span data-stu-id="1a33c-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1a33c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a33c-129">Request body</span></span>
<span data-ttu-id="1a33c-130">No corpo da solicitação, fornece uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações para a página.</span><span class="sxs-lookup"><span data-stu-id="1a33c-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="1a33c-131">Para obter mais informações e exemplos, consulte o [conteúdo de página do OneNote de atualização](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="1a33c-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="1a33c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a33c-132">Response</span></span>

<span data-ttu-id="1a33c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="1a33c-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="1a33c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a33c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a33c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a33c-136">Request</span></span>
<span data-ttu-id="1a33c-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a33c-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1a33c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a33c-138">Response</span></span>
<span data-ttu-id="1a33c-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a33c-139">Here is an example of the response.</span></span> 
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
