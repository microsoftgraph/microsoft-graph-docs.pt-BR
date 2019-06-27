---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 927b79c959dbf2d80c74d4e756f786e8e5203af2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265979"
---
# <a name="get-notebook"></a><span data-ttu-id="3bd3c-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="3bd3c-103">Get notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd3c-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="3bd3c-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bd3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bd3c-105">Permissions</span></span>
<span data-ttu-id="3bd3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bd3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bd3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bd3c-108">Permission type</span></span>      | <span data-ttu-id="3bd3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bd3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bd3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bd3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bd3c-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd3c-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bd3c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bd3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bd3c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bd3c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3bd3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bd3c-114">Application</span></span> | <span data-ttu-id="3bd3c-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd3c-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bd3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3bd3c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bd3c-117">Optional query parameters</span></span>
<span data-ttu-id="3bd3c-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3bd3c-119">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bd3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd3c-120">Request headers</span></span>
| <span data-ttu-id="3bd3c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3bd3c-121">Name</span></span>       | <span data-ttu-id="3bd3c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bd3c-122">Type</span></span> | <span data-ttu-id="3bd3c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bd3c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3bd3c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bd3c-124">Authorization</span></span>  | <span data-ttu-id="3bd3c-125">string</span><span class="sxs-lookup"><span data-stu-id="3bd3c-125">string</span></span>  | <span data-ttu-id="3bd3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bd3c-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bd3c-128">Accept</span></span> | <span data-ttu-id="3bd3c-129">string</span><span class="sxs-lookup"><span data-stu-id="3bd3c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3bd3c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd3c-130">Request body</span></span>
<span data-ttu-id="3bd3c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bd3c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bd3c-132">Response</span></span>

<span data-ttu-id="3bd3c-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3bd3c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bd3c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bd3c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd3c-135">Request</span></span>
<span data-ttu-id="3bd3c-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="3bd3c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bd3c-137">Response</span></span>
<span data-ttu-id="3bd3c-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bd3c-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bd3c-141">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="3bd3c-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bd3c-142">C#</span><span class="sxs-lookup"><span data-stu-id="3bd3c-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bd3c-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bd3c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_notebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3bd3c-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3bd3c-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_notebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
