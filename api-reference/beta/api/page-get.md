---
title: Obter página
description: Recupere as propriedades e os relacionamentos de um objeto Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 23fae34065f99afa22e0af9aa2c52d717f7dcce1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004603"
---
# <a name="get-page"></a><span data-ttu-id="a852e-103">Obter página</span><span class="sxs-lookup"><span data-stu-id="a852e-103">Get page</span></span>

<span data-ttu-id="a852e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a852e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a852e-105">Recupere as propriedades e os relacionamentos de um objeto [Page](../resources/onenotepage.md) .</span><span class="sxs-lookup"><span data-stu-id="a852e-105">Retrieve the properties and relationships of a [page](../resources/onenotepage.md) object.</span></span>

<span data-ttu-id="a852e-106">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="a852e-106">**Getting page information**</span></span>

<span data-ttu-id="a852e-107">Acessar os metadados de uma página por identificador de página:</span><span class="sxs-lookup"><span data-stu-id="a852e-107">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="a852e-108">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="a852e-108">**Getting page content**</span></span>

<span data-ttu-id="a852e-109">Você pode usar o ponto de `content` extremidade da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="a852e-109">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="a852e-110">A `includeIDs=true` opção de consulta é usada para [Atualizar páginas](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="a852e-110">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a852e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a852e-111">Permissions</span></span>
<span data-ttu-id="a852e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a852e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a852e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a852e-114">Permission type</span></span>      | <span data-ttu-id="a852e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a852e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a852e-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a852e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a852e-117">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a852e-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a852e-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a852e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a852e-119">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a852e-119">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a852e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a852e-120">Application</span></span> | <span data-ttu-id="a852e-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a852e-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a852e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a852e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a852e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a852e-123">Optional query parameters</span></span>
<span data-ttu-id="a852e-124">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a852e-124">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a852e-125">A resposta padrão expande `parentSection` e seleciona as `id` `name` Propriedades, e e `self` .</span><span class="sxs-lookup"><span data-stu-id="a852e-125">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="a852e-126">`expand`Os valores válidos para páginas são `parentNotebook` e `parentSection` .</span><span class="sxs-lookup"><span data-stu-id="a852e-126">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a852e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a852e-127">Request headers</span></span>
| <span data-ttu-id="a852e-128">Nome</span><span class="sxs-lookup"><span data-stu-id="a852e-128">Name</span></span>       | <span data-ttu-id="a852e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a852e-129">Type</span></span> | <span data-ttu-id="a852e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a852e-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a852e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="a852e-131">Authorization</span></span>  | <span data-ttu-id="a852e-132">string</span><span class="sxs-lookup"><span data-stu-id="a852e-132">string</span></span>  | <span data-ttu-id="a852e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a852e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a852e-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a852e-135">Accept</span></span> | <span data-ttu-id="a852e-136">string</span><span class="sxs-lookup"><span data-stu-id="a852e-136">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a852e-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a852e-137">Request body</span></span>
<span data-ttu-id="a852e-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a852e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a852e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a852e-139">Response</span></span>

<span data-ttu-id="a852e-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [onenotePage](../resources/onenotepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a852e-140">If successful, this method returns a `200 OK` response code and the [onenotePage](../resources/onenotepage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a852e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a852e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a852e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a852e-142">Request</span></span>
<span data-ttu-id="a852e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a852e-143">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="a852e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a852e-144">Response</span></span>
<span data-ttu-id="a852e-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a852e-145">Here is an example of the response.</span></span> <span data-ttu-id="a852e-146">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="a852e-146">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="a852e-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a852e-147">All of the properties will be returned from an actual call.</span></span>
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


