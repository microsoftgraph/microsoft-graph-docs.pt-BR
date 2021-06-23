---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: akjo
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c864e2dd8da2dbf3e5239ecbaa747c28fb96c05e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059958"
---
# <a name="list-channels"></a><span data-ttu-id="a354c-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="a354c-103">List channels</span></span>

<span data-ttu-id="a354c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a354c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a354c-105">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a354c-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a354c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a354c-106">Permissions</span></span>

<span data-ttu-id="a354c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a354c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a354c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a354c-109">Permission type</span></span>      | <span data-ttu-id="a354c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a354c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a354c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a354c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a354c-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a354c-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a354c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a354c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a354c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a354c-114">Not supported.</span></span>    |
|<span data-ttu-id="a354c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a354c-115">Application</span></span> | <span data-ttu-id="a354c-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a354c-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a354c-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a354c-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="a354c-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="a354c-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a354c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a354c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a354c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a354c-121">Optional query parameters</span></span>
<span data-ttu-id="a354c-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a354c-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="use-select-for-better-performance"></a><span data-ttu-id="a354c-123">Use $select para melhorar o desempenho</span><span class="sxs-lookup"><span data-stu-id="a354c-123">Use $select for better performance</span></span>
<span data-ttu-id="a354c-124">Preencher as propriedades **email** e **moderationSettings** de um canal é uma operação cara que resulta em desempenho lento.</span><span class="sxs-lookup"><span data-stu-id="a354c-124">Populating the **email** and **moderationSettings** properties for a channel is an expensive operation that results in slow performance.</span></span> <span data-ttu-id="a354c-125">Use `$select` para excluir o **email** e as propriedades **moderationSettings** para melhorar o desempenho.</span><span class="sxs-lookup"><span data-stu-id="a354c-125">Use `$select` to exclude the **email** and **moderationSettings** properties to improve performance.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a354c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a354c-126">Request headers</span></span>

| <span data-ttu-id="a354c-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a354c-127">Header</span></span>       | <span data-ttu-id="a354c-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a354c-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a354c-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a354c-129">Authorization</span></span>  | <span data-ttu-id="a354c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a354c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a354c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a354c-132">Request body</span></span>

<span data-ttu-id="a354c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a354c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a354c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a354c-134">Response</span></span>

<span data-ttu-id="a354c-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a354c-135">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a354c-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a354c-136">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="a354c-137">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="a354c-137">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="a354c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a354c-138">Request</span></span>

<span data-ttu-id="a354c-139">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="a354c-139">The following example shows a request to list all channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="a354c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a354c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[<span data-ttu-id="a354c-141">C#</span><span class="sxs-lookup"><span data-stu-id="a354c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a354c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a354c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a354c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a354c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a354c-144">Java</span><span class="sxs-lookup"><span data-stu-id="a354c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a354c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a354c-145">Response</span></span>

<span data-ttu-id="a354c-146">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="a354c-146">The following is the response.</span></span>

> <span data-ttu-id="a354c-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a354c-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="a354c-148">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="a354c-148">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="a354c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a354c-149">Request</span></span>

<span data-ttu-id="a354c-150">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="a354c-150">The following example shows a request to list all private channels.</span></span>



# <a name="http"></a>[<span data-ttu-id="a354c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a354c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="a354c-152">C#</span><span class="sxs-lookup"><span data-stu-id="a354c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a354c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a354c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a354c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a354c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a354c-155">Java</span><span class="sxs-lookup"><span data-stu-id="a354c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="a354c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a354c-156">Response</span></span>

<span data-ttu-id="a354c-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a354c-157">The following is an example of the response.</span></span>

> <span data-ttu-id="a354c-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a354c-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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


