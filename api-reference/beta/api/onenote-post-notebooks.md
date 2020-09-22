---
title: Criar blocos de anotações
description: Crie um novo bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: d129f8c6c8a740f44dcdddd29b3406e301dd6d42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004687"
---
# <a name="create-notebook"></a><span data-ttu-id="85c43-103">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="85c43-103">Create notebook</span></span>

<span data-ttu-id="85c43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c43-105">Criar um novo [bloco de anotações](../resources/notebook.md)do OneNote.</span><span class="sxs-lookup"><span data-stu-id="85c43-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85c43-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85c43-106">Permissions</span></span>
<span data-ttu-id="85c43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c43-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85c43-109">Permission type</span></span>      | <span data-ttu-id="85c43-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85c43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c43-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85c43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85c43-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c43-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="85c43-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85c43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c43-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85c43-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="85c43-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85c43-115">Application</span></span> | <span data-ttu-id="85c43-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c43-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85c43-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85c43-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="85c43-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85c43-118">Request headers</span></span>
| <span data-ttu-id="85c43-119">Nome</span><span class="sxs-lookup"><span data-stu-id="85c43-119">Name</span></span>       | <span data-ttu-id="85c43-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="85c43-120">Type</span></span> | <span data-ttu-id="85c43-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="85c43-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85c43-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85c43-122">Authorization</span></span>  | <span data-ttu-id="85c43-123">string</span><span class="sxs-lookup"><span data-stu-id="85c43-123">string</span></span>  | <span data-ttu-id="85c43-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85c43-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85c43-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85c43-126">Content-Type</span></span> | <span data-ttu-id="85c43-127">string</span><span class="sxs-lookup"><span data-stu-id="85c43-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="85c43-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85c43-128">Request body</span></span>
<span data-ttu-id="85c43-129">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="85c43-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="85c43-130">Os nomes dos blocos de anotações devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="85c43-130">Notebook names must be unique.</span></span> <span data-ttu-id="85c43-131">O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:? \* \/ : <>| ' "</span><span class="sxs-lookup"><span data-stu-id="85c43-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="85c43-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c43-132">Response</span></span>

<span data-ttu-id="85c43-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e o novo objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85c43-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c43-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85c43-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85c43-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85c43-135">Request</span></span>
<span data-ttu-id="85c43-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85c43-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85c43-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="85c43-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```
# <a name="c"></a>[<span data-ttu-id="85c43-138">C#</span><span class="sxs-lookup"><span data-stu-id="85c43-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85c43-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85c43-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85c43-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85c43-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85c43-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c43-141">Response</span></span>
<span data-ttu-id="85c43-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85c43-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


