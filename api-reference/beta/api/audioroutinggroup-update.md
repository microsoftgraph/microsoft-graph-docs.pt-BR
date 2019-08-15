---
title: Atualizar grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ad5b82a930ebc183e860816d58a8fff17c8e5f5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415698"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="8bb18-103">Atualizar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="8bb18-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb18-104">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="8bb18-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb18-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bb18-105">Permissions</span></span>
<span data-ttu-id="8bb18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bb18-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bb18-108">Permission type</span></span> | <span data-ttu-id="8bb18-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bb18-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8bb18-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bb18-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bb18-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8bb18-111">Not Supported</span></span>                       |
| <span data-ttu-id="8bb18-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bb18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb18-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8bb18-113">Not Supported</span></span>                       |
| <span data-ttu-id="8bb18-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bb18-114">Application</span></span>     | <span data-ttu-id="8bb18-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="8bb18-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb18-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb18-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bb18-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb18-117">Request headers</span></span>
| <span data-ttu-id="8bb18-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8bb18-118">Name</span></span>          | <span data-ttu-id="8bb18-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bb18-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8bb18-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bb18-120">Authorization</span></span> | <span data-ttu-id="8bb18-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bb18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb18-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb18-123">Request body</span></span>
<span data-ttu-id="8bb18-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8bb18-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8bb18-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8bb18-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8bb18-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8bb18-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8bb18-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bb18-127">Property</span></span>       | <span data-ttu-id="8bb18-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bb18-128">Type</span></span>    |<span data-ttu-id="8bb18-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bb18-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8bb18-130">receptores</span><span class="sxs-lookup"><span data-stu-id="8bb18-130">receivers</span></span> | <span data-ttu-id="8bb18-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bb18-131">String collection</span></span> | <span data-ttu-id="8bb18-132">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="8bb18-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="8bb18-133">routingmode</span><span class="sxs-lookup"><span data-stu-id="8bb18-133">routingMode</span></span> | <span data-ttu-id="8bb18-134">String</span><span class="sxs-lookup"><span data-stu-id="8bb18-134">String</span></span> | <span data-ttu-id="8bb18-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="8bb18-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="8bb18-136">fontes</span><span class="sxs-lookup"><span data-stu-id="8bb18-136">sources</span></span> | <span data-ttu-id="8bb18-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bb18-137">String collection</span></span> | <span data-ttu-id="8bb18-138">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="8bb18-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="8bb18-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb18-139">Response</span></span>
<span data-ttu-id="8bb18-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bb18-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb18-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bb18-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8bb18-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb18-142">Request</span></span>
<span data-ttu-id="8bb18-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bb18-143">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8bb18-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb18-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bb18-145">C#</span><span class="sxs-lookup"><span data-stu-id="8bb18-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bb18-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb18-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bb18-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8bb18-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bb18-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb18-148">Response</span></span>

> <span data-ttu-id="8bb18-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bb18-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
