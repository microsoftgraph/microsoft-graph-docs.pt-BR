---
title: Get page
description: Recupere as propriedades e os relacionamentos de um objeto page.
localization_priority: Normal
ms.openlocfilehash: 7fac5d442ade9f41201881e6b5082ce9ec5fed0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807942"
---
# <a name="get-page"></a><span data-ttu-id="dda05-103">Get page</span><span class="sxs-lookup"><span data-stu-id="dda05-103">Get page</span></span>

<span data-ttu-id="dda05-104">Recupere as propriedades e os relacionamentos de um objeto [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="dda05-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="dda05-105">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="dda05-105">**Getting page information**</span></span>

<span data-ttu-id="dda05-106">Acesse os metadados de uma página pelo identificador da página:</span><span class="sxs-lookup"><span data-stu-id="dda05-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="dda05-107">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="dda05-107">**Getting page content**</span></span>

<span data-ttu-id="dda05-108">Você pode usar o ponto de extremidade `content` da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="dda05-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="dda05-109">A opção de consulta `includeIDs=true` é usada para [atualizar páginas](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="dda05-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dda05-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="dda05-110">Permissions</span></span>
<span data-ttu-id="dda05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dda05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dda05-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dda05-113">Permission type</span></span>      | <span data-ttu-id="dda05-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dda05-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dda05-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dda05-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dda05-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda05-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dda05-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dda05-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dda05-118">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dda05-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dda05-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dda05-119">Application</span></span> | <span data-ttu-id="dda05-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda05-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dda05-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dda05-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dda05-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dda05-122">Optional query parameters</span></span>
<span data-ttu-id="dda05-123">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dda05-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="dda05-p102">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="dda05-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dda05-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dda05-126">Request headers</span></span>
| <span data-ttu-id="dda05-127">Nome</span><span class="sxs-lookup"><span data-stu-id="dda05-127">Name</span></span>       | <span data-ttu-id="dda05-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="dda05-128">Type</span></span> | <span data-ttu-id="dda05-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dda05-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dda05-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="dda05-130">Authorization</span></span>  | <span data-ttu-id="dda05-131">string</span><span class="sxs-lookup"><span data-stu-id="dda05-131">string</span></span>  | <span data-ttu-id="dda05-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dda05-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dda05-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dda05-134">Accept</span></span> | <span data-ttu-id="dda05-135">string</span><span class="sxs-lookup"><span data-stu-id="dda05-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dda05-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dda05-136">Request body</span></span>
<span data-ttu-id="dda05-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dda05-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dda05-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dda05-138">Response</span></span>

<span data-ttu-id="dda05-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dda05-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dda05-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dda05-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dda05-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dda05-141">Request</span></span>
<span data-ttu-id="dda05-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dda05-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="dda05-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dda05-143">Response</span></span>
<span data-ttu-id="dda05-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dda05-144">Here is an example of the response.</span></span> <span data-ttu-id="dda05-145">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="dda05-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="dda05-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dda05-146">All of the properties will be returned from an actual call.</span></span>
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
