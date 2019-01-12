---
title: Listar páginas
description: Recupere uma lista de objetos page da seção especificada.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a0dc01443d7d884fee1809310c0341bd2abc9ebd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942448"
---
# <a name="list-pages"></a><span data-ttu-id="6a760-103">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="6a760-103">List pages</span></span>

> <span data-ttu-id="6a760-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a760-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a760-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a760-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a760-106">Recupere uma lista de objetos [page](../resources/page.md) da seção especificada.</span><span class="sxs-lookup"><span data-stu-id="6a760-106">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a760-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a760-107">Permissions</span></span>
<span data-ttu-id="6a760-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a760-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a760-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a760-110">Permission type</span></span>      | <span data-ttu-id="6a760-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a760-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a760-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a760-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a760-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a760-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a760-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a760-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a760-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a760-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6a760-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a760-116">Application</span></span> | <span data-ttu-id="6a760-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a760-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a760-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a760-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a760-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a760-119">Optional query parameters</span></span>
<span data-ttu-id="6a760-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a760-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6a760-p103">A consulta padrão das páginas retorna as 20 páginas principais ordenadas por `lastModifiedTime desc`. Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um `@odata.nextLink` que você pode usar para passar pelo conjunto de resultados. o número máximo de páginas retornadas em uma solicitação `top` é 100.</span><span class="sxs-lookup"><span data-stu-id="6a760-p103">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="6a760-p104">A resposta padrão expande `parentSection` e escolhe as propriedades `id`, `name` e `self` da seção. Os valores `expand` válidos das páginas são `parentNotebook` e `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="6a760-p104">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a760-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a760-126">Request headers</span></span>
| <span data-ttu-id="6a760-127">Nome</span><span class="sxs-lookup"><span data-stu-id="6a760-127">Name</span></span>       | <span data-ttu-id="6a760-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a760-128">Type</span></span> | <span data-ttu-id="6a760-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a760-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a760-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a760-130">Authorization</span></span>  | <span data-ttu-id="6a760-131">string</span><span class="sxs-lookup"><span data-stu-id="6a760-131">string</span></span>  | <span data-ttu-id="6a760-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a760-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a760-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a760-134">Accept</span></span> | <span data-ttu-id="6a760-135">string</span><span class="sxs-lookup"><span data-stu-id="6a760-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6a760-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a760-136">Request body</span></span>
<span data-ttu-id="6a760-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a760-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a760-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a760-138">Response</span></span>

<span data-ttu-id="6a760-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [page](../resources/page.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a760-139">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a760-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a760-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a760-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a760-141">Request</span></span>
<span data-ttu-id="6a760-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a760-142">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="6a760-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a760-143">Response</span></span>
<span data-ttu-id="6a760-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a760-144">Here is an example of the response.</span></span> <span data-ttu-id="6a760-145">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="6a760-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="6a760-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a760-146">All of the properties will be returned from an actual call.</span></span>
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
