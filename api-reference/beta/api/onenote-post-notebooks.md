---
title: Criar blocos de anotações
description: Criar um novo bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 1fe0e9ac5c4ed1da62bf7419a0bd9e5fefa3a235
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878826"
---
# <a name="create-notebook"></a><span data-ttu-id="4f094-103">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="4f094-103">Create notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f094-104">Criar um novo [bloco de anotações](../resources/notebook.md)do OneNote.</span><span class="sxs-lookup"><span data-stu-id="4f094-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4f094-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f094-105">Permissions</span></span>
<span data-ttu-id="4f094-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f094-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f094-108">Permission type</span></span>      | <span data-ttu-id="4f094-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f094-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f094-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f094-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f094-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f094-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f094-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f094-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f094-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f094-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4f094-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f094-114">Application</span></span> | <span data-ttu-id="4f094-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f094-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f094-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f094-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="4f094-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f094-117">Request headers</span></span>
| <span data-ttu-id="4f094-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4f094-118">Name</span></span>       | <span data-ttu-id="4f094-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f094-119">Type</span></span> | <span data-ttu-id="4f094-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f094-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f094-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f094-121">Authorization</span></span>  | <span data-ttu-id="4f094-122">string</span><span class="sxs-lookup"><span data-stu-id="4f094-122">string</span></span>  | <span data-ttu-id="4f094-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f094-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f094-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f094-125">Content-Type</span></span> | <span data-ttu-id="4f094-126">string</span><span class="sxs-lookup"><span data-stu-id="4f094-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4f094-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f094-127">Request body</span></span>
<span data-ttu-id="4f094-128">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="4f094-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="4f094-129">Os nomes dos blocos de anotações devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="4f094-129">Notebook names must be unique.</span></span> <span data-ttu-id="4f094-130">O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:?\/\*: <>| ' "</span><span class="sxs-lookup"><span data-stu-id="4f094-130">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="4f094-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f094-131">Response</span></span>

<span data-ttu-id="4f094-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e o novo objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f094-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f094-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f094-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f094-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f094-134">Request</span></span>
<span data-ttu-id="4f094-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f094-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f094-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f094-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f094-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f094-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f094-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f094-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f094-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4f094-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f094-140">Java</span><span class="sxs-lookup"><span data-stu-id="4f094-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-notebook-from-onenote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f094-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f094-141">Response</span></span>
<span data-ttu-id="4f094-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f094-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
