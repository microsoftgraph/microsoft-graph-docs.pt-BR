---
title: Listar seções
description: Recupere uma lista de objetos onenoteSection do grupo de seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4cbf57f87d7f6d7d9a2cabe5c25e20043fe0224a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882985"
---
# <a name="list-sections"></a><span data-ttu-id="4d03f-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="4d03f-103">List sections</span></span>

<span data-ttu-id="4d03f-104">Recupere uma lista de objetos [onenoteSection](../resources/section.md) do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="4d03f-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d03f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d03f-105">Permissions</span></span>
<span data-ttu-id="4d03f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d03f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d03f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d03f-108">Permission type</span></span>      | <span data-ttu-id="4d03f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d03f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d03f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d03f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d03f-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d03f-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d03f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d03f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d03f-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d03f-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4d03f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d03f-114">Application</span></span> | <span data-ttu-id="4d03f-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d03f-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d03f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d03f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4d03f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d03f-117">Optional query parameters</span></span>
<span data-ttu-id="4d03f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d03f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4d03f-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="4d03f-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="4d03f-120">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="4d03f-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="4d03f-121">Os `expand` valores válidos para as `parentNotebook` seções `parentSectionGroup`são e.</span><span class="sxs-lookup"><span data-stu-id="4d03f-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="4d03f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d03f-122">Request headers</span></span>
| <span data-ttu-id="4d03f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4d03f-123">Name</span></span>       | <span data-ttu-id="4d03f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d03f-124">Type</span></span> | <span data-ttu-id="4d03f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d03f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4d03f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d03f-126">Authorization</span></span>  | <span data-ttu-id="4d03f-127">string</span><span class="sxs-lookup"><span data-stu-id="4d03f-127">string</span></span>  | <span data-ttu-id="4d03f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d03f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d03f-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d03f-130">Accept</span></span> | <span data-ttu-id="4d03f-131">string</span><span class="sxs-lookup"><span data-stu-id="4d03f-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4d03f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d03f-132">Request body</span></span>
<span data-ttu-id="4d03f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d03f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d03f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d03f-134">Response</span></span>

<span data-ttu-id="4d03f-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d03f-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d03f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d03f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d03f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d03f-137">Request</span></span>
<span data-ttu-id="4d03f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d03f-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d03f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d03f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sectionsgroup_get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d03f-140">C#</span><span class="sxs-lookup"><span data-stu-id="4d03f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sectionsgroup-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d03f-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d03f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sectionsgroup-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d03f-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d03f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sectionsgroup-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4d03f-143">Java</span><span class="sxs-lookup"><span data-stu-id="4d03f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sectionsgroup-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d03f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d03f-144">Response</span></span>
<span data-ttu-id="4d03f-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d03f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
