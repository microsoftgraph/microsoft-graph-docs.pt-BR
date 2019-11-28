---
title: Atualizar ipnamedlocation
description: Atualiza as propriedades de um objeto ipNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de1811094d6be3148610078d25e0afafecc3fb04
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636845"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="b482c-103">Atualizar ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="b482c-103">Update ipNamedlocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b482c-104">Atualiza as propriedades de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="b482c-104">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b482c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b482c-105">Permissions</span></span>

<span data-ttu-id="b482c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b482c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b482c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b482c-108">Permission type</span></span>                        | <span data-ttu-id="b482c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b482c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b482c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b482c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b482c-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b482c-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="b482c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b482c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b482c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b482c-113">Not supported.</span></span> |
| <span data-ttu-id="b482c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b482c-114">Application</span></span>                            | <span data-ttu-id="b482c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b482c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b482c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b482c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b482c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b482c-117">Request headers</span></span>

| <span data-ttu-id="b482c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b482c-118">Name</span></span>       | <span data-ttu-id="b482c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b482c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b482c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b482c-120">Authorization</span></span> | <span data-ttu-id="b482c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b482c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b482c-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="b482c-123">Content-type</span></span> | <span data-ttu-id="b482c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b482c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b482c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b482c-126">Request body</span></span>

<span data-ttu-id="b482c-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b482c-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b482c-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b482c-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b482c-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b482c-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b482c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b482c-130">Property</span></span>     | <span data-ttu-id="b482c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b482c-131">Type</span></span>        | <span data-ttu-id="b482c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b482c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b482c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b482c-133">displayName</span></span>|<span data-ttu-id="b482c-134">String</span><span class="sxs-lookup"><span data-stu-id="b482c-134">String</span></span>|<span data-ttu-id="b482c-135">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="b482c-135">Human-readable name of the location.</span></span>|
|<span data-ttu-id="b482c-136">Intervalos</span><span class="sxs-lookup"><span data-stu-id="b482c-136">ipRanges</span></span>|<span data-ttu-id="b482c-137">Coleção [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b482c-137">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="b482c-138">Lista de intervalos de endereços IP no formato CIDR do IPv4 (1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="b482c-138">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="b482c-139">isTrusted</span><span class="sxs-lookup"><span data-stu-id="b482c-139">isTrusted</span></span>|<span data-ttu-id="b482c-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="b482c-140">Boolean</span></span>|<span data-ttu-id="b482c-141">O valor é `true` se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="b482c-141">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="b482c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b482c-142">Response</span></span>

<span data-ttu-id="b482c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b482c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b482c-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b482c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b482c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b482c-146">Request</span></span>

<span data-ttu-id="b482c-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b482c-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b482c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b482c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b482c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b482c-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b482c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b482c-150">Response</span></span>

<span data-ttu-id="b482c-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b482c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b482c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b482c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
