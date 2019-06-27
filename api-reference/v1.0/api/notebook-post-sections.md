---
title: Criar seção
description: Criar um novo onenoteSection no bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e4d4bca4de6bc5814435a896ddfcf5f3b5ec1b3c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274498"
---
# <a name="create-section"></a><span data-ttu-id="8469d-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="8469d-103">Create section</span></span>

<span data-ttu-id="8469d-104">Criar um novo [onenoteSection](../resources/section.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="8469d-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="8469d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8469d-105">Permissions</span></span>
<span data-ttu-id="8469d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8469d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8469d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8469d-108">Permission type</span></span>      | <span data-ttu-id="8469d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8469d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8469d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8469d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8469d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8469d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8469d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8469d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8469d-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8469d-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8469d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8469d-114">Application</span></span> | <span data-ttu-id="8469d-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8469d-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8469d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8469d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="8469d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8469d-117">Request headers</span></span>
| <span data-ttu-id="8469d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8469d-118">Name</span></span>       | <span data-ttu-id="8469d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8469d-119">Type</span></span> | <span data-ttu-id="8469d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8469d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8469d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8469d-121">Authorization</span></span>  | <span data-ttu-id="8469d-122">string</span><span class="sxs-lookup"><span data-stu-id="8469d-122">string</span></span>  | <span data-ttu-id="8469d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8469d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8469d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8469d-125">Content-Type</span></span> | <span data-ttu-id="8469d-126">string</span><span class="sxs-lookup"><span data-stu-id="8469d-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8469d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8469d-127">Request body</span></span>
<span data-ttu-id="8469d-128">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="8469d-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="8469d-p103">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="8469d-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="8469d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8469d-131">Response</span></span>

<span data-ttu-id="8469d-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8469d-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8469d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8469d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8469d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8469d-134">Request</span></span>
<span data-ttu-id="8469d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8469d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="8469d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8469d-136">Response</span></span>
<span data-ttu-id="8469d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8469d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8469d-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="8469d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8469d-141">C#</span><span class="sxs-lookup"><span data-stu-id="8469d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_section_from_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8469d-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="8469d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_section_from_notebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8469d-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8469d-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_section_from_notebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-post-sections.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-post-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-post-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
