---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 4cfad0f0a37d50638da869b5aebc9f8f38154c5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450188"
---
# <a name="get-notebook"></a><span data-ttu-id="d20cc-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="d20cc-103">Get notebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d20cc-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="d20cc-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d20cc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d20cc-105">Permissions</span></span>
<span data-ttu-id="d20cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d20cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d20cc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d20cc-108">Permission type</span></span>      | <span data-ttu-id="d20cc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d20cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d20cc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d20cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d20cc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20cc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d20cc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d20cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d20cc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d20cc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d20cc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d20cc-114">Application</span></span> | <span data-ttu-id="d20cc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20cc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d20cc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d20cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d20cc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d20cc-117">Optional query parameters</span></span>
<span data-ttu-id="d20cc-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d20cc-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d20cc-119">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="d20cc-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d20cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d20cc-120">Request headers</span></span>
| <span data-ttu-id="d20cc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d20cc-121">Name</span></span>       | <span data-ttu-id="d20cc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d20cc-122">Type</span></span> | <span data-ttu-id="d20cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d20cc-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d20cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d20cc-124">Authorization</span></span>  | <span data-ttu-id="d20cc-125">string</span><span class="sxs-lookup"><span data-stu-id="d20cc-125">string</span></span>  | <span data-ttu-id="d20cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d20cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d20cc-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d20cc-128">Accept</span></span> | <span data-ttu-id="d20cc-129">string</span><span class="sxs-lookup"><span data-stu-id="d20cc-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d20cc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d20cc-130">Request body</span></span>
<span data-ttu-id="d20cc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d20cc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d20cc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d20cc-132">Response</span></span>

<span data-ttu-id="d20cc-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d20cc-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d20cc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d20cc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d20cc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d20cc-135">Request</span></span>
<span data-ttu-id="d20cc-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d20cc-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d20cc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d20cc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d20cc-138">C#</span><span class="sxs-lookup"><span data-stu-id="d20cc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d20cc-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d20cc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d20cc-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d20cc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d20cc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d20cc-141">Response</span></span>
<span data-ttu-id="d20cc-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d20cc-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
