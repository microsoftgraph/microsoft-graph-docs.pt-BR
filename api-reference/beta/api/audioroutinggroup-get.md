---
title: Obter grupo de roteamento de áudio
description: Recupere as propriedades e os relacionamentos de um objeto audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e998e39118a66cda6ce9473f400736dcde986d50
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408087"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="131e5-103">Obter grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="131e5-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131e5-104">Recupere as propriedades e os relacionamentos de um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="131e5-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="131e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="131e5-105">Permissions</span></span>
<span data-ttu-id="131e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="131e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="131e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="131e5-108">Permission type</span></span>                        | <span data-ttu-id="131e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="131e5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="131e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="131e5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="131e5-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="131e5-111">Not Supported</span></span>                               |
| <span data-ttu-id="131e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="131e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="131e5-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="131e5-113">Not Supported</span></span>                               |
| <span data-ttu-id="131e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="131e5-114">Application</span></span>                            | <span data-ttu-id="131e5-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="131e5-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="131e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="131e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="131e5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="131e5-117">Optional query parameters</span></span>
<span data-ttu-id="131e5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="131e5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="131e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="131e5-119">Request headers</span></span>
| <span data-ttu-id="131e5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="131e5-120">Name</span></span>          | <span data-ttu-id="131e5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="131e5-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="131e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="131e5-122">Authorization</span></span> | <span data-ttu-id="131e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="131e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="131e5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="131e5-125">Request body</span></span>
<span data-ttu-id="131e5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="131e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="131e5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="131e5-127">Response</span></span>
<span data-ttu-id="131e5-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="131e5-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="131e5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="131e5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="131e5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="131e5-130">Request</span></span>
<span data-ttu-id="131e5-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="131e5-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="131e5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="131e5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="131e5-133">C#</span><span class="sxs-lookup"><span data-stu-id="131e5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="131e5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="131e5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="131e5-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="131e5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="131e5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="131e5-136">Response</span></span>

> <span data-ttu-id="131e5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="131e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
