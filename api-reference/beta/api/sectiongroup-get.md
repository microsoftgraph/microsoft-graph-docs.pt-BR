---
title: Obter sectionGroup
description: Recupere as propriedades e os relacionamentos de um objeto sectionGroup.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 2bacba09167724935123becbb5d8194385b5b215
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643423"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="aa029-103">Obter sectionGroup</span><span class="sxs-lookup"><span data-stu-id="aa029-103">Get sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa029-104">Recupere as propriedades e os relacionamentos de um objeto [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="aa029-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa029-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa029-105">Permissions</span></span>
<span data-ttu-id="aa029-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa029-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa029-108">Permission type</span></span>      | <span data-ttu-id="aa029-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa029-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa029-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa029-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa029-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa029-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa029-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa029-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa029-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa029-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="aa029-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa029-114">Application</span></span> | <span data-ttu-id="aa029-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa029-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa029-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa029-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa029-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa029-117">Optional query parameters</span></span>
<span data-ttu-id="aa029-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa029-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="aa029-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `name` e `self`. Os valores `expand` válidos para o grupo de seção são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="aa029-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa029-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa029-121">Request headers</span></span>
| <span data-ttu-id="aa029-122">Nome</span><span class="sxs-lookup"><span data-stu-id="aa029-122">Name</span></span>       | <span data-ttu-id="aa029-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa029-123">Type</span></span> | <span data-ttu-id="aa029-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa029-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa029-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa029-125">Authorization</span></span>  | <span data-ttu-id="aa029-126">string</span><span class="sxs-lookup"><span data-stu-id="aa029-126">string</span></span>  | <span data-ttu-id="aa029-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa029-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa029-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa029-129">Accept</span></span> | <span data-ttu-id="aa029-130">string</span><span class="sxs-lookup"><span data-stu-id="aa029-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="aa029-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa029-131">Request body</span></span>
<span data-ttu-id="aa029-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa029-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa029-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa029-133">Response</span></span>

<span data-ttu-id="aa029-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa029-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa029-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa029-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa029-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa029-136">Request</span></span>
<span data-ttu-id="aa029-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa029-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="aa029-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa029-138">Response</span></span>
<span data-ttu-id="aa029-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa029-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
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
    "Error: /api-reference/beta/api/sectiongroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
