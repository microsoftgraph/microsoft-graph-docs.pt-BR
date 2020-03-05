---
title: Obter página
description: Recupere as propriedades e os relacionamentos de um objeto Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 13a4953c2ffa94ef85a836a3796f88a6cee149c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456005"
---
# <a name="get-page"></a><span data-ttu-id="ed455-103">Obter página</span><span class="sxs-lookup"><span data-stu-id="ed455-103">Get page</span></span>

<span data-ttu-id="ed455-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed455-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed455-105">Recupere as propriedades e os relacionamentos de um objeto [Page](../resources/onenotepage.md) .</span><span class="sxs-lookup"><span data-stu-id="ed455-105">Retrieve the properties and relationships of a [page](../resources/onenotepage.md) object.</span></span>

<span data-ttu-id="ed455-106">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="ed455-106">**Getting page information**</span></span>

<span data-ttu-id="ed455-107">Acessar os metadados de uma página por identificador de página:</span><span class="sxs-lookup"><span data-stu-id="ed455-107">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="ed455-108">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="ed455-108">**Getting page content**</span></span>

<span data-ttu-id="ed455-109">Você pode usar o ponto de `content` extremidade da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="ed455-109">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="ed455-110">A `includeIDs=true` opção de consulta é usada para [Atualizar páginas](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="ed455-110">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed455-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed455-111">Permissions</span></span>
<span data-ttu-id="ed455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed455-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed455-114">Permission type</span></span>      | <span data-ttu-id="ed455-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed455-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed455-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed455-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ed455-117">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ed455-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed455-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed455-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed455-119">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed455-119">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ed455-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed455-120">Application</span></span> | <span data-ttu-id="ed455-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed455-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed455-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed455-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed455-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed455-123">Optional query parameters</span></span>
<span data-ttu-id="ed455-124">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed455-124">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ed455-125">A resposta padrão expande `parentSection` e seleciona as propriedades `id`, `name`e e. `self`</span><span class="sxs-lookup"><span data-stu-id="ed455-125">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="ed455-126">Os `expand` valores válidos para páginas `parentNotebook` são `parentSection`e.</span><span class="sxs-lookup"><span data-stu-id="ed455-126">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed455-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed455-127">Request headers</span></span>
| <span data-ttu-id="ed455-128">Nome</span><span class="sxs-lookup"><span data-stu-id="ed455-128">Name</span></span>       | <span data-ttu-id="ed455-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed455-129">Type</span></span> | <span data-ttu-id="ed455-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed455-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed455-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed455-131">Authorization</span></span>  | <span data-ttu-id="ed455-132">string</span><span class="sxs-lookup"><span data-stu-id="ed455-132">string</span></span>  | <span data-ttu-id="ed455-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed455-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed455-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed455-135">Accept</span></span> | <span data-ttu-id="ed455-136">string</span><span class="sxs-lookup"><span data-stu-id="ed455-136">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ed455-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed455-137">Request body</span></span>
<span data-ttu-id="ed455-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed455-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed455-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed455-139">Response</span></span>

<span data-ttu-id="ed455-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [onenotePage](../resources/onenotepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed455-140">If successful, this method returns a `200 OK` response code and the [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed455-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed455-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed455-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed455-142">Request</span></span>
<span data-ttu-id="ed455-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed455-143">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="ed455-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed455-144">Response</span></span>
<span data-ttu-id="ed455-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed455-145">Here is an example of the response.</span></span> <span data-ttu-id="ed455-146">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="ed455-146">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="ed455-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed455-147">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
