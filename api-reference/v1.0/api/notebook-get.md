---
title: Obter bloco de anotações
description: Recupere as propriedades e os relacionamentos de um objeto notebook.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 21082e138a55a64e8d633fed663aeb91e09ce7f0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458973"
---
# <a name="get-notebook"></a><span data-ttu-id="52ae5-103">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="52ae5-103">Get notebook</span></span>

<span data-ttu-id="52ae5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52ae5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52ae5-105">Recupere as propriedades e os relacionamentos de um objeto [Notebook](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="52ae5-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52ae5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="52ae5-106">Permissions</span></span>
<span data-ttu-id="52ae5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52ae5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52ae5-109">Permission type</span></span>      | <span data-ttu-id="52ae5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52ae5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52ae5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52ae5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52ae5-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52ae5-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="52ae5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52ae5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52ae5-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52ae5-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="52ae5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52ae5-115">Application</span></span> | <span data-ttu-id="52ae5-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52ae5-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52ae5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52ae5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52ae5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52ae5-118">Optional query parameters</span></span>
<span data-ttu-id="52ae5-119">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52ae5-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="52ae5-120">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="52ae5-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52ae5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52ae5-121">Request headers</span></span>
| <span data-ttu-id="52ae5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="52ae5-122">Name</span></span>       | <span data-ttu-id="52ae5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ae5-123">Type</span></span> | <span data-ttu-id="52ae5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ae5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52ae5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="52ae5-125">Authorization</span></span>  | <span data-ttu-id="52ae5-126">string</span><span class="sxs-lookup"><span data-stu-id="52ae5-126">string</span></span>  | <span data-ttu-id="52ae5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52ae5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52ae5-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52ae5-129">Accept</span></span> | <span data-ttu-id="52ae5-130">string</span><span class="sxs-lookup"><span data-stu-id="52ae5-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="52ae5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52ae5-131">Request body</span></span>
<span data-ttu-id="52ae5-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52ae5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52ae5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ae5-133">Response</span></span>

<span data-ttu-id="52ae5-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52ae5-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52ae5-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52ae5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52ae5-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52ae5-136">Request</span></span>
<span data-ttu-id="52ae5-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52ae5-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52ae5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="52ae5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
# <a name="c"></a>[<span data-ttu-id="52ae5-139">C#</span><span class="sxs-lookup"><span data-stu-id="52ae5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52ae5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52ae5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52ae5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52ae5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52ae5-142">Java</span><span class="sxs-lookup"><span data-stu-id="52ae5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52ae5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ae5-143">Response</span></span>
<span data-ttu-id="52ae5-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52ae5-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
