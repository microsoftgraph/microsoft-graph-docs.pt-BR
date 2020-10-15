---
title: Obter o myseção
description: Recupere as propriedades e os relacionamentos de um objeto de objeto de seção.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 0e15caf09b1955bb583a63e767856ac03684ff16
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458896"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="e0f6d-103">Obter o myseção</span><span class="sxs-lookup"><span data-stu-id="e0f6d-103">Get sectionGroup</span></span>

<span data-ttu-id="e0f6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0f6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0f6d-105">Recupere as propriedades e os relacionamentos de um objeto de objeto de [seção](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="e0f6d-105">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0f6d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e0f6d-106">Permissions</span></span>
<span data-ttu-id="e0f6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0f6d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0f6d-109">Permission type</span></span>      | <span data-ttu-id="e0f6d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0f6d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0f6d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0f6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0f6d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f6d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0f6d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0f6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0f6d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0f6d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e0f6d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0f6d-115">Application</span></span> | <span data-ttu-id="e0f6d-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0f6d-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0f6d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0f6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0f6d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0f6d-118">Optional query parameters</span></span>
<span data-ttu-id="e0f6d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="e0f6d-120">A consulta padrão expande `parentNotebook` e seleciona suas `id` `name` Propriedades, e `self` .</span><span class="sxs-lookup"><span data-stu-id="e0f6d-120">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="e0f6d-121">`expand`Os valores válidos para os grupos de seções são `parentNotebook` e `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="e0f6d-121">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0f6d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f6d-122">Request headers</span></span>
| <span data-ttu-id="e0f6d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e0f6d-123">Name</span></span>       | <span data-ttu-id="e0f6d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0f6d-124">Type</span></span> | <span data-ttu-id="e0f6d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0f6d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0f6d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0f6d-126">Authorization</span></span>  | <span data-ttu-id="e0f6d-127">string</span><span class="sxs-lookup"><span data-stu-id="e0f6d-127">string</span></span>  | <span data-ttu-id="e0f6d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0f6d-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0f6d-130">Accept</span></span> | <span data-ttu-id="e0f6d-131">string</span><span class="sxs-lookup"><span data-stu-id="e0f6d-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e0f6d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f6d-132">Request body</span></span>
<span data-ttu-id="e0f6d-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0f6d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0f6d-134">Response</span></span>

<span data-ttu-id="e0f6d-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-135">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0f6d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0f6d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0f6d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f6d-137">Request</span></span>
<span data-ttu-id="e0f6d-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0f6d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0f6d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="e0f6d-140">C#</span><span class="sxs-lookup"><span data-stu-id="e0f6d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0f6d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0f6d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0f6d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0f6d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0f6d-143">Java</span><span class="sxs-lookup"><span data-stu-id="e0f6d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0f6d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0f6d-144">Response</span></span>
<span data-ttu-id="e0f6d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0f6d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
