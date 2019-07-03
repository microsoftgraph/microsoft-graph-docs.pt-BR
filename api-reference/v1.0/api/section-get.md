---
title: Obter seção
description: Recupere as propriedades e os relacionamentos de um objeto onenoteSection.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8f1a66c85835fab94541553843e45109f61e4bf5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461516"
---
# <a name="get-section"></a><span data-ttu-id="e8437-103">Obter seção</span><span class="sxs-lookup"><span data-stu-id="e8437-103">Get section</span></span>

<span data-ttu-id="e8437-104">Recupere as propriedades e os relacionamentos de um objeto [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="e8437-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8437-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8437-105">Permissions</span></span>
<span data-ttu-id="e8437-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8437-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8437-108">Permission type</span></span>      | <span data-ttu-id="e8437-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8437-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8437-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8437-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8437-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8437-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8437-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8437-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8437-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8437-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e8437-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8437-114">Application</span></span> | <span data-ttu-id="e8437-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8437-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8437-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8437-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8437-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8437-117">Optional query parameters</span></span>
<span data-ttu-id="e8437-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8437-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e8437-119">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="e8437-119">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="e8437-120">Os `expand` valores válidos para as `parentNotebook` seções `parentSectionGroup`são e.</span><span class="sxs-lookup"><span data-stu-id="e8437-120">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8437-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8437-121">Request headers</span></span>
| <span data-ttu-id="e8437-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8437-122">Name</span></span>       | <span data-ttu-id="e8437-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8437-123">Type</span></span> | <span data-ttu-id="e8437-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8437-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8437-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8437-125">Authorization</span></span>  | <span data-ttu-id="e8437-126">string</span><span class="sxs-lookup"><span data-stu-id="e8437-126">string</span></span>  | <span data-ttu-id="e8437-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8437-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8437-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8437-129">Accept</span></span> | <span data-ttu-id="e8437-130">string</span><span class="sxs-lookup"><span data-stu-id="e8437-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e8437-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8437-131">Request body</span></span>
<span data-ttu-id="e8437-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8437-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8437-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8437-133">Response</span></span>

<span data-ttu-id="e8437-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8437-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8437-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8437-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8437-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8437-136">Request</span></span>
<span data-ttu-id="e8437-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8437-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8437-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8437-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8437-139">C#</span><span class="sxs-lookup"><span data-stu-id="e8437-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8437-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8437-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8437-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e8437-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8437-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8437-142">Response</span></span>
<span data-ttu-id="e8437-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8437-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
