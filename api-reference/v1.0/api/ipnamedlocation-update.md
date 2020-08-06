---
title: Atualizar ipnamedlocation
description: Atualiza as propriedades de um objeto ipNamedLocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1bb1ae728498c79cfe06efabe27b3986f8cdee4c
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567338"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="73966-103">Atualizar ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="73966-103">Update ipNamedlocation</span></span>

<span data-ttu-id="73966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73966-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73966-105">Atualiza as propriedades de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="73966-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73966-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="73966-106">Permissions</span></span>

<span data-ttu-id="73966-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73966-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73966-109">Permission type</span></span>                        | <span data-ttu-id="73966-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73966-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73966-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73966-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="73966-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="73966-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="73966-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73966-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73966-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73966-114">Not supported.</span></span> |
| <span data-ttu-id="73966-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73966-115">Application</span></span>                            | <span data-ttu-id="73966-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="73966-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="73966-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73966-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73966-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73966-118">Request headers</span></span>

| <span data-ttu-id="73966-119">Nome</span><span class="sxs-lookup"><span data-stu-id="73966-119">Name</span></span>       | <span data-ttu-id="73966-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="73966-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="73966-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="73966-121">Authorization</span></span> | <span data-ttu-id="73966-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73966-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73966-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="73966-124">Content-type</span></span> | <span data-ttu-id="73966-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73966-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73966-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73966-127">Request body</span></span>

<span data-ttu-id="73966-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="73966-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="73966-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="73966-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73966-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="73966-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73966-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73966-131">Property</span></span>     | <span data-ttu-id="73966-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="73966-132">Type</span></span>        | <span data-ttu-id="73966-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="73966-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73966-134">displayName</span><span class="sxs-lookup"><span data-stu-id="73966-134">displayName</span></span>|<span data-ttu-id="73966-135">String</span><span class="sxs-lookup"><span data-stu-id="73966-135">String</span></span>|<span data-ttu-id="73966-136">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="73966-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="73966-137">Intervalos</span><span class="sxs-lookup"><span data-stu-id="73966-137">ipRanges</span></span>|<span data-ttu-id="73966-138">Coleção [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="73966-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="73966-139">Lista de intervalos de endereços IP no formato CIDR do IPv4 (1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="73966-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="73966-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="73966-140">isTrusted</span></span>|<span data-ttu-id="73966-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="73966-141">Boolean</span></span>|<span data-ttu-id="73966-142">O valor é `true` se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="73966-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="73966-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="73966-143">Response</span></span>

<span data-ttu-id="73966-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73966-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73966-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73966-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73966-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73966-147">Request</span></span>

<span data-ttu-id="73966-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73966-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73966-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="73966-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
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
# <a name="c"></a>[<span data-ttu-id="73966-150">C#</span><span class="sxs-lookup"><span data-stu-id="73966-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73966-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73966-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73966-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73966-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73966-153">Java</span><span class="sxs-lookup"><span data-stu-id="73966-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73966-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="73966-154">Response</span></span>

<span data-ttu-id="73966-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73966-155">The following is an example of the response.</span></span>

> <span data-ttu-id="73966-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73966-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
