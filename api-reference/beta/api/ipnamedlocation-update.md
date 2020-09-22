---
title: Atualizar ipnamedlocation
description: Atualiza as propriedades de um objeto ipNamedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1e9ff22fb86400214f283cb4e09fb0097f7843b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980061"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="4fff1-103">Atualizar ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="4fff1-103">Update ipNamedlocation</span></span>

<span data-ttu-id="4fff1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fff1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fff1-105">Atualiza as propriedades de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="4fff1-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fff1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fff1-106">Permissions</span></span>

<span data-ttu-id="4fff1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fff1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fff1-109">Permission type</span></span>                        | <span data-ttu-id="4fff1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fff1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fff1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fff1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fff1-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="4fff1-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="4fff1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fff1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fff1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fff1-114">Not supported.</span></span> |
| <span data-ttu-id="4fff1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fff1-115">Application</span></span>                            | <span data-ttu-id="4fff1-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="4fff1-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fff1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fff1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fff1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fff1-118">Request headers</span></span>

| <span data-ttu-id="4fff1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4fff1-119">Name</span></span>       | <span data-ttu-id="4fff1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fff1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4fff1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fff1-121">Authorization</span></span> | <span data-ttu-id="4fff1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fff1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fff1-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="4fff1-124">Content-type</span></span> | <span data-ttu-id="4fff1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fff1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fff1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fff1-127">Request body</span></span>

<span data-ttu-id="4fff1-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4fff1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4fff1-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4fff1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4fff1-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4fff1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4fff1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fff1-131">Property</span></span>     | <span data-ttu-id="4fff1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fff1-132">Type</span></span>        | <span data-ttu-id="4fff1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fff1-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4fff1-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4fff1-134">displayName</span></span>|<span data-ttu-id="4fff1-135">String</span><span class="sxs-lookup"><span data-stu-id="4fff1-135">String</span></span>|<span data-ttu-id="4fff1-136">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="4fff1-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="4fff1-137">Intervalos</span><span class="sxs-lookup"><span data-stu-id="4fff1-137">ipRanges</span></span>|<span data-ttu-id="4fff1-138">Coleção [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4fff1-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="4fff1-139">Lista de intervalos de endereços IP no formato CIDR do IPv4 (1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="4fff1-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="4fff1-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="4fff1-140">isTrusted</span></span>|<span data-ttu-id="4fff1-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fff1-141">Boolean</span></span>|<span data-ttu-id="4fff1-142">O valor é `true` se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="4fff1-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="4fff1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fff1-143">Response</span></span>

<span data-ttu-id="4fff1-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fff1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fff1-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4fff1-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fff1-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fff1-147">Request</span></span>

<span data-ttu-id="4fff1-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fff1-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fff1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fff1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted named location with only IPv4 address",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "6.5.4.3/18"
        }

    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="4fff1-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fff1-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4fff1-151">C#</span><span class="sxs-lookup"><span data-stu-id="4fff1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fff1-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fff1-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fff1-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fff1-153">Response</span></span>

<span data-ttu-id="4fff1-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4fff1-154">The following is an example of the response.</span></span>

> <span data-ttu-id="4fff1-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fff1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ipnamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


