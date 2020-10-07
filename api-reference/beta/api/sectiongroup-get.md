---
title: Obter o myseção
description: Recupere as propriedades e os relacionamentos de um objeto de objeto de seção.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: def145671066b44dc63eadb070a0960a9e9f890a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374235"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="4368c-103">Obter o myseção</span><span class="sxs-lookup"><span data-stu-id="4368c-103">Get sectionGroup</span></span>

<span data-ttu-id="4368c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4368c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4368c-105">Recupere as propriedades e os relacionamentos de um objeto de objeto de [seção](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4368c-105">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4368c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4368c-106">Permissions</span></span>
<span data-ttu-id="4368c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4368c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4368c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4368c-109">Permission type</span></span>      | <span data-ttu-id="4368c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4368c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4368c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4368c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4368c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4368c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4368c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4368c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4368c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4368c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4368c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4368c-115">Application</span></span> | <span data-ttu-id="4368c-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4368c-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4368c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4368c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4368c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4368c-118">Optional query parameters</span></span>
<span data-ttu-id="4368c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4368c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="4368c-120">A consulta padrão expande `parentNotebook` e seleciona suas `id` `name` Propriedades, e `self` .</span><span class="sxs-lookup"><span data-stu-id="4368c-120">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="4368c-121">`expand`Os valores válidos para os grupos de seções são `parentNotebook` e `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="4368c-121">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4368c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4368c-122">Request headers</span></span>
| <span data-ttu-id="4368c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4368c-123">Name</span></span>       | <span data-ttu-id="4368c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="4368c-124">Type</span></span> | <span data-ttu-id="4368c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4368c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4368c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4368c-126">Authorization</span></span>  | <span data-ttu-id="4368c-127">string</span><span class="sxs-lookup"><span data-stu-id="4368c-127">string</span></span>  | <span data-ttu-id="4368c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4368c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4368c-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4368c-130">Accept</span></span> | <span data-ttu-id="4368c-131">string</span><span class="sxs-lookup"><span data-stu-id="4368c-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4368c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4368c-132">Request body</span></span>
<span data-ttu-id="4368c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4368c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4368c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4368c-134">Response</span></span>

<span data-ttu-id="4368c-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4368c-135">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4368c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4368c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4368c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4368c-137">Request</span></span>
<span data-ttu-id="4368c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4368c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4368c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4368c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="4368c-140">C#</span><span class="sxs-lookup"><span data-stu-id="4368c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4368c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4368c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4368c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4368c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4368c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4368c-143">Response</span></span>
<span data-ttu-id="4368c-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4368c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
