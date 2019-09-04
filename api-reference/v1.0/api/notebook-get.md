---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2c7bf57d4bf04784ff0f872ed7cdd5a0a6f0123b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728641"
---
# <a name="get-notebook"></a><span data-ttu-id="274d6-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="274d6-103">Get notebook</span></span>

<span data-ttu-id="274d6-104">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="274d6-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="274d6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="274d6-105">Permissions</span></span>
<span data-ttu-id="274d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="274d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="274d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="274d6-108">Permission type</span></span>      | <span data-ttu-id="274d6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="274d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="274d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="274d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="274d6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="274d6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="274d6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="274d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="274d6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274d6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="274d6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="274d6-114">Application</span></span> | <span data-ttu-id="274d6-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="274d6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="274d6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="274d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="274d6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="274d6-117">Optional query parameters</span></span>
<span data-ttu-id="274d6-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="274d6-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="274d6-119">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="274d6-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="274d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="274d6-120">Request headers</span></span>
| <span data-ttu-id="274d6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="274d6-121">Name</span></span>       | <span data-ttu-id="274d6-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="274d6-122">Type</span></span> | <span data-ttu-id="274d6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="274d6-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="274d6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="274d6-124">Authorization</span></span>  | <span data-ttu-id="274d6-125">string</span><span class="sxs-lookup"><span data-stu-id="274d6-125">string</span></span>  | <span data-ttu-id="274d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="274d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="274d6-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="274d6-128">Accept</span></span> | <span data-ttu-id="274d6-129">string</span><span class="sxs-lookup"><span data-stu-id="274d6-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="274d6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="274d6-130">Request body</span></span>
<span data-ttu-id="274d6-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="274d6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="274d6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="274d6-132">Response</span></span>

<span data-ttu-id="274d6-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="274d6-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="274d6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="274d6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="274d6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="274d6-135">Request</span></span>
<span data-ttu-id="274d6-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="274d6-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="274d6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="274d6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="274d6-138">C#</span><span class="sxs-lookup"><span data-stu-id="274d6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="274d6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="274d6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="274d6-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="274d6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="274d6-141">Java</span><span class="sxs-lookup"><span data-stu-id="274d6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="274d6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="274d6-142">Response</span></span>
<span data-ttu-id="274d6-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="274d6-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
