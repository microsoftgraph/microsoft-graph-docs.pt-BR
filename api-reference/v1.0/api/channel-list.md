---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 87895685781982e054714b2991441250cb1738b3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202223"
---
# <a name="list-channels"></a><span data-ttu-id="66555-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="66555-103">List channels</span></span>

<span data-ttu-id="66555-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66555-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="66555-105">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="66555-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66555-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66555-106">Permissions</span></span>

<span data-ttu-id="66555-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66555-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66555-109">Permission type</span></span>      | <span data-ttu-id="66555-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66555-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66555-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66555-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66555-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66555-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="66555-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66555-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66555-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66555-114">Not supported.</span></span>    |
|<span data-ttu-id="66555-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66555-115">Application</span></span> | <span data-ttu-id="66555-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66555-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="66555-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="66555-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="66555-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="66555-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="66555-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66555-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66555-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66555-120">Optional query parameters</span></span>

<span data-ttu-id="66555-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66555-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66555-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66555-122">Request headers</span></span>

| <span data-ttu-id="66555-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66555-123">Header</span></span>       | <span data-ttu-id="66555-124">Valor</span><span class="sxs-lookup"><span data-stu-id="66555-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66555-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="66555-125">Authorization</span></span>  | <span data-ttu-id="66555-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66555-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66555-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66555-128">Request body</span></span>

<span data-ttu-id="66555-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66555-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66555-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="66555-130">Response</span></span>

<span data-ttu-id="66555-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66555-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66555-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66555-132">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="66555-133">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="66555-133">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="66555-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66555-134">Request</span></span>

<span data-ttu-id="66555-135">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="66555-135">The following example shows a request to list all channels.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels
```


#### <a name="response"></a><span data-ttu-id="66555-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="66555-136">Response</span></span>

<span data-ttu-id="66555-137">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="66555-137">The following is the response.</span></span>

> <span data-ttu-id="66555-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66555-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="66555-139">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="66555-139">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="66555-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66555-140">Request</span></span>

<span data-ttu-id="66555-141">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="66555-141">The following example shows a request to list all private channels.</span></span>


<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```

#### <a name="response"></a><span data-ttu-id="66555-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="66555-142">Response</span></span>

<span data-ttu-id="66555-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66555-143">The following is an example of the response.</span></span>

> <span data-ttu-id="66555-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66555-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
