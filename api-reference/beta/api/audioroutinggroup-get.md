---
title: Obter grupo de roteamento de áudio
description: Recupere as propriedades e os relacionamentos de um objeto audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 43279f67b88e5e4c08c2c1cd83648786585b538d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258286"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="27997-103">Obter grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="27997-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27997-104">Recupere as propriedades e os relacionamentos de um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="27997-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27997-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27997-105">Permissions</span></span>
<span data-ttu-id="27997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27997-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27997-108">Permission type</span></span>                        | <span data-ttu-id="27997-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27997-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27997-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27997-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27997-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="27997-111">Not Supported</span></span>                               |
| <span data-ttu-id="27997-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27997-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27997-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="27997-113">Not Supported</span></span>                               |
| <span data-ttu-id="27997-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27997-114">Application</span></span>                            | <span data-ttu-id="27997-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="27997-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27997-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27997-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27997-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27997-117">Optional query parameters</span></span>
<span data-ttu-id="27997-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27997-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27997-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27997-119">Request headers</span></span>
| <span data-ttu-id="27997-120">Nome</span><span class="sxs-lookup"><span data-stu-id="27997-120">Name</span></span>          | <span data-ttu-id="27997-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="27997-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="27997-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27997-122">Authorization</span></span> | <span data-ttu-id="27997-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27997-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27997-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27997-125">Request body</span></span>
<span data-ttu-id="27997-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27997-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27997-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="27997-127">Response</span></span>
<span data-ttu-id="27997-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27997-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27997-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27997-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27997-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27997-130">Request</span></span>
<span data-ttu-id="27997-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="27997-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="27997-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="27997-132">Response</span></span>

> <span data-ttu-id="27997-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27997-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27997-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="27997-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27997-136">C#</span><span class="sxs-lookup"><span data-stu-id="27997-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27997-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="27997-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="27997-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27997-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
