---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d075fbcf2f912c125f1af65ae7368a2a6b2c75bc
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535643"
---
# <a name="list-channels"></a><span data-ttu-id="8767f-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="8767f-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8767f-104">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8767f-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8767f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8767f-105">Permissions</span></span>

<span data-ttu-id="8767f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8767f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8767f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8767f-108">Permission type</span></span>      | <span data-ttu-id="8767f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8767f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8767f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8767f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8767f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8767f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8767f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8767f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8767f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8767f-113">Not supported.</span></span>    |
|<span data-ttu-id="8767f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8767f-114">Application</span></span> | <span data-ttu-id="8767f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8767f-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8767f-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8767f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8767f-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8767f-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8767f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8767f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8767f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8767f-119">Optional query parameters</span></span>
<span data-ttu-id="8767f-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8767f-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8767f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8767f-121">Request headers</span></span>

| <span data-ttu-id="8767f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8767f-122">Header</span></span>       | <span data-ttu-id="8767f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8767f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8767f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8767f-124">Authorization</span></span>  | <span data-ttu-id="8767f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8767f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8767f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8767f-127">Request body</span></span>

<span data-ttu-id="8767f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8767f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8767f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8767f-129">Response</span></span>

<span data-ttu-id="8767f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8767f-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8767f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8767f-131">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="8767f-132">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="8767f-132">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="8767f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8767f-133">Request</span></span>

<span data-ttu-id="8767f-134">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="8767f-134">The following example shows a request to list all channels.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8767f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8767f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8767f-136">C#</span><span class="sxs-lookup"><span data-stu-id="8767f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8767f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8767f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8767f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8767f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8767f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8767f-139">Response</span></span>

<span data-ttu-id="8767f-140">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="8767f-140">The following is the response.</span></span>

> <span data-ttu-id="8767f-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8767f-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8767f-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8767f-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="8767f-143">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="8767f-143">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="8767f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8767f-144">Request</span></span>

<span data-ttu-id="8767f-145">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="8767f-145">The following example shows a request to list all private channels.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8767f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8767f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8767f-147">C#</span><span class="sxs-lookup"><span data-stu-id="8767f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8767f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8767f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8767f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8767f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8767f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8767f-150">Response</span></span>

<span data-ttu-id="8767f-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8767f-151">The following is an example of the response.</span></span>

> <span data-ttu-id="8767f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8767f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
