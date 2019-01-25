---
title: Atualizar o grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a6c8142ec36becd2a06a16d81bff7d1ceff75b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524671"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="c0792-103">Atualizar o grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="c0792-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0792-104">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="c0792-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0792-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0792-105">Permissions</span></span>
<span data-ttu-id="c0792-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0792-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0792-108">Permission type</span></span> | <span data-ttu-id="c0792-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0792-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="c0792-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0792-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0792-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="c0792-111">Not Supported</span></span>                       |
| <span data-ttu-id="c0792-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0792-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0792-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="c0792-113">Not Supported</span></span>                       |
| <span data-ttu-id="c0792-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0792-114">Application</span></span>     | <span data-ttu-id="c0792-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="c0792-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0792-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0792-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0792-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0792-117">Request headers</span></span>
| <span data-ttu-id="c0792-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c0792-118">Name</span></span>          | <span data-ttu-id="c0792-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0792-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c0792-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0792-120">Authorization</span></span> | <span data-ttu-id="c0792-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0792-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0792-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0792-123">Request body</span></span>
<span data-ttu-id="c0792-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c0792-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c0792-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c0792-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c0792-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0792-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0792-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0792-127">Property</span></span>       | <span data-ttu-id="c0792-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0792-128">Type</span></span>    |<span data-ttu-id="c0792-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0792-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0792-130">receptores</span><span class="sxs-lookup"><span data-stu-id="c0792-130">receivers</span></span> | <span data-ttu-id="c0792-131">String collection</span><span class="sxs-lookup"><span data-stu-id="c0792-131">String collection</span></span> | <span data-ttu-id="c0792-132">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="c0792-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="c0792-133">routingMode</span><span class="sxs-lookup"><span data-stu-id="c0792-133">routingMode</span></span> | <span data-ttu-id="c0792-134">String</span><span class="sxs-lookup"><span data-stu-id="c0792-134">String</span></span> | <span data-ttu-id="c0792-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="c0792-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="c0792-136">sources</span><span class="sxs-lookup"><span data-stu-id="c0792-136">sources</span></span> | <span data-ttu-id="c0792-137">String collection</span><span class="sxs-lookup"><span data-stu-id="c0792-137">String collection</span></span> | <span data-ttu-id="c0792-138">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="c0792-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="c0792-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0792-139">Response</span></span>
<span data-ttu-id="c0792-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0792-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0792-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0792-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0792-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0792-142">Request</span></span>
<span data-ttu-id="c0792-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0792-143">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
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
##### <a name="response"></a><span data-ttu-id="c0792-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0792-144">Response</span></span>

> <span data-ttu-id="c0792-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0792-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
