---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 631b592dc75bc34d462fe27fee674f94035c1ab5
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589225"
---
# <a name="get-channel"></a><span data-ttu-id="e0e51-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="e0e51-103">Get channel</span></span>

<span data-ttu-id="e0e51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0e51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e51-105">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e0e51-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0e51-106">Permissions</span></span>

<span data-ttu-id="e0e51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0e51-109">Permission type</span></span>      | <span data-ttu-id="e0e51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0e51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0e51-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0e51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0e51-112">Channel. ReadBasic. All, ChannelSettings. Read. All, ChannelSettings. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0e51-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0e51-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0e51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0e51-114">Not supported.</span></span>    |
|<span data-ttu-id="e0e51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0e51-115">Application</span></span> | <span data-ttu-id="e0e51-116">Channel. ReadBasic. All, ChannelSettings. Read. All, ChannelSettings. ReadWrite. All, ChannelSettings. Read. Group *, ChannelSettings. Edit. Group*, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0e51-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, ChannelSettings.Read.Group *, ChannelSettings.Edit.Group*, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="e0e51-117">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e0e51-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="e0e51-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e0e51-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e0e51-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e0e51-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e0e51-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e51-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0e51-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0e51-121">Optional query parameters</span></span>

<span data-ttu-id="e0e51-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e51-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0e51-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e51-123">Request headers</span></span>

| <span data-ttu-id="e0e51-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0e51-124">Header</span></span>       | <span data-ttu-id="e0e51-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e0e51-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0e51-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0e51-126">Authorization</span></span>  | <span data-ttu-id="e0e51-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0e51-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0e51-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e51-129">Request body</span></span>

<span data-ttu-id="e0e51-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0e51-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0e51-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e51-131">Response</span></span>

<span data-ttu-id="e0e51-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e51-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0e51-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0e51-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0e51-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e51-134">Request</span></span>

<span data-ttu-id="e0e51-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e51-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0e51-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e51-136">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

# <a name="c"></a>[<span data-ttu-id="e0e51-137">C#</span><span class="sxs-lookup"><span data-stu-id="e0e51-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0e51-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e51-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0e51-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0e51-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e0e51-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e51-140">Response</span></span>

<span data-ttu-id="e0e51-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e51-141">Here is an example of the response.</span></span>

><span data-ttu-id="e0e51-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0e51-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value",
    "membershipType": "membership-type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
