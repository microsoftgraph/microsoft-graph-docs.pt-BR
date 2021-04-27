---
title: Criar grupo de roteamento de áudio
description: Crie um novo **audioRoutingGroup**.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f4c7cbc969b676db6786bf0d708e92381fd4cecf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047627"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="ef423-103">Criar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="ef423-103">Create audio routing group</span></span>

<span data-ttu-id="ef423-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef423-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef423-105">Crie um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="ef423-105">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef423-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef423-106">Permissions</span></span>
<span data-ttu-id="ef423-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef423-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef423-109">Permission type</span></span>                        | <span data-ttu-id="ef423-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef423-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef423-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef423-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef423-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef423-112">Not supported.</span></span>                               |
| <span data-ttu-id="ef423-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef423-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef423-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef423-114">Not supported.</span></span>                               |
| <span data-ttu-id="ef423-115">Application</span><span class="sxs-lookup"><span data-stu-id="ef423-115">Application</span></span>                            | <span data-ttu-id="ef423-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="ef423-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef423-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef423-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="ef423-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="ef423-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="ef423-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="ef423-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef423-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef423-120">Request headers</span></span>
| <span data-ttu-id="ef423-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ef423-121">Name</span></span>          | <span data-ttu-id="ef423-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef423-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ef423-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef423-123">Authorization</span></span> | <span data-ttu-id="ef423-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef423-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef423-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef423-126">Request body</span></span>
<span data-ttu-id="ef423-127">No corpo da solicitação, fornece uma representação JSON do [objeto audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef423-127">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef423-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef423-128">Response</span></span>
<span data-ttu-id="ef423-129">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef423-129">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef423-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ef423-130">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="ef423-131">Exemplo 1: grupo de roteamento de áudio um para um</span><span class="sxs-lookup"><span data-stu-id="ef423-131">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="ef423-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef423-132">Request</span></span>
<span data-ttu-id="ef423-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef423-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ef423-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef423-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef423-135">C#</span><span class="sxs-lookup"><span data-stu-id="ef423-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef423-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef423-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef423-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef423-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef423-138">Java</span><span class="sxs-lookup"><span data-stu-id="ef423-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-audioroutinggroup-from-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ef423-139">No corpo da solicitação, fornece uma representação JSON do [objeto audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef423-139">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ef423-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef423-140">Response</span></span>

> <span data-ttu-id="ef423-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef423-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="ef423-142">Exemplo 2: audioRoutingGroup multicast</span><span class="sxs-lookup"><span data-stu-id="ef423-142">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="ef423-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef423-143">Request</span></span>
<span data-ttu-id="ef423-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef423-144">The following example shows the request.</span></span>

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

<span data-ttu-id="ef423-145">No corpo da solicitação, fornece uma representação JSON do [objeto audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef423-145">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ef423-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef423-146">Response</span></span>

> <span data-ttu-id="ef423-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef423-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


