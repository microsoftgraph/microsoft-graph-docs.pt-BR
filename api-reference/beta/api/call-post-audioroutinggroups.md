---
title: Criar grupo de roteamento de áudio
description: Criar um novo **audioRoutingGroup**.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9dc787e7dc5c4339319c46f66f94ba7845c443d9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959582"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="096c4-103">Criar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="096c4-103">Create audio routing group</span></span>

<span data-ttu-id="096c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="096c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="096c4-105">Criar um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="096c4-105">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="096c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="096c4-106">Permissions</span></span>
<span data-ttu-id="096c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="096c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="096c4-109">Permission type</span></span>                        | <span data-ttu-id="096c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="096c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="096c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="096c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="096c4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="096c4-112">Not supported.</span></span>                               |
| <span data-ttu-id="096c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="096c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="096c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="096c4-114">Not supported.</span></span>                               |
| <span data-ttu-id="096c4-115">Application</span><span class="sxs-lookup"><span data-stu-id="096c4-115">Application</span></span>                            | <span data-ttu-id="096c4-116">Calls. JoinGroupCalls. All, Calls.InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="096c4-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="096c4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="096c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="096c4-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="096c4-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="096c4-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="096c4-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="096c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="096c4-120">Request headers</span></span>
| <span data-ttu-id="096c4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="096c4-121">Name</span></span>          | <span data-ttu-id="096c4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="096c4-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="096c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="096c4-123">Authorization</span></span> | <span data-ttu-id="096c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="096c4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="096c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="096c4-126">Request body</span></span>
<span data-ttu-id="096c4-127">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="096c4-127">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="096c4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="096c4-128">Response</span></span>
<span data-ttu-id="096c4-129">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="096c4-129">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="096c4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="096c4-130">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="096c4-131">Exemplo 1: grupo de roteamento de áudio de um para um</span><span class="sxs-lookup"><span data-stu-id="096c4-131">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="096c4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="096c4-132">Request</span></span>
<span data-ttu-id="096c4-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="096c4-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="096c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="096c4-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="096c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="096c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096c4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096c4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096c4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096c4-138">Java</span><span class="sxs-lookup"><span data-stu-id="096c4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-audioroutinggroup-from-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="096c4-139">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="096c4-139">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="096c4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="096c4-140">Response</span></span>

> <span data-ttu-id="096c4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="096c4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="096c4-143">Exemplo 2: audioRoutingGroup de difusão seletiva</span><span class="sxs-lookup"><span data-stu-id="096c4-143">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="096c4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="096c4-144">Request</span></span>
<span data-ttu-id="096c4-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="096c4-145">The following example shows the request.</span></span>

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

<span data-ttu-id="096c4-146">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="096c4-146">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="096c4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="096c4-147">Response</span></span>

> <span data-ttu-id="096c4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="096c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


