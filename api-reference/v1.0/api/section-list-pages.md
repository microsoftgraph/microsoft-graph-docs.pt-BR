---
title: Listar páginas
description: Recupere uma lista de objetos page da seção especificada.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8d5aae356a703968ca05317e653cad5b9a931161
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951366"
---
# <a name="list-pages"></a><span data-ttu-id="3acbc-103">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="3acbc-103">List pages</span></span>

<span data-ttu-id="3acbc-104">Recupere uma lista de objetos [page](../resources/page.md) da seção especificada.</span><span class="sxs-lookup"><span data-stu-id="3acbc-104">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="3acbc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3acbc-105">Permissions</span></span>
<span data-ttu-id="3acbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3acbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3acbc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3acbc-108">Permission type</span></span>      | <span data-ttu-id="3acbc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3acbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3acbc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3acbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3acbc-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acbc-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3acbc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3acbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3acbc-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3acbc-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3acbc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3acbc-114">Application</span></span> | <span data-ttu-id="3acbc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acbc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3acbc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3acbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3acbc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3acbc-117">Optional query parameters</span></span>
<span data-ttu-id="3acbc-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3acbc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="3acbc-p102">A consulta padrão das páginas retorna as 20 páginas principais ordenadas por `lastModifiedTime desc`. Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para passar pelo conjunto de resultados. o número máximo de páginas retornadas em uma solicitação `top` é 100.</span><span class="sxs-lookup"><span data-stu-id="3acbc-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="3acbc-p103">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="3acbc-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3acbc-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3acbc-124">Request headers</span></span>
| <span data-ttu-id="3acbc-125">Nome</span><span class="sxs-lookup"><span data-stu-id="3acbc-125">Name</span></span>       | <span data-ttu-id="3acbc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3acbc-126">Type</span></span> | <span data-ttu-id="3acbc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3acbc-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3acbc-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3acbc-128">Authorization</span></span>  | <span data-ttu-id="3acbc-129">string</span><span class="sxs-lookup"><span data-stu-id="3acbc-129">string</span></span>  | <span data-ttu-id="3acbc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3acbc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3acbc-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3acbc-132">Accept</span></span> | <span data-ttu-id="3acbc-133">string</span><span class="sxs-lookup"><span data-stu-id="3acbc-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3acbc-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3acbc-134">Request body</span></span>
<span data-ttu-id="3acbc-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3acbc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3acbc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3acbc-136">Response</span></span>

<span data-ttu-id="3acbc-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3acbc-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3acbc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3acbc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3acbc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3acbc-139">Request</span></span>
<span data-ttu-id="3acbc-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3acbc-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="3acbc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3acbc-141">Response</span></span>
<span data-ttu-id="3acbc-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3acbc-142">Here is an example of the response.</span></span> <span data-ttu-id="3acbc-143">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="3acbc-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="3acbc-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3acbc-144">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
