---
title: Obter seção
description: Recupere as propriedades e os relacionamentos de um objeto onenoteSection.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: bbcd2c5a70e816da8b039b9b2ba81f48640070fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088935"
---
# <a name="get-section"></a><span data-ttu-id="9185a-103">Obter seção</span><span class="sxs-lookup"><span data-stu-id="9185a-103">Get section</span></span>

<span data-ttu-id="9185a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9185a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9185a-105">Recupere as propriedades e os relacionamentos de um objeto [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="9185a-105">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9185a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9185a-106">Permissions</span></span>
<span data-ttu-id="9185a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9185a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9185a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9185a-109">Permission type</span></span>      | <span data-ttu-id="9185a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9185a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9185a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9185a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9185a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9185a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9185a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9185a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9185a-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9185a-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9185a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9185a-115">Application</span></span> | <span data-ttu-id="9185a-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9185a-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9185a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9185a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9185a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9185a-118">Optional query parameters</span></span>
<span data-ttu-id="9185a-119">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9185a-119">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9185a-120">A consulta padrão expande `parentNotebook` e seleciona suas `id` `displayName` Propriedades, e `self` .</span><span class="sxs-lookup"><span data-stu-id="9185a-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="9185a-121">`expand`Os valores válidos para as seções são `parentNotebook` e `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="9185a-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9185a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9185a-122">Request headers</span></span>
| <span data-ttu-id="9185a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9185a-123">Name</span></span>       | <span data-ttu-id="9185a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="9185a-124">Type</span></span> | <span data-ttu-id="9185a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9185a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9185a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9185a-126">Authorization</span></span>  | <span data-ttu-id="9185a-127">string</span><span class="sxs-lookup"><span data-stu-id="9185a-127">string</span></span>  | <span data-ttu-id="9185a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9185a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9185a-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9185a-130">Accept</span></span> | <span data-ttu-id="9185a-131">string</span><span class="sxs-lookup"><span data-stu-id="9185a-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9185a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9185a-132">Request body</span></span>
<span data-ttu-id="9185a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9185a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9185a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9185a-134">Response</span></span>

<span data-ttu-id="9185a-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9185a-135">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9185a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9185a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9185a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9185a-137">Request</span></span>
<span data-ttu-id="9185a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9185a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9185a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9185a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
# <a name="c"></a>[<span data-ttu-id="9185a-140">C#</span><span class="sxs-lookup"><span data-stu-id="9185a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9185a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9185a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9185a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9185a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9185a-143">Java</span><span class="sxs-lookup"><span data-stu-id="9185a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-section-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9185a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9185a-144">Response</span></span>
<span data-ttu-id="9185a-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9185a-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

