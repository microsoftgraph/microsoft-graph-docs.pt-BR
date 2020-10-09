---
title: Listar páginas
description: Recupere uma lista de objetos Page.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a3ad29002ed42330937bd6b64d396e403467d889
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405999"
---
# <a name="list-pages"></a><span data-ttu-id="b7417-103">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="b7417-103">List pages</span></span>

<span data-ttu-id="b7417-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7417-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7417-105">Recupere uma lista de objetos [Page](../resources/page.md) .</span><span class="sxs-lookup"><span data-stu-id="b7417-105">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7417-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7417-106">Permissions</span></span>
<span data-ttu-id="b7417-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7417-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7417-109">Permission type</span></span>      | <span data-ttu-id="b7417-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7417-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7417-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7417-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7417-112">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7417-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7417-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7417-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7417-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7417-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b7417-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7417-115">Application</span></span> | <span data-ttu-id="b7417-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7417-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7417-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7417-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7417-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7417-118">Optional query parameters</span></span>
<span data-ttu-id="b7417-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7417-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="b7417-120">A consulta padrão para páginas retorna as 20 principais páginas ordenadas por `lastModifiedTime desc` .</span><span class="sxs-lookup"><span data-stu-id="b7417-120">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="b7417-121">Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para percorrer o conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="b7417-121">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="b7417-122">O número máximo de páginas retornadas para uma `top` solicitação é 100.</span><span class="sxs-lookup"><span data-stu-id="b7417-122">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="b7417-123">A resposta padrão expande `parentSection` e seleciona as `id` `displayName` Propriedades, e e `self` .</span><span class="sxs-lookup"><span data-stu-id="b7417-123">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="b7417-124">`expand`Os valores válidos para páginas são `parentNotebook` e `parentSection` .</span><span class="sxs-lookup"><span data-stu-id="b7417-124">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7417-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7417-125">Request headers</span></span>
| <span data-ttu-id="b7417-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b7417-126">Name</span></span>       | <span data-ttu-id="b7417-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7417-127">Type</span></span> | <span data-ttu-id="b7417-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7417-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7417-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7417-129">Authorization</span></span>  | <span data-ttu-id="b7417-130">string</span><span class="sxs-lookup"><span data-stu-id="b7417-130">string</span></span>  | <span data-ttu-id="b7417-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7417-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7417-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7417-133">Accept</span></span> | <span data-ttu-id="b7417-134">string</span><span class="sxs-lookup"><span data-stu-id="b7417-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b7417-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7417-135">Request body</span></span>
<span data-ttu-id="b7417-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7417-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7417-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7417-137">Response</span></span>

<span data-ttu-id="b7417-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7417-138">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7417-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7417-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7417-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7417-140">Request</span></span>
<span data-ttu-id="b7417-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7417-141">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="b7417-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7417-142">Response</span></span>
<span data-ttu-id="b7417-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7417-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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