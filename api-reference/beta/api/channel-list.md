---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7aeec6da0c25a2ac5dee28b29871c8ead546eb2c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200935"
---
# <a name="list-channels"></a><span data-ttu-id="d43fc-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="d43fc-103">List channels</span></span>

<span data-ttu-id="d43fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d43fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d43fc-105">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d43fc-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d43fc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d43fc-106">Permissions</span></span>

<span data-ttu-id="d43fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d43fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d43fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d43fc-109">Permission type</span></span>      | <span data-ttu-id="d43fc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d43fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d43fc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d43fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d43fc-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d43fc-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d43fc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d43fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d43fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d43fc-114">Not supported.</span></span>    |
|<span data-ttu-id="d43fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d43fc-115">Application</span></span> | <span data-ttu-id="d43fc-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d43fc-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d43fc-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d43fc-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d43fc-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d43fc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d43fc-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d43fc-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d43fc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d43fc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d43fc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d43fc-121">Optional query parameters</span></span>
<span data-ttu-id="d43fc-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d43fc-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d43fc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d43fc-123">Request headers</span></span>

| <span data-ttu-id="d43fc-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d43fc-124">Header</span></span>       | <span data-ttu-id="d43fc-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d43fc-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d43fc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d43fc-126">Authorization</span></span>  | <span data-ttu-id="d43fc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d43fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d43fc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d43fc-129">Request body</span></span>

<span data-ttu-id="d43fc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d43fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d43fc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d43fc-131">Response</span></span>

<span data-ttu-id="d43fc-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d43fc-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d43fc-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d43fc-133">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="d43fc-134">Exemplo 1: Listar todos os canais</span><span class="sxs-lookup"><span data-stu-id="d43fc-134">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="d43fc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d43fc-135">Request</span></span>

<span data-ttu-id="d43fc-136">O exemplo a seguir mostra uma solicitação para listar todos os canais.</span><span class="sxs-lookup"><span data-stu-id="d43fc-136">The following example shows a request to list all channels.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels
```

#### <a name="response"></a><span data-ttu-id="d43fc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d43fc-137">Response</span></span>

<span data-ttu-id="d43fc-138">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="d43fc-138">The following is the response.</span></span>

> <span data-ttu-id="d43fc-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d43fc-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="d43fc-140">Exemplo 2: Listar todos os canais privados</span><span class="sxs-lookup"><span data-stu-id="d43fc-140">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="d43fc-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d43fc-141">Request</span></span>

<span data-ttu-id="d43fc-142">O exemplo a seguir mostra uma solicitação para listar todos os canais privados.</span><span class="sxs-lookup"><span data-stu-id="d43fc-142">The following example shows a request to list all private channels.</span></span>


<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```


#### <a name="response"></a><span data-ttu-id="d43fc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d43fc-143">Response</span></span>

<span data-ttu-id="d43fc-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d43fc-144">The following is an example of the response.</span></span>

> <span data-ttu-id="d43fc-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d43fc-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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


