---
title: Listar sectionGroups
description: Recupere uma lista de objetos de objeto de seção.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: d79854013bb166a4fa603edff130d626b6408b1c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511317"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="69ea0-103">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="69ea0-103">List sectionGroups</span></span>

<span data-ttu-id="69ea0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ea0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69ea0-105">Recupere uma lista de objetos de objeto de [seção](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="69ea0-105">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="69ea0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69ea0-106">Permissions</span></span>
<span data-ttu-id="69ea0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ea0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69ea0-109">Permission type</span></span>      | <span data-ttu-id="69ea0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69ea0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69ea0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69ea0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69ea0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ea0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="69ea0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69ea0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ea0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ea0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="69ea0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69ea0-115">Application</span></span> | <span data-ttu-id="69ea0-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ea0-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69ea0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69ea0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69ea0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="69ea0-118">Optional query parameters</span></span>
<span data-ttu-id="69ea0-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="69ea0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="69ea0-120">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="69ea0-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="69ea0-121">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="69ea0-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="69ea0-122">Os `expand` valores válidos para os grupos `sections`de `sectionGroups`seção `parentNotebook`são, `parentSectionGroup`, e.</span><span class="sxs-lookup"><span data-stu-id="69ea0-122">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69ea0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69ea0-123">Request headers</span></span>
| <span data-ttu-id="69ea0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="69ea0-124">Name</span></span>       | <span data-ttu-id="69ea0-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="69ea0-125">Type</span></span> | <span data-ttu-id="69ea0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="69ea0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69ea0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="69ea0-127">Authorization</span></span>  | <span data-ttu-id="69ea0-128">string</span><span class="sxs-lookup"><span data-stu-id="69ea0-128">string</span></span>  | <span data-ttu-id="69ea0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69ea0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69ea0-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69ea0-131">Accept</span></span> | <span data-ttu-id="69ea0-132">string</span><span class="sxs-lookup"><span data-stu-id="69ea0-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="69ea0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69ea0-133">Request body</span></span>
<span data-ttu-id="69ea0-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69ea0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69ea0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ea0-135">Response</span></span>

<span data-ttu-id="69ea0-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de objeto de [seção](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69ea0-136">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69ea0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69ea0-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69ea0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69ea0-138">Request</span></span>
<span data-ttu-id="69ea0-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69ea0-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69ea0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="69ea0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sectiongroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
# <a name="c"></a>[<span data-ttu-id="69ea0-141">C#</span><span class="sxs-lookup"><span data-stu-id="69ea0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69ea0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69ea0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69ea0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69ea0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69ea0-144">Java</span><span class="sxs-lookup"><span data-stu-id="69ea0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/onenote-get-sectiongroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69ea0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ea0-145">Response</span></span>
<span data-ttu-id="69ea0-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69ea0-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
