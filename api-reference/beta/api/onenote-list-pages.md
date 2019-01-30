---
title: Listar páginas
description: Recuperar uma lista de objetos page.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 4717428dc7b45d893993dd366eb33137000d3bb3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640795"
---
# <a name="list-pages"></a><span data-ttu-id="a27f5-103">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="a27f5-103">List pages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a27f5-104">Recuperar uma lista de objetos [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="a27f5-104">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a27f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a27f5-105">Permissions</span></span>
<span data-ttu-id="a27f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a27f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27f5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a27f5-108">Permission type</span></span>      | <span data-ttu-id="a27f5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a27f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a27f5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a27f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a27f5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a27f5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a27f5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a27f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a27f5-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27f5-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a27f5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a27f5-114">Application</span></span> | <span data-ttu-id="a27f5-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a27f5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a27f5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a27f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a27f5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a27f5-117">Optional query parameters</span></span>
<span data-ttu-id="a27f5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a27f5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a27f5-p102">A consulta padrão das páginas retorna as 20 páginas principais ordenadas por `lastModifiedTime desc`. Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para passar pelo conjunto de resultados. o número máximo de páginas retornadas em uma solicitação `top` é 100.</span><span class="sxs-lookup"><span data-stu-id="a27f5-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="a27f5-p103">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `displayName` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="a27f5-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a27f5-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a27f5-124">Request headers</span></span>
| <span data-ttu-id="a27f5-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a27f5-125">Name</span></span>       | <span data-ttu-id="a27f5-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a27f5-126">Type</span></span> | <span data-ttu-id="a27f5-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a27f5-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a27f5-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a27f5-128">Authorization</span></span>  | <span data-ttu-id="a27f5-129">string</span><span class="sxs-lookup"><span data-stu-id="a27f5-129">string</span></span>  | <span data-ttu-id="a27f5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a27f5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a27f5-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a27f5-132">Accept</span></span> | <span data-ttu-id="a27f5-133">string</span><span class="sxs-lookup"><span data-stu-id="a27f5-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a27f5-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a27f5-134">Request body</span></span>
<span data-ttu-id="a27f5-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a27f5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a27f5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27f5-136">Response</span></span>

<span data-ttu-id="a27f5-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27f5-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a27f5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a27f5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a27f5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a27f5-139">Request</span></span>
<span data-ttu-id="a27f5-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a27f5-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="a27f5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27f5-141">Response</span></span>
<span data-ttu-id="a27f5-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27f5-142">Here is an example of the response.</span></span> <span data-ttu-id="a27f5-143">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="a27f5-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="a27f5-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a27f5-144">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
    {
      "title": "title-value",
      "createdByAppId": "createdByAppId-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      },
      "contentUrl": "contentUrl-value",
      "content": "content-value",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-list-pages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
