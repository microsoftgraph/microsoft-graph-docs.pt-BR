---
title: Listar sectionGroups
description: Recupere uma lista de grupos de seções do bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c5c4d292142c65ca5af962892816e8c3824dd7f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022709"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="157ea-103">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="157ea-103">List sectionGroups</span></span>

<span data-ttu-id="157ea-104">Recupere uma lista de [grupos de seções](../resources/sectiongroup.md) do bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="157ea-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="157ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="157ea-105">Permissions</span></span>
<span data-ttu-id="157ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="157ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="157ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="157ea-108">Permission type</span></span>      | <span data-ttu-id="157ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="157ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="157ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="157ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="157ea-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157ea-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="157ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="157ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157ea-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="157ea-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="157ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="157ea-114">Application</span></span> | <span data-ttu-id="157ea-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157ea-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="157ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="157ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="157ea-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="157ea-117">Optional query parameters</span></span>
<span data-ttu-id="157ea-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="157ea-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="157ea-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="157ea-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="157ea-120">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="157ea-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="157ea-121">Os `expand` valores válidos para os grupos `sections`de `sectionGroups`seção `parentNotebook`são, `parentSectionGroup`, e.</span><span class="sxs-lookup"><span data-stu-id="157ea-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="157ea-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="157ea-122">Request headers</span></span>
| <span data-ttu-id="157ea-123">Nome</span><span class="sxs-lookup"><span data-stu-id="157ea-123">Name</span></span>       | <span data-ttu-id="157ea-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="157ea-124">Type</span></span> | <span data-ttu-id="157ea-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="157ea-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="157ea-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="157ea-126">Authorization</span></span>  | <span data-ttu-id="157ea-127">string</span><span class="sxs-lookup"><span data-stu-id="157ea-127">string</span></span>  | <span data-ttu-id="157ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="157ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="157ea-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="157ea-130">Accept</span></span> | <span data-ttu-id="157ea-131">string</span><span class="sxs-lookup"><span data-stu-id="157ea-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="157ea-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="157ea-132">Request body</span></span>
<span data-ttu-id="157ea-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="157ea-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="157ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="157ea-134">Response</span></span>

<span data-ttu-id="157ea-135">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de objeto de [seção](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="157ea-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="157ea-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="157ea-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="157ea-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="157ea-137">Request</span></span>
<span data-ttu-id="157ea-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="157ea-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="157ea-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="157ea-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="157ea-140">C#</span><span class="sxs-lookup"><span data-stu-id="157ea-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="157ea-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="157ea-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="157ea-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="157ea-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="157ea-143">Java</span><span class="sxs-lookup"><span data-stu-id="157ea-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-get-sectiongroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="157ea-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="157ea-144">Response</span></span>
<span data-ttu-id="157ea-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="157ea-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
