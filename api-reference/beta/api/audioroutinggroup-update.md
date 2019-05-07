---
title: Atualizar grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 835298804e2b409f75ef4d0e86786951f7ae0099
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636419"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="d14a7-103">Atualizar grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="d14a7-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d14a7-104">Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="d14a7-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d14a7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d14a7-105">Permissions</span></span>
<span data-ttu-id="d14a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d14a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d14a7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d14a7-108">Permission type</span></span> | <span data-ttu-id="d14a7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d14a7-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d14a7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d14a7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d14a7-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d14a7-111">Not Supported</span></span>                       |
| <span data-ttu-id="d14a7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d14a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d14a7-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d14a7-113">Not Supported</span></span>                       |
| <span data-ttu-id="d14a7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d14a7-114">Application</span></span>     | <span data-ttu-id="d14a7-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="d14a7-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d14a7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d14a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d14a7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d14a7-117">Request headers</span></span>
| <span data-ttu-id="d14a7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d14a7-118">Name</span></span>          | <span data-ttu-id="d14a7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d14a7-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d14a7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d14a7-120">Authorization</span></span> | <span data-ttu-id="d14a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d14a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d14a7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d14a7-123">Request body</span></span>
<span data-ttu-id="d14a7-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d14a7-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d14a7-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d14a7-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d14a7-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d14a7-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d14a7-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d14a7-127">Property</span></span>       | <span data-ttu-id="d14a7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d14a7-128">Type</span></span>    |<span data-ttu-id="d14a7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d14a7-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d14a7-130">receptores</span><span class="sxs-lookup"><span data-stu-id="d14a7-130">receivers</span></span> | <span data-ttu-id="d14a7-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d14a7-131">String collection</span></span> | <span data-ttu-id="d14a7-132">Os participantes de destino no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="d14a7-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="d14a7-133">routingmode</span><span class="sxs-lookup"><span data-stu-id="d14a7-133">routingMode</span></span> | <span data-ttu-id="d14a7-134">String</span><span class="sxs-lookup"><span data-stu-id="d14a7-134">String</span></span> | <span data-ttu-id="d14a7-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="d14a7-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="d14a7-136">fontes</span><span class="sxs-lookup"><span data-stu-id="d14a7-136">sources</span></span> | <span data-ttu-id="d14a7-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d14a7-137">String collection</span></span> | <span data-ttu-id="d14a7-138">O participante de origem no audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="d14a7-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="d14a7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d14a7-139">Response</span></span>
<span data-ttu-id="d14a7-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d14a7-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d14a7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d14a7-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d14a7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d14a7-142">Request</span></span>
<span data-ttu-id="d14a7-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d14a7-143">The following example shows the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="d14a7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d14a7-144">Response</span></span>

> <span data-ttu-id="d14a7-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d14a7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d14a7-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d14a7-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d14a7-148">Basic</span><span class="sxs-lookup"><span data-stu-id="d14a7-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d14a7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d14a7-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-audioRoutingGroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
