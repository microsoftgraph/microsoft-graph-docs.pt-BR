---
title: Listar seções
description: Recupere uma lista de objetos section do bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7ca40aede19e60b4c4b8462b917775a842643f68
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967715"
---
# <a name="list-sections"></a><span data-ttu-id="15c0d-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="15c0d-103">List sections</span></span>

<span data-ttu-id="15c0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15c0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15c0d-105">Recupere uma lista de objetos [Section](../resources/onenotesection.md) do bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="15c0d-105">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="15c0d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15c0d-106">Permissions</span></span>
<span data-ttu-id="15c0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c0d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15c0d-109">Permission type</span></span>      | <span data-ttu-id="15c0d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15c0d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15c0d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15c0d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15c0d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c0d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="15c0d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15c0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c0d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15c0d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="15c0d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15c0d-115">Application</span></span> | <span data-ttu-id="15c0d-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c0d-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15c0d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15c0d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15c0d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15c0d-118">Optional query parameters</span></span>
<span data-ttu-id="15c0d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15c0d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="15c0d-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="15c0d-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="15c0d-121">A consulta padrão expande `parentNotebook` e seleciona suas `id` `displayName` Propriedades, e `self` .</span><span class="sxs-lookup"><span data-stu-id="15c0d-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="15c0d-122">`expand`Os valores válidos para as seções são `parentNotebook` e `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="15c0d-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="15c0d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15c0d-123">Request headers</span></span>
| <span data-ttu-id="15c0d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="15c0d-124">Name</span></span>       | <span data-ttu-id="15c0d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="15c0d-125">Type</span></span> | <span data-ttu-id="15c0d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="15c0d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15c0d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="15c0d-127">Authorization</span></span>  | <span data-ttu-id="15c0d-128">string</span><span class="sxs-lookup"><span data-stu-id="15c0d-128">string</span></span>  | <span data-ttu-id="15c0d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15c0d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15c0d-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15c0d-131">Accept</span></span> | <span data-ttu-id="15c0d-132">string</span><span class="sxs-lookup"><span data-stu-id="15c0d-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="15c0d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15c0d-133">Request body</span></span>
<span data-ttu-id="15c0d-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15c0d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15c0d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15c0d-135">Response</span></span>

<span data-ttu-id="15c0d-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15c0d-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15c0d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15c0d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15c0d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15c0d-138">Request</span></span>
<span data-ttu-id="15c0d-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15c0d-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15c0d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="15c0d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="15c0d-141">C#</span><span class="sxs-lookup"><span data-stu-id="15c0d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15c0d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15c0d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15c0d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15c0d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15c0d-144">Java</span><span class="sxs-lookup"><span data-stu-id="15c0d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15c0d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="15c0d-145">Response</span></span>
<span data-ttu-id="15c0d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15c0d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
