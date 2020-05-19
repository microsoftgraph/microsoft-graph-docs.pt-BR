---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1113880beb3386f5cd0c220028caa5e85f4de30b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288610"
---
# <a name="list-channels"></a><span data-ttu-id="a8dd5-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="a8dd5-103">List channels</span></span>

<span data-ttu-id="a8dd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8dd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8dd5-105">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a8dd5-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8dd5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8dd5-106">Permissions</span></span>

<span data-ttu-id="a8dd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8dd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8dd5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8dd5-109">Permission type</span></span>      | <span data-ttu-id="a8dd5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8dd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8dd5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8dd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8dd5-112">Channel. ReadBasic. All, ChannelSettings. Read. All, ChannelSettings. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8dd5-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8dd5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8dd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8dd5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-114">Not supported.</span></span>    |
|<span data-ttu-id="a8dd5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8dd5-115">Application</span></span> | <span data-ttu-id="a8dd5-116">Channel. ReadBasic. All, ChannelSettings. Read. All, ChannelSettings. ReadWrite. All, ChannelSettings. Read. Group ([RSC](https://aka.ms/teams-rsc)), ChannelSettings. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8dd5-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, ChannelSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), ChannelSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="a8dd5-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a8dd5-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8dd5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8dd5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8dd5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8dd5-120">Optional query parameters</span></span>
<span data-ttu-id="a8dd5-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8dd5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8dd5-122">Request headers</span></span>

| <span data-ttu-id="a8dd5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8dd5-123">Header</span></span>       | <span data-ttu-id="a8dd5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a8dd5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8dd5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8dd5-125">Authorization</span></span>  | <span data-ttu-id="a8dd5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8dd5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8dd5-128">Request body</span></span>

<span data-ttu-id="a8dd5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8dd5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8dd5-130">Response</span></span>

<span data-ttu-id="a8dd5-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8dd5-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8dd5-132">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="a8dd5-133">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="a8dd5-133">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="a8dd5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8dd5-134">Request</span></span>

<span data-ttu-id="a8dd5-135">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-135">The following example shows a request to list all channels.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8dd5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8dd5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="a8dd5-137">C#</span><span class="sxs-lookup"><span data-stu-id="a8dd5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8dd5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8dd5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8dd5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8dd5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a8dd5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8dd5-140">Response</span></span>

<span data-ttu-id="a8dd5-141">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-141">The following is the response.</span></span>

> <span data-ttu-id="a8dd5-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8dd5-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-143">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="a8dd5-144">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="a8dd5-144">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="a8dd5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8dd5-145">Request</span></span>

<span data-ttu-id="a8dd5-146">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-146">The following example shows a request to list all private channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8dd5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8dd5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="a8dd5-148">C#</span><span class="sxs-lookup"><span data-stu-id="a8dd5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8dd5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8dd5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8dd5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8dd5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8dd5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8dd5-151">Response</span></span>

<span data-ttu-id="a8dd5-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-152">The following is an example of the response.</span></span>

> <span data-ttu-id="a8dd5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8dd5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
