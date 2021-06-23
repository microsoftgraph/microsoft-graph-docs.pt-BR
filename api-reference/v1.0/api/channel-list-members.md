---
title: Listar membros de um canal
description: Liste os membros de um canal.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dd59e40abbd24a80af11fa4bcde48ecbbe3def98
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060016"
---
# <a name="list-members-of-a-channel"></a><span data-ttu-id="3bf0d-103">Listar membros de um canal</span><span class="sxs-lookup"><span data-stu-id="3bf0d-103">List members of a channel</span></span>

<span data-ttu-id="3bf0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bf0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3bf0d-105">Recupere a lista [conversationMembers](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="3bf0d-105">Retrieve a list of [conversationMembers](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3bf0d-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-106">The membership IDs returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="3bf0d-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="3bf0d-p102">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf0d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bf0d-110">Permissions</span></span>

<span data-ttu-id="3bf0d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bf0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf0d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bf0d-113">Permission Type</span></span>|<span data-ttu-id="3bf0d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bf0d-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3bf0d-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bf0d-115">Delegated (work or school account)</span></span>|<span data-ttu-id="3bf0d-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf0d-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="3bf0d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bf0d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bf0d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-118">Not supported.</span></span>|
|<span data-ttu-id="3bf0d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bf0d-119">Application</span></span>|<span data-ttu-id="3bf0d-120">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf0d-120">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3bf0d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bf0d-121">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
GET /teams/{team-id}/channels/{channel-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bf0d-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bf0d-122">Optional query parameters</span></span>

<span data-ttu-id="3bf0d-123">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bf0d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bf0d-124">Request headers</span></span>

| <span data-ttu-id="3bf0d-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bf0d-125">Header</span></span>       | <span data-ttu-id="3bf0d-126">Valor</span><span class="sxs-lookup"><span data-stu-id="3bf0d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3bf0d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bf0d-127">Authorization</span></span>  | <span data-ttu-id="3bf0d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3bf0d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bf0d-130">Request body</span></span>

<span data-ttu-id="3bf0d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bf0d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bf0d-132">Response</span></span>

<span data-ttu-id="3bf0d-133">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-133">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bf0d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bf0d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bf0d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bf0d-135">Request</span></span>

<span data-ttu-id="3bf0d-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3bf0d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bf0d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel-list_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/2ab9c796-2902-45f8-b712-7c5a63cf41c4/channels/19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype/members
```
# <a name="c"></a>[<span data-ttu-id="3bf0d-138">C#</span><span class="sxs-lookup"><span data-stu-id="3bf0d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-list-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bf0d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bf0d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-list-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bf0d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bf0d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-list-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bf0d-141">Java</span><span class="sxs-lookup"><span data-stu-id="3bf0d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-list-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3bf0d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bf0d-142">Response</span></span>

<span data-ttu-id="3bf0d-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-143">Here is an example of the response.</span></span>

><span data-ttu-id="3bf0d-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3bf0d-144">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
"@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('2ab9c796-2902-45f8-b712-7c5a63cf41c4')/channels('19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype')/members",
"@odata.count": 2,
"value": [
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ=",
        "roles": [],
        "displayName": "Jane Doe",
        "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
        "email": "jdoe@teamsip.onmicrosoft.com"
    },
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNiMzI0NmY0NC1jMDkxLTQ2MjctOTZjNi0yNWIxOGZhMmM5MTA=",
        "roles": [
            "owner"
        ],
        "displayName": "Ace John",
        "userId": "b3246f44-c091-4627-96c6-25b18fa2c910",
        "email": "ajohn@teamsip.onmicrosoft.com"
    }
]
}

```

## <a name="see-also"></a><span data-ttu-id="3bf0d-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="3bf0d-145">See also</span></span>

- [<span data-ttu-id="3bf0d-146">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="3bf0d-146">List members of team</span></span>](team-list-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
