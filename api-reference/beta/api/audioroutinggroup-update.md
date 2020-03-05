---
title: Atualizar grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 28cbf6662b09be81c6ffbafecbe1f888e596e3a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441309"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="bf563-103">Atualizar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="bf563-103">Update audio routing group</span></span>

<span data-ttu-id="bf563-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bf563-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf563-105">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="bf563-105">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf563-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf563-106">Permissions</span></span>
<span data-ttu-id="bf563-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf563-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf563-109">Permission type</span></span> | <span data-ttu-id="bf563-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf563-110">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="bf563-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf563-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf563-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bf563-112">Not Supported</span></span>                       |
| <span data-ttu-id="bf563-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf563-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf563-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bf563-114">Not Supported</span></span>                       |
| <span data-ttu-id="bf563-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf563-115">Application</span></span>     | <span data-ttu-id="bf563-116">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="bf563-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf563-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf563-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="bf563-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="bf563-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="bf563-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="bf563-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf563-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf563-120">Request headers</span></span>
| <span data-ttu-id="bf563-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bf563-121">Name</span></span>          | <span data-ttu-id="bf563-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf563-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bf563-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf563-123">Authorization</span></span> | <span data-ttu-id="bf563-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf563-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf563-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf563-126">Request body</span></span>
<span data-ttu-id="bf563-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bf563-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bf563-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bf563-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bf563-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bf563-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bf563-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf563-130">Property</span></span>       | <span data-ttu-id="bf563-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf563-131">Type</span></span>    |<span data-ttu-id="bf563-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf563-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf563-133">receptores</span><span class="sxs-lookup"><span data-stu-id="bf563-133">receivers</span></span> | <span data-ttu-id="bf563-134">String collection</span><span class="sxs-lookup"><span data-stu-id="bf563-134">String collection</span></span> | <span data-ttu-id="bf563-135">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="bf563-135">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="bf563-136">routingmode</span><span class="sxs-lookup"><span data-stu-id="bf563-136">routingMode</span></span> | <span data-ttu-id="bf563-137">String</span><span class="sxs-lookup"><span data-stu-id="bf563-137">String</span></span> | <span data-ttu-id="bf563-138">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="bf563-138">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="bf563-139">fontes</span><span class="sxs-lookup"><span data-stu-id="bf563-139">sources</span></span> | <span data-ttu-id="bf563-140">String collection</span><span class="sxs-lookup"><span data-stu-id="bf563-140">String collection</span></span> | <span data-ttu-id="bf563-141">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="bf563-141">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="bf563-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf563-142">Response</span></span>
<span data-ttu-id="bf563-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf563-143">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf563-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf563-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bf563-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf563-145">Request</span></span>
<span data-ttu-id="bf563-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf563-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bf563-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf563-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json

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
# <a name="c"></a>[<span data-ttu-id="bf563-148">C#</span><span class="sxs-lookup"><span data-stu-id="bf563-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf563-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf563-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf563-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf563-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf563-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf563-151">Response</span></span>

> <span data-ttu-id="bf563-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf563-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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
  ]
}
-->
