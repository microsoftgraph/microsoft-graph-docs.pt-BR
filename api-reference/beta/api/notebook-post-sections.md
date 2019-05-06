---
title: Criar seção
description: Crie uma nova seção no bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d664c747a6d19f314e99792809a25049b874c8a8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597309"
---
# <a name="create-section"></a><span data-ttu-id="18cbe-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="18cbe-103">Create section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18cbe-104">Crie uma nova [seção](../resources/onenotesection.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="18cbe-104">Create a new [section](../resources/onenotesection.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="18cbe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="18cbe-105">Permissions</span></span>
<span data-ttu-id="18cbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18cbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18cbe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18cbe-108">Permission type</span></span>      | <span data-ttu-id="18cbe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18cbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18cbe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18cbe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18cbe-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cbe-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18cbe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18cbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18cbe-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18cbe-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18cbe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18cbe-114">Application</span></span> | <span data-ttu-id="18cbe-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cbe-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18cbe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18cbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="18cbe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18cbe-117">Request headers</span></span>
| <span data-ttu-id="18cbe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="18cbe-118">Name</span></span>       | <span data-ttu-id="18cbe-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="18cbe-119">Type</span></span> | <span data-ttu-id="18cbe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18cbe-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18cbe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18cbe-121">Authorization</span></span>  | <span data-ttu-id="18cbe-122">string</span><span class="sxs-lookup"><span data-stu-id="18cbe-122">string</span></span>  | <span data-ttu-id="18cbe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18cbe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18cbe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18cbe-125">Content-Type</span></span> | <span data-ttu-id="18cbe-126">string</span><span class="sxs-lookup"><span data-stu-id="18cbe-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18cbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18cbe-127">Request body</span></span>
<span data-ttu-id="18cbe-128">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="18cbe-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="18cbe-p103">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="18cbe-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="18cbe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="18cbe-131">Response</span></span>

<span data-ttu-id="18cbe-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18cbe-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18cbe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18cbe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18cbe-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18cbe-134">Request</span></span>
<span data-ttu-id="18cbe-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18cbe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="18cbe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="18cbe-136">Response</span></span>
<span data-ttu-id="18cbe-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18cbe-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="18cbe-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="18cbe-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18cbe-141">Basic</span><span class="sxs-lookup"><span data-stu-id="18cbe-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_section_from_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18cbe-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18cbe-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_section_from_notebook-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-post-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-post-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
