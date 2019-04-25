---
title: Atualizar página
description: Atualizar o conteúdo de uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d80aae98828fa2ad07360e3a5b8d660e5d980b35
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539385"
---
# <a name="update-page"></a><span data-ttu-id="e4b21-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="e4b21-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4b21-104">Atualizar o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e4b21-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4b21-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4b21-105">Permissions</span></span>
<span data-ttu-id="e4b21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b21-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4b21-108">Permission type</span></span>      | <span data-ttu-id="e4b21-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4b21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b21-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4b21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4b21-111">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e4b21-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4b21-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4b21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b21-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4b21-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e4b21-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4b21-114">Application</span></span> | <span data-ttu-id="e4b21-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b21-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b21-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4b21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="e4b21-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4b21-117">Request headers</span></span>
| <span data-ttu-id="e4b21-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e4b21-118">Name</span></span>       | <span data-ttu-id="e4b21-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4b21-119">Type</span></span> | <span data-ttu-id="e4b21-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4b21-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4b21-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4b21-121">Authorization</span></span>  | <span data-ttu-id="e4b21-122">string</span><span class="sxs-lookup"><span data-stu-id="e4b21-122">string</span></span>  | <span data-ttu-id="e4b21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4b21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4b21-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4b21-125">Content-Type</span></span> | <span data-ttu-id="e4b21-126">string</span><span class="sxs-lookup"><span data-stu-id="e4b21-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e4b21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4b21-127">Request body</span></span>
<span data-ttu-id="e4b21-128">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações na página.</span><span class="sxs-lookup"><span data-stu-id="e4b21-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="e4b21-129">Para obter mais informações e exemplos, consulte [Atualizar conteúdo da página do OneNote](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="e4b21-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="e4b21-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4b21-130">Response</span></span>

<span data-ttu-id="e4b21-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4b21-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="e4b21-132">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="e4b21-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="e4b21-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4b21-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4b21-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4b21-134">Request</span></span>
<span data-ttu-id="e4b21-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4b21-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e4b21-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4b21-136">Response</span></span>
<span data-ttu-id="e4b21-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4b21-137">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
