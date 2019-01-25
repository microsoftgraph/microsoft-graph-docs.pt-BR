---
title: Criar um grupo de roteamento de áudio
description: Crie um novo **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dc0e2a3463229762b3a641f33f77f2df8d506aa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522858"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="98fc5-103">Criar um grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="98fc5-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98fc5-104">Crie um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="98fc5-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="98fc5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="98fc5-105">Permissions</span></span>
<span data-ttu-id="98fc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98fc5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98fc5-108">Permission type</span></span>                        | <span data-ttu-id="98fc5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98fc5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98fc5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98fc5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98fc5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98fc5-111">Not supported.</span></span>                               |
| <span data-ttu-id="98fc5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98fc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98fc5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98fc5-113">Not supported.</span></span>                               |
| <span data-ttu-id="98fc5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98fc5-114">Application</span></span>                            | <span data-ttu-id="98fc5-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="98fc5-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98fc5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98fc5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="98fc5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98fc5-117">Request headers</span></span>
| <span data-ttu-id="98fc5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="98fc5-118">Name</span></span>          | <span data-ttu-id="98fc5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="98fc5-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="98fc5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="98fc5-120">Authorization</span></span> | <span data-ttu-id="98fc5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98fc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98fc5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98fc5-123">Request body</span></span>
<span data-ttu-id="98fc5-124">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="98fc5-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98fc5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fc5-125">Response</span></span>
<span data-ttu-id="98fc5-126">Se tiver êxito, este método retornará `200 OK` objeto response de código e [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98fc5-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98fc5-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="98fc5-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="98fc5-128">O exemplo 1: Grupo de roteamento de áudio individual</span><span class="sxs-lookup"><span data-stu-id="98fc5-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="98fc5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98fc5-129">Request</span></span>
<span data-ttu-id="98fc5-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="98fc5-130">The following example shows the request.</span></span>

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

<span data-ttu-id="98fc5-131">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="98fc5-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="98fc5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fc5-132">Response</span></span>

> <span data-ttu-id="98fc5-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98fc5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="98fc5-135">Exemplo 2: AudioRoutingGroup Multicast</span><span class="sxs-lookup"><span data-stu-id="98fc5-135">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="98fc5-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98fc5-136">Request</span></span>
<span data-ttu-id="98fc5-137">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="98fc5-137">The following example shows the request.</span></span>

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

<span data-ttu-id="98fc5-138">No corpo da solicitação, fornece uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="98fc5-138">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="98fc5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fc5-139">Response</span></span>

> <span data-ttu-id="98fc5-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98fc5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
