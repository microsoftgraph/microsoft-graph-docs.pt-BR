---
title: Listar seções
description: Recupere uma lista de objetos Section.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e4672fd9a2858d7f39d1ed6952c262da4af5a1fa
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461332"
---
# <a name="list-sections"></a><span data-ttu-id="c7b59-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="c7b59-103">List sections</span></span>

<span data-ttu-id="c7b59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7b59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7b59-105">Recupere uma lista de objetos [Section](../resources/onenotesection.md) .</span><span class="sxs-lookup"><span data-stu-id="c7b59-105">Retrieve a list of [section](../resources/onenotesection.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7b59-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7b59-106">Permissions</span></span>
<span data-ttu-id="c7b59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7b59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7b59-109">Permission type</span></span>      | <span data-ttu-id="c7b59-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7b59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7b59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7b59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7b59-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7b59-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7b59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7b59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7b59-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7b59-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c7b59-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7b59-115">Application</span></span> | <span data-ttu-id="c7b59-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7b59-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7b59-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7b59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7b59-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7b59-118">Optional query parameters</span></span>
<span data-ttu-id="c7b59-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7b59-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="c7b59-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c7b59-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="c7b59-121">A consulta padrão expande `parentNotebook` e seleciona suas `id` `displayName` Propriedades, e `self` .</span><span class="sxs-lookup"><span data-stu-id="c7b59-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="c7b59-122">`expand`Os valores válidos para as seções são `parentNotebook` e `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="c7b59-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7b59-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7b59-123">Request headers</span></span>
| <span data-ttu-id="c7b59-124">Nome</span><span class="sxs-lookup"><span data-stu-id="c7b59-124">Name</span></span>       | <span data-ttu-id="c7b59-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7b59-125">Type</span></span> | <span data-ttu-id="c7b59-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7b59-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7b59-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7b59-127">Authorization</span></span>  | <span data-ttu-id="c7b59-128">string</span><span class="sxs-lookup"><span data-stu-id="c7b59-128">string</span></span>  | <span data-ttu-id="c7b59-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7b59-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7b59-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7b59-131">Accept</span></span> | <span data-ttu-id="c7b59-132">string</span><span class="sxs-lookup"><span data-stu-id="c7b59-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c7b59-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7b59-133">Request body</span></span>
<span data-ttu-id="c7b59-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7b59-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7b59-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7b59-135">Response</span></span>

<span data-ttu-id="c7b59-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [onenoteSection](../resources/onenotesection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7b59-136">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7b59-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7b59-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7b59-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7b59-138">Request</span></span>
<span data-ttu-id="c7b59-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7b59-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7b59-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7b59-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sections
```
# <a name="c"></a>[<span data-ttu-id="c7b59-141">C#</span><span class="sxs-lookup"><span data-stu-id="c7b59-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7b59-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7b59-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7b59-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7b59-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7b59-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7b59-144">Response</span></span>
<span data-ttu-id="c7b59-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7b59-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
