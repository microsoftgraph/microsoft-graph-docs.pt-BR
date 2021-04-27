---
title: Get primaryChannel
description: Recupere a propriedade de navegação de uma equipe que permita acesso ao seu canal Geral padrão.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 87b68bc313fbfc03e9ab52d8e9a77ea8b4fbebab
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050812"
---
# <a name="get-primarychannel"></a><span data-ttu-id="1a632-103">Get primaryChannel</span><span class="sxs-lookup"><span data-stu-id="1a632-103">Get primaryChannel</span></span>

<span data-ttu-id="1a632-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a632-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a632-105">Obtenha o canal [padrão](../resources/channel.md), **Geral**, de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1a632-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a632-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a632-106">Permissions</span></span>
<span data-ttu-id="1a632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a632-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a632-109">Permission type</span></span>      | <span data-ttu-id="1a632-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a632-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a632-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a632-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a632-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a632-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="1a632-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a632-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a632-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a632-114">Not supported.</span></span>    |
|<span data-ttu-id="1a632-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a632-115">Application</span></span> | <span data-ttu-id="1a632-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a632-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> |

> <span data-ttu-id="1a632-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1a632-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1a632-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="1a632-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a632-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a632-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a632-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a632-121">Optional query parameters</span></span>

<span data-ttu-id="1a632-122">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a632-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a632-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a632-123">Request headers</span></span>
| <span data-ttu-id="1a632-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a632-124">Header</span></span>       | <span data-ttu-id="1a632-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1a632-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a632-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a632-126">Authorization</span></span>  | <span data-ttu-id="1a632-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a632-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a632-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a632-129">Request body</span></span>
<span data-ttu-id="1a632-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a632-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a632-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a632-131">Response</span></span>

<span data-ttu-id="1a632-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a632-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a632-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a632-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a632-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a632-134">Request</span></span>
<span data-ttu-id="1a632-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a632-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a632-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a632-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="1a632-137">C#</span><span class="sxs-lookup"><span data-stu-id="1a632-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a632-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a632-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a632-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a632-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a632-140">Java</span><span class="sxs-lookup"><span data-stu-id="1a632-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-primarychannel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1a632-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a632-141">Response</span></span>
<span data-ttu-id="1a632-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a632-142">The following is an example of the response.</span></span> 

><span data-ttu-id="1a632-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a632-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "isFavoriteByDefault": null,
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47",
    "membershipType": "standard"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get primaryChannel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


