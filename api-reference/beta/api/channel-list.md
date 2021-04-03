---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1297f7434c7eba8c2145ad31a8c94a7b3a3fb1e8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507289"
---
# <a name="list-channels"></a><span data-ttu-id="789be-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="789be-103">List channels</span></span>

<span data-ttu-id="789be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="789be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="789be-105">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="789be-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="789be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="789be-106">Permissions</span></span>

<span data-ttu-id="789be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="789be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="789be-109">Permission type</span></span>      | <span data-ttu-id="789be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="789be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="789be-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="789be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="789be-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789be-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="789be-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="789be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="789be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="789be-114">Not supported.</span></span>    |
|<span data-ttu-id="789be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="789be-115">Application</span></span> | <span data-ttu-id="789be-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789be-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="789be-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="789be-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="789be-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="789be-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="789be-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="789be-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="789be-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="789be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="789be-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="789be-121">Optional query parameters</span></span>
<span data-ttu-id="789be-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="789be-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="789be-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="789be-123">Request headers</span></span>

| <span data-ttu-id="789be-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="789be-124">Header</span></span>       | <span data-ttu-id="789be-125">Valor</span><span class="sxs-lookup"><span data-stu-id="789be-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="789be-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="789be-126">Authorization</span></span>  | <span data-ttu-id="789be-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="789be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="789be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="789be-129">Request body</span></span>

<span data-ttu-id="789be-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="789be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="789be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="789be-131">Response</span></span>

<span data-ttu-id="789be-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="789be-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="789be-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="789be-133">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="789be-134">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="789be-134">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="789be-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="789be-135">Request</span></span>

<span data-ttu-id="789be-136">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="789be-136">The following example shows a request to list all channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="789be-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="789be-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[<span data-ttu-id="789be-138">C#</span><span class="sxs-lookup"><span data-stu-id="789be-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="789be-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="789be-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="789be-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="789be-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="789be-141">Java</span><span class="sxs-lookup"><span data-stu-id="789be-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="789be-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="789be-142">Response</span></span>

<span data-ttu-id="789be-143">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="789be-143">The following is the response.</span></span>

> <span data-ttu-id="789be-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="789be-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="789be-145">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="789be-145">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="789be-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="789be-146">Request</span></span>

<span data-ttu-id="789be-147">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="789be-147">The following example shows a request to list all private channels.</span></span>



# <a name="http"></a>[<span data-ttu-id="789be-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="789be-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="789be-149">C#</span><span class="sxs-lookup"><span data-stu-id="789be-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="789be-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="789be-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="789be-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="789be-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="789be-152">Java</span><span class="sxs-lookup"><span data-stu-id="789be-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="789be-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="789be-153">Response</span></span>

<span data-ttu-id="789be-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="789be-154">The following is an example of the response.</span></span>

> <span data-ttu-id="789be-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="789be-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "19:982abbfca323a582f0a6d00ae2deca@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "test private team",
      "membershipType": "private"
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


