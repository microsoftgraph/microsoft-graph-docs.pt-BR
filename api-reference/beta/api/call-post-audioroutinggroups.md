---
title: Criar grupo de roteamento de áudio
description: Criar um novo **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7b34bc058c116a9be78f491f8dc2e826ea09f0c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005967"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="ba29b-103">Criar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="ba29b-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba29b-104">Criar um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="ba29b-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba29b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba29b-105">Permissions</span></span>
<span data-ttu-id="ba29b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba29b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba29b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba29b-108">Permission type</span></span>                        | <span data-ttu-id="ba29b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba29b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba29b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba29b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba29b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba29b-111">Not supported.</span></span>                               |
| <span data-ttu-id="ba29b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba29b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba29b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba29b-113">Not supported.</span></span>                               |
| <span data-ttu-id="ba29b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba29b-114">Application</span></span>                            | <span data-ttu-id="ba29b-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="ba29b-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba29b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba29b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="ba29b-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="ba29b-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="ba29b-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="ba29b-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba29b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba29b-119">Request headers</span></span>
| <span data-ttu-id="ba29b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ba29b-120">Name</span></span>          | <span data-ttu-id="ba29b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba29b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ba29b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba29b-122">Authorization</span></span> | <span data-ttu-id="ba29b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba29b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba29b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba29b-125">Request body</span></span>
<span data-ttu-id="ba29b-126">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ba29b-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ba29b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba29b-127">Response</span></span>
<span data-ttu-id="ba29b-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba29b-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba29b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba29b-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="ba29b-130">Exemplo 1: grupo de roteamento de áudio de um para um</span><span class="sxs-lookup"><span data-stu-id="ba29b-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="ba29b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba29b-131">Request</span></span>
<span data-ttu-id="ba29b-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba29b-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ba29b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba29b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba29b-134">C#</span><span class="sxs-lookup"><span data-stu-id="ba29b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba29b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba29b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba29b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba29b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ba29b-137">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ba29b-137">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ba29b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba29b-138">Response</span></span>

> <span data-ttu-id="ba29b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba29b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="ba29b-141">Exemplo 2: audioRoutingGroup de difusão seletiva</span><span class="sxs-lookup"><span data-stu-id="ba29b-141">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="ba29b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba29b-142">Request</span></span>
<span data-ttu-id="ba29b-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba29b-143">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
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

<span data-ttu-id="ba29b-144">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ba29b-144">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ba29b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba29b-145">Response</span></span>

> <span data-ttu-id="ba29b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba29b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
