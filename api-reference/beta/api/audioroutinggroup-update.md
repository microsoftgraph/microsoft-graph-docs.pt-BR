---
title: Atualizar grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 77fa0c78f295cd8d0380a386ad19f88388417989
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911871"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="bc9d9-103">Atualizar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="bc9d9-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc9d9-104">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="bc9d9-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc9d9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc9d9-105">Permissions</span></span>
<span data-ttu-id="bc9d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc9d9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc9d9-108">Permission type</span></span> | <span data-ttu-id="bc9d9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc9d9-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="bc9d9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc9d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc9d9-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bc9d9-111">Not Supported</span></span>                       |
| <span data-ttu-id="bc9d9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc9d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc9d9-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bc9d9-113">Not Supported</span></span>                       |
| <span data-ttu-id="bc9d9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc9d9-114">Application</span></span>     | <span data-ttu-id="bc9d9-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="bc9d9-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc9d9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc9d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="bc9d9-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="bc9d9-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc9d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9d9-119">Request headers</span></span>
| <span data-ttu-id="bc9d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bc9d9-120">Name</span></span>          | <span data-ttu-id="bc9d9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9d9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bc9d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc9d9-122">Authorization</span></span> | <span data-ttu-id="bc9d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc9d9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9d9-125">Request body</span></span>
<span data-ttu-id="bc9d9-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bc9d9-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc9d9-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc9d9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc9d9-129">Property</span></span>       | <span data-ttu-id="bc9d9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc9d9-130">Type</span></span>    |<span data-ttu-id="bc9d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9d9-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc9d9-132">receptores</span><span class="sxs-lookup"><span data-stu-id="bc9d9-132">receivers</span></span> | <span data-ttu-id="bc9d9-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc9d9-133">String collection</span></span> | <span data-ttu-id="bc9d9-134">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="bc9d9-135">routingmode</span><span class="sxs-lookup"><span data-stu-id="bc9d9-135">routingMode</span></span> | <span data-ttu-id="bc9d9-136">String</span><span class="sxs-lookup"><span data-stu-id="bc9d9-136">String</span></span> | <span data-ttu-id="bc9d9-137">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="bc9d9-138">fontes</span><span class="sxs-lookup"><span data-stu-id="bc9d9-138">sources</span></span> | <span data-ttu-id="bc9d9-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc9d9-139">String collection</span></span> | <span data-ttu-id="bc9d9-140">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="bc9d9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc9d9-141">Response</span></span>
<span data-ttu-id="bc9d9-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc9d9-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc9d9-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc9d9-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc9d9-144">Request</span></span>
<span data-ttu-id="bc9d9-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bc9d9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc9d9-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc9d9-147">C#</span><span class="sxs-lookup"><span data-stu-id="bc9d9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc9d9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc9d9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc9d9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc9d9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc9d9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc9d9-150">Response</span></span>

> <span data-ttu-id="bc9d9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc9d9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
