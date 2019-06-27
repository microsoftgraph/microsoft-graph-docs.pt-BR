---
title: Criar blocos de anotações
description: Criar um novo bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 0f10795b6295b0aba4298bb238a33545b7cacc38
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274449"
---
# <a name="create-notebook"></a><span data-ttu-id="a3ef3-103">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="a3ef3-103">Create notebook</span></span>

<span data-ttu-id="a3ef3-104">Criar um novo [bloco de anotações](../resources/notebook.md)do OneNote.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a3ef3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3ef3-105">Permissions</span></span>
<span data-ttu-id="a3ef3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ef3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3ef3-108">Permission type</span></span>      | <span data-ttu-id="a3ef3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3ef3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3ef3-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ef3-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3ef3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3ef3-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3ef3-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a3ef3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3ef3-114">Application</span></span> | <span data-ttu-id="a3ef3-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ef3-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ef3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3ef3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="a3ef3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3ef3-117">Request headers</span></span>
| <span data-ttu-id="a3ef3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a3ef3-118">Name</span></span>       | <span data-ttu-id="a3ef3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3ef3-119">Type</span></span> | <span data-ttu-id="a3ef3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3ef3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3ef3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3ef3-121">Authorization</span></span>  | <span data-ttu-id="a3ef3-122">string</span><span class="sxs-lookup"><span data-stu-id="a3ef3-122">string</span></span>  | <span data-ttu-id="a3ef3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3ef3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3ef3-125">Content-Type</span></span> | <span data-ttu-id="a3ef3-126">string</span><span class="sxs-lookup"><span data-stu-id="a3ef3-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a3ef3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3ef3-127">Request body</span></span>
<span data-ttu-id="a3ef3-128">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="a3ef3-129">Os nomes dos blocos de anotações devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-129">Notebook names must be unique.</span></span> <span data-ttu-id="a3ef3-130">O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:?\/\*: <>| ' "</span><span class="sxs-lookup"><span data-stu-id="a3ef3-130">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="a3ef3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3ef3-131">Response</span></span>

<span data-ttu-id="a3ef3-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e o novo objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3ef3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3ef3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3ef3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3ef3-134">Request</span></span>
<span data-ttu-id="a3ef3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="a3ef3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3ef3-136">Response</span></span>
<span data-ttu-id="a3ef3-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3ef3-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="a3ef3-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3ef3-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3ef3-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_notebook_from_onenote-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3ef3-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3ef3-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_notebook_from_onenote-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a3ef3-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3ef3-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_notebook_from_onenote-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/onenote-post-notebooks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/onenote-post-notebooks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/onenote-post-notebooks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
