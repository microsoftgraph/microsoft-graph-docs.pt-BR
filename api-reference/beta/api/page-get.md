---
title: Obter página
description: Recupere as propriedades e os relacionamentos de um objeto Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 57a2c75bbe671086c89818a84f7f8266b90713c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539379"
---
# <a name="get-page"></a><span data-ttu-id="6fb18-103">Obter página</span><span class="sxs-lookup"><span data-stu-id="6fb18-103">Get page</span></span>

<span data-ttu-id="6fb18-104">Recupere as propriedades e os relacionamentos de um objeto [Page](../resources/page.md) .</span><span class="sxs-lookup"><span data-stu-id="6fb18-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="6fb18-105">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="6fb18-105">**Getting page information**</span></span>

<span data-ttu-id="6fb18-106">Acessar os metadados de uma página por identificador de página:</span><span class="sxs-lookup"><span data-stu-id="6fb18-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="6fb18-107">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="6fb18-107">**Getting page content**</span></span>

<span data-ttu-id="6fb18-108">Você pode usar o ponto de `content` extremidade da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="6fb18-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="6fb18-109">A `includeIDs=true` opção de consulta é usada para [Atualizar páginas](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="6fb18-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb18-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fb18-110">Permissions</span></span>
<span data-ttu-id="6fb18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb18-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fb18-113">Permission type</span></span>      | <span data-ttu-id="6fb18-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fb18-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb18-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fb18-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb18-116">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6fb18-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fb18-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fb18-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb18-118">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fb18-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6fb18-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fb18-119">Application</span></span> | <span data-ttu-id="6fb18-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb18-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb18-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb18-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb18-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fb18-122">Optional query parameters</span></span>
<span data-ttu-id="6fb18-123">Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb18-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6fb18-124">A resposta padrão expande `parentSection` e seleciona as propriedades `id`, `name`e e. `self`</span><span class="sxs-lookup"><span data-stu-id="6fb18-124">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="6fb18-125">Os `expand` valores válidos para páginas `parentNotebook` são `parentSection`e.</span><span class="sxs-lookup"><span data-stu-id="6fb18-125">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fb18-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb18-126">Request headers</span></span>
| <span data-ttu-id="6fb18-127">Nome</span><span class="sxs-lookup"><span data-stu-id="6fb18-127">Name</span></span>       | <span data-ttu-id="6fb18-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fb18-128">Type</span></span> | <span data-ttu-id="6fb18-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fb18-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6fb18-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fb18-130">Authorization</span></span>  | <span data-ttu-id="6fb18-131">string</span><span class="sxs-lookup"><span data-stu-id="6fb18-131">string</span></span>  | <span data-ttu-id="6fb18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fb18-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6fb18-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fb18-134">Accept</span></span> | <span data-ttu-id="6fb18-135">string</span><span class="sxs-lookup"><span data-stu-id="6fb18-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6fb18-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb18-136">Request body</span></span>
<span data-ttu-id="6fb18-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fb18-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb18-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb18-138">Response</span></span>

<span data-ttu-id="6fb18-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [Page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb18-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb18-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fb18-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fb18-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb18-141">Request</span></span>
<span data-ttu-id="6fb18-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fb18-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="6fb18-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb18-143">Response</span></span>
<span data-ttu-id="6fb18-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb18-144">Here is an example of the response.</span></span> <span data-ttu-id="6fb18-145">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="6fb18-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="6fb18-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fb18-146">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
