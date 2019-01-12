---
title: Criar um grupo de roteamento de áudio
description: Crie um novo **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe623a581233324e13c949d16570b1396fdd663c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966381"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="07d1a-103">Criar um grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="07d1a-103">Create audio routing group</span></span>

> <span data-ttu-id="07d1a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07d1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07d1a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07d1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07d1a-106">Crie um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="07d1a-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="07d1a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07d1a-107">Permissions</span></span>
<span data-ttu-id="07d1a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07d1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07d1a-110">Permission type</span></span>                        | <span data-ttu-id="07d1a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07d1a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="07d1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07d1a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="07d1a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07d1a-113">Not supported.</span></span>                               |
| <span data-ttu-id="07d1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07d1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07d1a-115">Not supported.</span></span>                               |
| <span data-ttu-id="07d1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07d1a-116">Application</span></span>                            | <span data-ttu-id="07d1a-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="07d1a-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07d1a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="07d1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07d1a-119">Request headers</span></span>
| <span data-ttu-id="07d1a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="07d1a-120">Name</span></span>          | <span data-ttu-id="07d1a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="07d1a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="07d1a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07d1a-122">Authorization</span></span> | <span data-ttu-id="07d1a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07d1a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07d1a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07d1a-125">Request body</span></span>
<span data-ttu-id="07d1a-126">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="07d1a-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="07d1a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d1a-127">Response</span></span>
<span data-ttu-id="07d1a-128">Se tiver êxito, este método retornará `200 OK` objeto response de código e [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07d1a-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07d1a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07d1a-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="07d1a-130">O exemplo 1: Grupo de roteamento de áudio individual</span><span class="sxs-lookup"><span data-stu-id="07d1a-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="07d1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07d1a-131">Request</span></span>
<span data-ttu-id="07d1a-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="07d1a-132">The following example shows the request.</span></span>

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

<span data-ttu-id="07d1a-133">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="07d1a-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="07d1a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d1a-134">Response</span></span>

> <span data-ttu-id="07d1a-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07d1a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="07d1a-137">Exemplo 2: AudioRoutingGroup Multicast</span><span class="sxs-lookup"><span data-stu-id="07d1a-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="07d1a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07d1a-138">Request</span></span>
<span data-ttu-id="07d1a-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="07d1a-139">The following example shows the request.</span></span>

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

<span data-ttu-id="07d1a-140">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="07d1a-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="07d1a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d1a-141">Response</span></span>

> <span data-ttu-id="07d1a-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07d1a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
