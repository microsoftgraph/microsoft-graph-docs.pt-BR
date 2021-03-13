---
title: Obter guia no chat
description: 'Recupere as propriedades e as relações da guia especificada em um chat. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0cdba3257a6008005597dcc7c9f6a1cc60bdf06
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775840"
---
# <a name="get-tab-in-chat"></a><span data-ttu-id="56d50-103">Obter guia no chat</span><span class="sxs-lookup"><span data-stu-id="56d50-103">Get tab in chat</span></span>

<span data-ttu-id="56d50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56d50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56d50-105">Recupere as propriedades e as relações da guia [especificada](../resources/teamstab.md) em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="56d50-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="56d50-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="56d50-106">Permissions</span></span>
<span data-ttu-id="56d50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d50-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56d50-109">Permission type</span></span>      | <span data-ttu-id="56d50-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56d50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d50-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56d50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56d50-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d50-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="56d50-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56d50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d50-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56d50-114">Not supported.</span></span>    |
|<span data-ttu-id="56d50-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56d50-115">Application</span></span> | <span data-ttu-id="56d50-116">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d50-116">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="56d50-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56d50-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /chats/{chat-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56d50-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56d50-118">Optional query parameters</span></span>

<span data-ttu-id="56d50-119">Este método oferece suporte aos parâmetros de consulta `$select` e `$expand`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56d50-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56d50-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56d50-120">Request headers</span></span>
| <span data-ttu-id="56d50-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56d50-121">Header</span></span>       | <span data-ttu-id="56d50-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56d50-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56d50-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56d50-123">Authorization</span></span>  | <span data-ttu-id="56d50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56d50-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56d50-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56d50-126">Request body</span></span>
<span data-ttu-id="56d50-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56d50-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56d50-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d50-128">Response</span></span>

<span data-ttu-id="56d50-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56d50-129">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56d50-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56d50-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="56d50-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56d50-131">Request</span></span>
<span data-ttu-id="56d50-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56d50-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56d50-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="56d50-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tab_in_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d?$expand=teamsApp
```
# <a name="c"></a>[<span data-ttu-id="56d50-134">C#</span><span class="sxs-lookup"><span data-stu-id="56d50-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56d50-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d50-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56d50-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56d50-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56d50-137">Java</span><span class="sxs-lookup"><span data-stu-id="56d50-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="56d50-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d50-138">Response</span></span>
<span data-ttu-id="56d50-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56d50-139">The following is an example of the response.</span></span> 

><span data-ttu-id="56d50-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56d50-140">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "messageId": "1607411534158",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="56d50-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="56d50-141">See also</span></span>

- [<span data-ttu-id="56d50-142">Guia obter no canal</span><span class="sxs-lookup"><span data-stu-id="56d50-142">Get tab in channel</span></span>](channel-get-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


