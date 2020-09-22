---
title: Listar páginas
description: Recupere uma lista de objetos Page.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 993adcbefb97d15d1d43cd5184cbddb1284f5078
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038379"
---
# <a name="list-pages"></a><span data-ttu-id="fe233-103">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="fe233-103">List pages</span></span>

<span data-ttu-id="fe233-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe233-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe233-105">Recupere uma lista de objetos [Page](../resources/page.md) .</span><span class="sxs-lookup"><span data-stu-id="fe233-105">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe233-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe233-106">Permissions</span></span>
<span data-ttu-id="fe233-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe233-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe233-109">Permission type</span></span>      | <span data-ttu-id="fe233-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe233-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe233-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe233-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe233-112">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fe233-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe233-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe233-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe233-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe233-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="fe233-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe233-115">Application</span></span> | <span data-ttu-id="fe233-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe233-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe233-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe233-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe233-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe233-118">Optional query parameters</span></span>
<span data-ttu-id="fe233-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe233-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fe233-120">A consulta padrão para páginas retorna as 20 principais páginas ordenadas por `lastModifiedTime desc` .</span><span class="sxs-lookup"><span data-stu-id="fe233-120">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="fe233-121">Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para percorrer o conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="fe233-121">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="fe233-122">O número máximo de páginas retornadas para uma `top` solicitação é 100.</span><span class="sxs-lookup"><span data-stu-id="fe233-122">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="fe233-123">A resposta padrão expande `parentSection` e seleciona as `id` `displayName` Propriedades, e e `self` .</span><span class="sxs-lookup"><span data-stu-id="fe233-123">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="fe233-124">`expand`Os valores válidos para páginas são `parentNotebook` e `parentSection` .</span><span class="sxs-lookup"><span data-stu-id="fe233-124">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe233-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe233-125">Request headers</span></span>
| <span data-ttu-id="fe233-126">Nome</span><span class="sxs-lookup"><span data-stu-id="fe233-126">Name</span></span>       | <span data-ttu-id="fe233-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe233-127">Type</span></span> | <span data-ttu-id="fe233-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe233-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe233-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe233-129">Authorization</span></span>  | <span data-ttu-id="fe233-130">string</span><span class="sxs-lookup"><span data-stu-id="fe233-130">string</span></span>  | <span data-ttu-id="fe233-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe233-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe233-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe233-133">Accept</span></span> | <span data-ttu-id="fe233-134">string</span><span class="sxs-lookup"><span data-stu-id="fe233-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fe233-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe233-135">Request body</span></span>
<span data-ttu-id="fe233-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe233-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe233-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe233-137">Response</span></span>

<span data-ttu-id="fe233-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe233-138">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe233-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe233-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe233-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe233-140">Request</span></span>
<span data-ttu-id="fe233-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe233-141">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="fe233-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe233-142">Response</span></span>
<span data-ttu-id="fe233-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe233-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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

