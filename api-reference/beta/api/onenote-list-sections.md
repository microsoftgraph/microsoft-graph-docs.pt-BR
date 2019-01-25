---
title: Listar seções
description: Recupere uma lista de objetos section.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d5f01799877ed86bc9802de9f2d3cb4b417a3167
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516683"
---
# <a name="list-sections"></a><span data-ttu-id="b8d9a-103">Listar seções</span><span class="sxs-lookup"><span data-stu-id="b8d9a-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d9a-104">Recupere uma lista de objetos [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="b8d9a-104">Retrieve a list of [section](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8d9a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8d9a-105">Permissions</span></span>
<span data-ttu-id="b8d9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d9a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8d9a-108">Permission type</span></span>      | <span data-ttu-id="b8d9a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8d9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8d9a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8d9a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8d9a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d9a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8d9a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8d9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d9a-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8d9a-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b8d9a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8d9a-114">Application</span></span> | <span data-ttu-id="b8d9a-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d9a-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8d9a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8d9a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8d9a-117">Optional query parameters</span></span>
<span data-ttu-id="b8d9a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b8d9a-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="b8d9a-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8d9a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d9a-122">Request headers</span></span>
| <span data-ttu-id="b8d9a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b8d9a-123">Name</span></span>       | <span data-ttu-id="b8d9a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8d9a-124">Type</span></span> | <span data-ttu-id="b8d9a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d9a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8d9a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8d9a-126">Authorization</span></span>  | <span data-ttu-id="b8d9a-127">string</span><span class="sxs-lookup"><span data-stu-id="b8d9a-127">string</span></span>  | <span data-ttu-id="b8d9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8d9a-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8d9a-130">Accept</span></span> | <span data-ttu-id="b8d9a-131">string</span><span class="sxs-lookup"><span data-stu-id="b8d9a-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b8d9a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d9a-132">Request body</span></span>
<span data-ttu-id="b8d9a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8d9a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d9a-134">Response</span></span>

<span data-ttu-id="b8d9a-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-135">If successful, this method returns a `200 OK` response code and collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8d9a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8d9a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8d9a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d9a-137">Request</span></span>
<span data-ttu-id="b8d9a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections
```
##### <a name="response"></a><span data-ttu-id="b8d9a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d9a-139">Response</span></span>
<span data-ttu-id="b8d9a-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8d9a-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/onenote-list-sections.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
