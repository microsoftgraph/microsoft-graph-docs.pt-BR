---
title: Criar grupo de roteamento de áudio
description: Criar um novo **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dc0e2a3463229762b3a641f33f77f2df8d506aa0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461217"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="874ab-103">Criar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="874ab-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="874ab-104">Criar um novo **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="874ab-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="874ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="874ab-105">Permissions</span></span>
<span data-ttu-id="874ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="874ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874ab-108">Permission type</span></span>                        | <span data-ttu-id="874ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="874ab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="874ab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="874ab-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874ab-111">Not supported.</span></span>                               |
| <span data-ttu-id="874ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874ab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874ab-113">Not supported.</span></span>                               |
| <span data-ttu-id="874ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874ab-114">Application</span></span>                            | <span data-ttu-id="874ab-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="874ab-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="874ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="874ab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874ab-117">Request headers</span></span>
| <span data-ttu-id="874ab-118">Nome</span><span class="sxs-lookup"><span data-stu-id="874ab-118">Name</span></span>          | <span data-ttu-id="874ab-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="874ab-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="874ab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="874ab-120">Authorization</span></span> | <span data-ttu-id="874ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="874ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874ab-123">Request body</span></span>
<span data-ttu-id="874ab-124">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="874ab-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="874ab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ab-125">Response</span></span>
<span data-ttu-id="874ab-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874ab-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="874ab-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="874ab-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="874ab-128">Exemplo 1: grupo de roteamento de áudio de um para um</span><span class="sxs-lookup"><span data-stu-id="874ab-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="874ab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874ab-129">Request</span></span>
<span data-ttu-id="874ab-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="874ab-130">The following example shows the request.</span></span>

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

<span data-ttu-id="874ab-131">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="874ab-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="874ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ab-132">Response</span></span>

> <span data-ttu-id="874ab-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="874ab-135">Exemplo 2: audioRoutingGroup de difusão seletiva</span><span class="sxs-lookup"><span data-stu-id="874ab-135">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="874ab-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874ab-136">Request</span></span>
<span data-ttu-id="874ab-137">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="874ab-137">The following example shows the request.</span></span>

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

<span data-ttu-id="874ab-138">No corpo da solicitação, forneça uma representação JSON do objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="874ab-138">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="874ab-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ab-139">Response</span></span>

> <span data-ttu-id="874ab-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
