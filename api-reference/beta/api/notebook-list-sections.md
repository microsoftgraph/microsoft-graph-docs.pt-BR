---
title: Listar seções
description: Recupere uma lista de objetos section do bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ac308e7c7578b366dc624e59bfd8de0c39791738
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456704"
---
# <a name="list-sections"></a><span data-ttu-id="6234c-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="6234c-103">List sections</span></span>

<span data-ttu-id="6234c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6234c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6234c-105">Recupere uma lista de objetos [Section](../resources/onenotesection.md) do bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="6234c-105">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="6234c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6234c-106">Permissions</span></span>
<span data-ttu-id="6234c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6234c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6234c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6234c-109">Permission type</span></span>      | <span data-ttu-id="6234c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6234c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6234c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6234c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6234c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6234c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6234c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6234c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6234c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6234c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6234c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6234c-115">Application</span></span> | <span data-ttu-id="6234c-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6234c-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6234c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6234c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6234c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6234c-118">Optional query parameters</span></span>
<span data-ttu-id="6234c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6234c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6234c-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="6234c-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="6234c-121">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="6234c-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="6234c-122">Os `expand` valores válidos para as `parentNotebook` seções `parentSectionGroup`são e.</span><span class="sxs-lookup"><span data-stu-id="6234c-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="6234c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6234c-123">Request headers</span></span>
| <span data-ttu-id="6234c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6234c-124">Name</span></span>       | <span data-ttu-id="6234c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6234c-125">Type</span></span> | <span data-ttu-id="6234c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6234c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6234c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6234c-127">Authorization</span></span>  | <span data-ttu-id="6234c-128">string</span><span class="sxs-lookup"><span data-stu-id="6234c-128">string</span></span>  | <span data-ttu-id="6234c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6234c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6234c-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6234c-131">Accept</span></span> | <span data-ttu-id="6234c-132">string</span><span class="sxs-lookup"><span data-stu-id="6234c-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6234c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6234c-133">Request body</span></span>
<span data-ttu-id="6234c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6234c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6234c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6234c-135">Response</span></span>

<span data-ttu-id="6234c-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6234c-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6234c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6234c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6234c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6234c-138">Request</span></span>
<span data-ttu-id="6234c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6234c-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6234c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6234c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="6234c-141">C#</span><span class="sxs-lookup"><span data-stu-id="6234c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6234c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6234c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6234c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6234c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6234c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6234c-144">Response</span></span>
<span data-ttu-id="6234c-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6234c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
