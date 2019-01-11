---
title: Get page
description: Recupere as propriedades e os relacionamentos de um objeto page.
localization_priority: Normal
ms.openlocfilehash: 117f4d15d676f0be26e75a610d87b2de2581b17a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890822"
---
# <a name="get-page"></a><span data-ttu-id="1460a-103">Get page</span><span class="sxs-lookup"><span data-stu-id="1460a-103">Get page</span></span>

> <span data-ttu-id="1460a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1460a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1460a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1460a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1460a-106">Recupere as propriedades e os relacionamentos de um objeto [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="1460a-106">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="1460a-107">**Obtendo informações da página**</span><span class="sxs-lookup"><span data-stu-id="1460a-107">**Getting page information**</span></span>

<span data-ttu-id="1460a-108">Acesse os metadados de uma página pelo identificador da página:</span><span class="sxs-lookup"><span data-stu-id="1460a-108">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="1460a-109">**Obtendo o conteúdo da página**</span><span class="sxs-lookup"><span data-stu-id="1460a-109">**Getting page content**</span></span>

<span data-ttu-id="1460a-110">Você pode usar o ponto de extremidade `content` da página para obter o conteúdo HTML de uma página:</span><span class="sxs-lookup"><span data-stu-id="1460a-110">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="1460a-111">A opção de consulta `includeIDs=true` é usada para [atualizar páginas](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="1460a-111">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1460a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1460a-112">Permissions</span></span>
<span data-ttu-id="1460a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1460a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1460a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1460a-115">Permission type</span></span>      | <span data-ttu-id="1460a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1460a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1460a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1460a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1460a-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1460a-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1460a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1460a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1460a-120">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1460a-120">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1460a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1460a-121">Application</span></span> | <span data-ttu-id="1460a-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1460a-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1460a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1460a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1460a-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1460a-124">Optional query parameters</span></span>
<span data-ttu-id="1460a-125">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1460a-125">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1460a-p103">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="1460a-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1460a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1460a-128">Request headers</span></span>
| <span data-ttu-id="1460a-129">Nome</span><span class="sxs-lookup"><span data-stu-id="1460a-129">Name</span></span>       | <span data-ttu-id="1460a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1460a-130">Type</span></span> | <span data-ttu-id="1460a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1460a-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1460a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="1460a-132">Authorization</span></span>  | <span data-ttu-id="1460a-133">string</span><span class="sxs-lookup"><span data-stu-id="1460a-133">string</span></span>  | <span data-ttu-id="1460a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1460a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1460a-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1460a-136">Accept</span></span> | <span data-ttu-id="1460a-137">string</span><span class="sxs-lookup"><span data-stu-id="1460a-137">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1460a-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1460a-138">Request body</span></span>
<span data-ttu-id="1460a-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1460a-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1460a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1460a-140">Response</span></span>

<span data-ttu-id="1460a-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1460a-141">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1460a-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1460a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1460a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1460a-143">Request</span></span>
<span data-ttu-id="1460a-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1460a-144">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="1460a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1460a-145">Response</span></span>
<span data-ttu-id="1460a-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1460a-146">Here is an example of the response.</span></span> <span data-ttu-id="1460a-147">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="1460a-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="1460a-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1460a-148">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
