---
title: Obter o myseção
description: Recupere as propriedades e os relacionamentos de um objeto de objeto de seção.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7f3c2d8d489f6b8e97f602ca5e470085a3858db1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272818"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="3c402-103">Obter o myseção</span><span class="sxs-lookup"><span data-stu-id="3c402-103">Get sectionGroup</span></span>

<span data-ttu-id="3c402-104">Recupere as propriedades e os relacionamentos de um objeto de objeto de [seção](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="3c402-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c402-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c402-105">Permissions</span></span>
<span data-ttu-id="3c402-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c402-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c402-108">Permission type</span></span>      | <span data-ttu-id="3c402-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c402-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c402-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c402-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c402-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c402-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c402-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c402-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c402-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c402-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3c402-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c402-114">Application</span></span> | <span data-ttu-id="3c402-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c402-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c402-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c402-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c402-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c402-117">Optional query parameters</span></span>
<span data-ttu-id="3c402-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c402-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3c402-119">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `name`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="3c402-119">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="3c402-120">Os `expand` valores válidos para os grupos `parentNotebook` de `parentSectionGroup`seções são e.</span><span class="sxs-lookup"><span data-stu-id="3c402-120">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c402-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c402-121">Request headers</span></span>
| <span data-ttu-id="3c402-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3c402-122">Name</span></span>       | <span data-ttu-id="3c402-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c402-123">Type</span></span> | <span data-ttu-id="3c402-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c402-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c402-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c402-125">Authorization</span></span>  | <span data-ttu-id="3c402-126">string</span><span class="sxs-lookup"><span data-stu-id="3c402-126">string</span></span>  | <span data-ttu-id="3c402-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c402-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c402-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c402-129">Accept</span></span> | <span data-ttu-id="3c402-130">string</span><span class="sxs-lookup"><span data-stu-id="3c402-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3c402-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c402-131">Request body</span></span>
<span data-ttu-id="3c402-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c402-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c402-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c402-133">Response</span></span>

<span data-ttu-id="3c402-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c402-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c402-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c402-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c402-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c402-136">Request</span></span>
<span data-ttu-id="3c402-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c402-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="3c402-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c402-138">Response</span></span>
<span data-ttu-id="3c402-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c402-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c402-142">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="3c402-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c402-143">C#</span><span class="sxs-lookup"><span data-stu-id="3c402-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c402-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c402-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3c402-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3c402-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_sectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/sectiongroup-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/sectiongroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/sectiongroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
