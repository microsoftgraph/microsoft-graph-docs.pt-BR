---
title: Listar sectionGroups
description: Recupere uma lista de grupos de seção do grupo de seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65fa81d9e4fd7632d177d484abd374522fa42e81
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638841"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="62570-103">Listar sectionGroups</span><span class="sxs-lookup"><span data-stu-id="62570-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62570-104">Recupere uma lista de [grupos de seção](../resources/sectiongroup.md) do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="62570-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="62570-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62570-105">Permissions</span></span>
<span data-ttu-id="62570-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62570-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62570-108">Permission type</span></span>      | <span data-ttu-id="62570-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62570-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62570-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62570-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62570-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62570-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="62570-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62570-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62570-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62570-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="62570-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62570-114">Application</span></span> | <span data-ttu-id="62570-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62570-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62570-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62570-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="62570-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62570-117">Optional query parameters</span></span>
<span data-ttu-id="62570-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62570-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="62570-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="62570-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="62570-120">A consulta padrão expande `parentNotebook` e seleciona suas `id`propriedades `displayName`, e `self` .</span><span class="sxs-lookup"><span data-stu-id="62570-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="62570-121">Os `expand` valores válidos para os grupos `sections`de `sectionGroups`seção `parentNotebook`são, `parentSectionGroup`, e.</span><span class="sxs-lookup"><span data-stu-id="62570-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62570-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62570-122">Request headers</span></span>
| <span data-ttu-id="62570-123">Nome</span><span class="sxs-lookup"><span data-stu-id="62570-123">Name</span></span>       | <span data-ttu-id="62570-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="62570-124">Type</span></span> | <span data-ttu-id="62570-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="62570-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="62570-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="62570-126">Authorization</span></span>  | <span data-ttu-id="62570-127">string</span><span class="sxs-lookup"><span data-stu-id="62570-127">string</span></span>  | <span data-ttu-id="62570-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62570-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62570-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62570-130">Accept</span></span> | <span data-ttu-id="62570-131">string</span><span class="sxs-lookup"><span data-stu-id="62570-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="62570-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62570-132">Request body</span></span>
<span data-ttu-id="62570-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62570-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62570-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="62570-134">Response</span></span>

<span data-ttu-id="62570-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de objeto de [seção](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62570-135">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62570-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62570-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62570-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62570-137">Request</span></span>
<span data-ttu-id="62570-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62570-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="62570-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="62570-139">Response</span></span>
<span data-ttu-id="62570-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62570-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="62570-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="62570-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62570-144">Basic</span><span class="sxs-lookup"><span data-stu-id="62570-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62570-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62570-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sectiongroup-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
