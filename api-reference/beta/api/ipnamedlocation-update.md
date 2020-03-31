---
title: Atualizar ipnamedlocation
description: Atualiza as propriedades de um objeto ipNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 50ae9a0e1523a625b2deaf971e9031a1e2ea1bb1
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062257"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="9274f-103">Atualizar ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="9274f-103">Update ipNamedlocation</span></span>

<span data-ttu-id="9274f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9274f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9274f-105">Atualiza as propriedades de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="9274f-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9274f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9274f-106">Permissions</span></span>

<span data-ttu-id="9274f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9274f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9274f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9274f-109">Permission type</span></span>                        | <span data-ttu-id="9274f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9274f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9274f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9274f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9274f-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="9274f-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="9274f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9274f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9274f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9274f-114">Not supported.</span></span> |
| <span data-ttu-id="9274f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9274f-115">Application</span></span>                            | <span data-ttu-id="9274f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9274f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9274f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9274f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9274f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9274f-118">Request headers</span></span>

| <span data-ttu-id="9274f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9274f-119">Name</span></span>       | <span data-ttu-id="9274f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9274f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9274f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9274f-121">Authorization</span></span> | <span data-ttu-id="9274f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9274f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9274f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9274f-124">Content-type</span></span> | <span data-ttu-id="9274f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9274f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9274f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9274f-127">Request body</span></span>

<span data-ttu-id="9274f-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9274f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9274f-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9274f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9274f-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9274f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9274f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9274f-131">Property</span></span>     | <span data-ttu-id="9274f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9274f-132">Type</span></span>        | <span data-ttu-id="9274f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9274f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9274f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9274f-134">displayName</span></span>|<span data-ttu-id="9274f-135">String</span><span class="sxs-lookup"><span data-stu-id="9274f-135">String</span></span>|<span data-ttu-id="9274f-136">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="9274f-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="9274f-137">Intervalos</span><span class="sxs-lookup"><span data-stu-id="9274f-137">ipRanges</span></span>|<span data-ttu-id="9274f-138">Coleção [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="9274f-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="9274f-139">Lista de intervalos de endereços IP no formato CIDR do IPv4 (1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="9274f-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="9274f-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="9274f-140">isTrusted</span></span>|<span data-ttu-id="9274f-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="9274f-141">Boolean</span></span>|<span data-ttu-id="9274f-142">O valor é `true` se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="9274f-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="9274f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9274f-143">Response</span></span>

<span data-ttu-id="9274f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9274f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9274f-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9274f-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9274f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9274f-147">Request</span></span>

<span data-ttu-id="9274f-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9274f-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9274f-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="9274f-149">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9274f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9274f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9274f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9274f-151">Response</span></span>

<span data-ttu-id="9274f-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9274f-152">The following is an example of the response.</span></span>

> <span data-ttu-id="9274f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9274f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
