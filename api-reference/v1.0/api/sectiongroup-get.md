---
title: Obter o myseção
description: Recupere as propriedades e os relacionamentos de um objeto de objeto de seção.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 228c68883cb3ebf3e19df3146ff3839bcc19c9cb
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729312"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="21ffc-103">Obter o myseção</span><span class="sxs-lookup"><span data-stu-id="21ffc-103">Get sectionGroup</span></span>

<span data-ttu-id="21ffc-104">Recupere as propriedades e os relacionamentos de um objeto de objeto de [seção](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="21ffc-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21ffc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="21ffc-105">Permissions</span></span>
<span data-ttu-id="21ffc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21ffc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21ffc-108">Permission type</span></span>      | <span data-ttu-id="21ffc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21ffc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21ffc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21ffc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21ffc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ffc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="21ffc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21ffc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21ffc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21ffc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="21ffc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21ffc-114">Application</span></span> | <span data-ttu-id="21ffc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ffc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21ffc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21ffc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21ffc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21ffc-117">Optional query parameters</span></span>
<span data-ttu-id="21ffc-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21ffc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="21ffc-119">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `name`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="21ffc-119">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="21ffc-120">Os `expand` valores válidos para os grupos `parentNotebook` de `parentSectionGroup`seções são e.</span><span class="sxs-lookup"><span data-stu-id="21ffc-120">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21ffc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21ffc-121">Request headers</span></span>
| <span data-ttu-id="21ffc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="21ffc-122">Name</span></span>       | <span data-ttu-id="21ffc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="21ffc-123">Type</span></span> | <span data-ttu-id="21ffc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ffc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21ffc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="21ffc-125">Authorization</span></span>  | <span data-ttu-id="21ffc-126">string</span><span class="sxs-lookup"><span data-stu-id="21ffc-126">string</span></span>  | <span data-ttu-id="21ffc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21ffc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21ffc-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21ffc-129">Accept</span></span> | <span data-ttu-id="21ffc-130">string</span><span class="sxs-lookup"><span data-stu-id="21ffc-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="21ffc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21ffc-131">Request body</span></span>
<span data-ttu-id="21ffc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21ffc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21ffc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21ffc-133">Response</span></span>

<span data-ttu-id="21ffc-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21ffc-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21ffc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21ffc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21ffc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21ffc-136">Request</span></span>
<span data-ttu-id="21ffc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21ffc-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21ffc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="21ffc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21ffc-139">C#</span><span class="sxs-lookup"><span data-stu-id="21ffc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21ffc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21ffc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21ffc-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="21ffc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21ffc-142">Java</span><span class="sxs-lookup"><span data-stu-id="21ffc-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21ffc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="21ffc-143">Response</span></span>
<span data-ttu-id="21ffc-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21ffc-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
