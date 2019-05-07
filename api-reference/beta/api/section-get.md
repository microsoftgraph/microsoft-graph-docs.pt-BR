---
title: Obter seção
description: Recupere as propriedades e os relacionamentos de um objeto Section.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: df73036ca65ce0038430aed0f0c55635f02605a7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638855"
---
# <a name="get-section"></a><span data-ttu-id="5f0b5-103">Obter seção</span><span class="sxs-lookup"><span data-stu-id="5f0b5-103">Get section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f0b5-104">Recupere as propriedades e os relacionamentos de um objeto [Section](../resources/onenotesection.md) .</span><span class="sxs-lookup"><span data-stu-id="5f0b5-104">Retrieve the properties and relationships of a [section](../resources/onenotesection.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f0b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f0b5-105">Permissions</span></span>
<span data-ttu-id="5f0b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f0b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f0b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f0b5-108">Permission type</span></span>      | <span data-ttu-id="5f0b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f0b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f0b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f0b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f0b5-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f0b5-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f0b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f0b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f0b5-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f0b5-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5f0b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f0b5-114">Application</span></span> | <span data-ttu-id="5f0b5-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f0b5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f0b5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f0b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5f0b5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f0b5-117">Optional query parameters</span></span>
<span data-ttu-id="5f0b5-118">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5f0b5-119">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="5f0b5-119">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="5f0b5-120">Os `expand` valores válidos para as `parentNotebook` seções `parentSectionGroup`são e.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-120">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f0b5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f0b5-121">Request headers</span></span>
| <span data-ttu-id="5f0b5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5f0b5-122">Name</span></span>       | <span data-ttu-id="5f0b5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f0b5-123">Type</span></span> | <span data-ttu-id="5f0b5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f0b5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5f0b5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f0b5-125">Authorization</span></span>  | <span data-ttu-id="5f0b5-126">string</span><span class="sxs-lookup"><span data-stu-id="5f0b5-126">string</span></span>  | <span data-ttu-id="5f0b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f0b5-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f0b5-129">Accept</span></span> | <span data-ttu-id="5f0b5-130">string</span><span class="sxs-lookup"><span data-stu-id="5f0b5-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5f0b5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f0b5-131">Request body</span></span>
<span data-ttu-id="5f0b5-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f0b5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f0b5-133">Response</span></span>

<span data-ttu-id="5f0b5-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f0b5-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f0b5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f0b5-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f0b5-136">Request</span></span>
<span data-ttu-id="5f0b5-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="5f0b5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f0b5-138">Response</span></span>
<span data-ttu-id="5f0b5-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f0b5-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5f0b5-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5f0b5-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5f0b5-143">Basic</span><span class="sxs-lookup"><span data-stu-id="5f0b5-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_section-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f0b5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f0b5-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_section-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/section-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
