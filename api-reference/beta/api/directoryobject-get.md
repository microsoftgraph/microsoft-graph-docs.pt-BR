---
title: Obter directoryObject
description: Recupere as propriedades e os relacionamentos do objeto directoryobject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ccd869b203b91a0b60872f3915c46eeae3cd3543
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260778"
---
# <a name="get-directoryobject"></a><span data-ttu-id="a981e-103">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="a981e-103">Get directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a981e-104">Recupere as propriedades e os relacionamentos do objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="a981e-104">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a981e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a981e-105">Permissions</span></span>
<span data-ttu-id="a981e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a981e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a981e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a981e-108">Permission type</span></span>      | <span data-ttu-id="a981e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a981e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a981e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a981e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a981e-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a981e-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a981e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a981e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a981e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a981e-113">Not supported.</span></span>    |
|<span data-ttu-id="a981e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a981e-114">Application</span></span> | <span data-ttu-id="a981e-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a981e-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a981e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a981e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a981e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a981e-117">Optional query parameters</span></span>
<span data-ttu-id="a981e-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a981e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a981e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a981e-119">Request headers</span></span>
| <span data-ttu-id="a981e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a981e-120">Name</span></span>       | <span data-ttu-id="a981e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a981e-121">Type</span></span> | <span data-ttu-id="a981e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a981e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a981e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a981e-123">Authorization</span></span>  | <span data-ttu-id="a981e-124">string</span><span class="sxs-lookup"><span data-stu-id="a981e-124">string</span></span>  | <span data-ttu-id="a981e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a981e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a981e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a981e-127">Request body</span></span>
<span data-ttu-id="a981e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a981e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a981e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a981e-129">Response</span></span>

<span data-ttu-id="a981e-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a981e-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a981e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a981e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a981e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a981e-132">Request</span></span>
<span data-ttu-id="a981e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a981e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="a981e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a981e-134">Response</span></span>
<span data-ttu-id="a981e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a981e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a981e-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a981e-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a981e-139">C#</span><span class="sxs-lookup"><span data-stu-id="a981e-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a981e-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a981e-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryobject-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a981e-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a981e-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryobject-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
