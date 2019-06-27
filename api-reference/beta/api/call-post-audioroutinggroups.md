---
title: Criar grupo de roteamento de áudio
description: Criar um novo **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05b7e7230857da139e7331940f014b20001f3b9b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262255"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="375e2-103">Criar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="375e2-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="375e2-104">Criar um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="375e2-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="375e2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="375e2-105">Permissions</span></span>
<span data-ttu-id="375e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="375e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="375e2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="375e2-108">Permission type</span></span>                        | <span data-ttu-id="375e2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="375e2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="375e2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="375e2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="375e2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375e2-111">Not supported.</span></span>                               |
| <span data-ttu-id="375e2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="375e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375e2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375e2-113">Not supported.</span></span>                               |
| <span data-ttu-id="375e2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="375e2-114">Application</span></span>                            | <span data-ttu-id="375e2-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="375e2-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="375e2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="375e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="375e2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="375e2-117">Request headers</span></span>
| <span data-ttu-id="375e2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="375e2-118">Name</span></span>          | <span data-ttu-id="375e2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="375e2-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="375e2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="375e2-120">Authorization</span></span> | <span data-ttu-id="375e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="375e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="375e2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="375e2-123">Request body</span></span>
<span data-ttu-id="375e2-124">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="375e2-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="375e2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="375e2-125">Response</span></span>
<span data-ttu-id="375e2-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="375e2-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="375e2-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="375e2-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="375e2-128">Exemplo 1: grupo de roteamento de áudio de um para um</span><span class="sxs-lookup"><span data-stu-id="375e2-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="375e2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="375e2-129">Request</span></span>
<span data-ttu-id="375e2-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="375e2-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```

<span data-ttu-id="375e2-131">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="375e2-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="375e2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="375e2-132">Response</span></span>

> <span data-ttu-id="375e2-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="375e2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="375e2-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="375e2-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="375e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="375e2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="375e2-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="375e2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="375e2-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="375e2-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="375e2-139">Exemplo 2: audioRoutingGroup de difusão seletiva</span><span class="sxs-lookup"><span data-stu-id="375e2-139">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="375e2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="375e2-140">Request</span></span>
<span data-ttu-id="375e2-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="375e2-141">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create-audioRoutingGroup-from-call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<span data-ttu-id="375e2-142">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="375e2-142">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="375e2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="375e2-143">Response</span></span>

> <span data-ttu-id="375e2-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="375e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
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
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
