---
title: Atualizar o grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
ms.openlocfilehash: a6b5d2ed3c11733f7a8e46ed4db61def05395c5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035627"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="08dab-103">Atualizar o grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="08dab-103">Update audio routing group</span></span>

> <span data-ttu-id="08dab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="08dab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08dab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="08dab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08dab-106">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="08dab-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08dab-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="08dab-107">Permissions</span></span>
<span data-ttu-id="08dab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08dab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08dab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08dab-110">Permission type</span></span> | <span data-ttu-id="08dab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08dab-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="08dab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08dab-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="08dab-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="08dab-113">Not Supported</span></span>                       |
| <span data-ttu-id="08dab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08dab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08dab-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="08dab-115">Not Supported</span></span>                       |
| <span data-ttu-id="08dab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08dab-116">Application</span></span>     | <span data-ttu-id="08dab-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="08dab-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08dab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08dab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="08dab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08dab-119">Request headers</span></span>
| <span data-ttu-id="08dab-120">Nome</span><span class="sxs-lookup"><span data-stu-id="08dab-120">Name</span></span>          | <span data-ttu-id="08dab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="08dab-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="08dab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08dab-122">Authorization</span></span> | <span data-ttu-id="08dab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08dab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08dab-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08dab-125">Request body</span></span>
<span data-ttu-id="08dab-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="08dab-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="08dab-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="08dab-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08dab-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="08dab-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08dab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08dab-129">Property</span></span>       | <span data-ttu-id="08dab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="08dab-130">Type</span></span>    |<span data-ttu-id="08dab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="08dab-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08dab-132">receptores</span><span class="sxs-lookup"><span data-stu-id="08dab-132">receivers</span></span> | <span data-ttu-id="08dab-133">String collection</span><span class="sxs-lookup"><span data-stu-id="08dab-133">String collection</span></span> | <span data-ttu-id="08dab-134">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="08dab-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="08dab-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="08dab-135">routingMode</span></span> | <span data-ttu-id="08dab-136">String</span><span class="sxs-lookup"><span data-stu-id="08dab-136">String</span></span> | <span data-ttu-id="08dab-137">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="08dab-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="08dab-138">sources</span><span class="sxs-lookup"><span data-stu-id="08dab-138">sources</span></span> | <span data-ttu-id="08dab-139">String collection</span><span class="sxs-lookup"><span data-stu-id="08dab-139">String collection</span></span> | <span data-ttu-id="08dab-140">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="08dab-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="08dab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dab-141">Response</span></span>
<span data-ttu-id="08dab-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08dab-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08dab-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08dab-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08dab-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08dab-144">Request</span></span>
<span data-ttu-id="08dab-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="08dab-145">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_audioRoutingGroup"
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
##### <a name="response"></a><span data-ttu-id="08dab-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dab-146">Response</span></span>

> <span data-ttu-id="08dab-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08dab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->