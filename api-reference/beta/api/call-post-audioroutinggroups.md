---
title: Criar um grupo de roteamento de áudio
description: Crie um novo **audioRoutingGroup**.
ms.openlocfilehash: 0dd506f3cf02e59d5a34c7184f4e596f6ff9e1fd
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156037"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="6db95-103">Criar um grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="6db95-103">Create audio routing group</span></span>

> <span data-ttu-id="6db95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6db95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6db95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6db95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6db95-106">Crie um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="6db95-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6db95-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6db95-107">Permissions</span></span>
<span data-ttu-id="6db95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6db95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db95-110">Permission type</span></span>                        | <span data-ttu-id="6db95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db95-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6db95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db95-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6db95-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db95-113">Not supported.</span></span>                               |
| <span data-ttu-id="6db95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db95-115">Not supported.</span></span>                               |
| <span data-ttu-id="6db95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db95-116">Application</span></span>     | <span data-ttu-id="6db95-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="6db95-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6db95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="6db95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db95-119">Request headers</span></span>
| <span data-ttu-id="6db95-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6db95-120">Name</span></span>          | <span data-ttu-id="6db95-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db95-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6db95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db95-122">Authorization</span></span> | <span data-ttu-id="6db95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db95-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6db95-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db95-125">Request body</span></span>
<span data-ttu-id="6db95-126">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6db95-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6db95-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db95-127">Response</span></span>
<span data-ttu-id="6db95-128">Se tiver êxito, este método retornará `200 OK` objeto response de código e [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db95-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6db95-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6db95-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="6db95-130">O exemplo 1: Grupo de roteamento de áudio individual</span><span class="sxs-lookup"><span data-stu-id="6db95-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="6db95-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db95-131">Request</span></span>
<span data-ttu-id="6db95-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db95-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_audioRoutingGroup_from_call"
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

<span data-ttu-id="6db95-133">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6db95-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6db95-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db95-134">Response</span></span>

> <span data-ttu-id="6db95-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6db95-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="6db95-137">Exemplo 2: AudioRoutingGroup Multicast</span><span class="sxs-lookup"><span data-stu-id="6db95-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="6db95-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db95-138">Request</span></span>
<span data-ttu-id="6db95-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db95-139">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create_audioRoutingGroup_from_call",
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

<span data-ttu-id="6db95-140">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6db95-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6db95-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db95-141">Response</span></span>

> <span data-ttu-id="6db95-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6db95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
