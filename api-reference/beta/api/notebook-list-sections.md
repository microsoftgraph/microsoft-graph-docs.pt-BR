---
title: Listar seções
description: Recupere uma lista de objetos section do bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fe412cb68020423832648d23f862a3ddf97825f1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723872"
---
# <a name="list-sections"></a><span data-ttu-id="23cf1-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="23cf1-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23cf1-104">Recupere uma lista de objetos [Section](../resources/onenotesection.md) do bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="23cf1-104">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="23cf1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="23cf1-105">Permissions</span></span>
<span data-ttu-id="23cf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23cf1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23cf1-108">Permission type</span></span>      | <span data-ttu-id="23cf1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23cf1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23cf1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23cf1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23cf1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cf1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="23cf1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23cf1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23cf1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23cf1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="23cf1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23cf1-114">Application</span></span> | <span data-ttu-id="23cf1-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cf1-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23cf1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23cf1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23cf1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23cf1-117">Optional query parameters</span></span>
<span data-ttu-id="23cf1-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23cf1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="23cf1-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="23cf1-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="23cf1-120">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="23cf1-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="23cf1-121">Os `expand` valores válidos para as `parentNotebook` seções `parentSectionGroup`são e.</span><span class="sxs-lookup"><span data-stu-id="23cf1-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="23cf1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23cf1-122">Request headers</span></span>
| <span data-ttu-id="23cf1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="23cf1-123">Name</span></span>       | <span data-ttu-id="23cf1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cf1-124">Type</span></span> | <span data-ttu-id="23cf1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cf1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23cf1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="23cf1-126">Authorization</span></span>  | <span data-ttu-id="23cf1-127">string</span><span class="sxs-lookup"><span data-stu-id="23cf1-127">string</span></span>  | <span data-ttu-id="23cf1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23cf1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23cf1-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23cf1-130">Accept</span></span> | <span data-ttu-id="23cf1-131">string</span><span class="sxs-lookup"><span data-stu-id="23cf1-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="23cf1-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23cf1-132">Request body</span></span>
<span data-ttu-id="23cf1-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23cf1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23cf1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cf1-134">Response</span></span>

<span data-ttu-id="23cf1-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23cf1-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23cf1-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23cf1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23cf1-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23cf1-137">Request</span></span>
<span data-ttu-id="23cf1-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23cf1-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23cf1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="23cf1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23cf1-140">C#</span><span class="sxs-lookup"><span data-stu-id="23cf1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23cf1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23cf1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23cf1-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="23cf1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23cf1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cf1-143">Response</span></span>
<span data-ttu-id="23cf1-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23cf1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "isDefault": true,
      "pagesUrl": "pagesUrl-value",
      "displayName": "name-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
