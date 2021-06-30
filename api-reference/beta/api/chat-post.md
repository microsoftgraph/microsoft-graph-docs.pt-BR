---
title: Criar chat
description: Crie um novo objeto de chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1e6f844b1c216eae63c85644aca556812fdadc1
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207912"
---
# <a name="create-chat"></a><span data-ttu-id="7c62f-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="7c62f-103">Create chat</span></span>
<span data-ttu-id="7c62f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c62f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c62f-105">Crie um novo [objeto de chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="7c62f-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c62f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c62f-106">Permissions</span></span>
<span data-ttu-id="7c62f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c62f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c62f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c62f-109">Permission type</span></span>|<span data-ttu-id="7c62f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c62f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c62f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c62f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c62f-112">Chat.Create, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c62f-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="7c62f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c62f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c62f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c62f-114">Not supported.</span></span> |
|<span data-ttu-id="7c62f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c62f-115">Application</span></span> | <span data-ttu-id="7c62f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c62f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c62f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c62f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="7c62f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c62f-118">Request headers</span></span>
|<span data-ttu-id="7c62f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7c62f-119">Name</span></span>|<span data-ttu-id="7c62f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c62f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c62f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c62f-121">Authorization</span></span>|<span data-ttu-id="7c62f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c62f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c62f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c62f-124">Content-Type</span></span>|<span data-ttu-id="7c62f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c62f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c62f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c62f-127">Request body</span></span>
<span data-ttu-id="7c62f-128">No corpo da solicitação, fornece uma representação JSON do [objeto chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="7c62f-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="7c62f-129">A tabela a seguir lista as propriedades necessárias para criar um objeto de chat.</span><span class="sxs-lookup"><span data-stu-id="7c62f-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="7c62f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c62f-130">Property</span></span>|<span data-ttu-id="7c62f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c62f-131">Type</span></span>|<span data-ttu-id="7c62f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c62f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c62f-133">topic</span><span class="sxs-lookup"><span data-stu-id="7c62f-133">topic</span></span>|<span data-ttu-id="7c62f-134">(Opcional) Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c62f-134">(Optional) String</span></span>|<span data-ttu-id="7c62f-135">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="7c62f-135">The title of the chat.</span></span> <span data-ttu-id="7c62f-136">O título do chat só poderá ser fornecido se o chat for do `group` tipo.</span><span class="sxs-lookup"><span data-stu-id="7c62f-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="7c62f-137">chatType</span><span class="sxs-lookup"><span data-stu-id="7c62f-137">chatType</span></span>|[<span data-ttu-id="7c62f-138">chatType</span><span class="sxs-lookup"><span data-stu-id="7c62f-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="7c62f-139">Especifica o tipo de chat.</span><span class="sxs-lookup"><span data-stu-id="7c62f-139">Specifies the type of chat.</span></span> <span data-ttu-id="7c62f-140">Os valores possíveis são: `group` e `oneOnOne` .</span><span class="sxs-lookup"><span data-stu-id="7c62f-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="7c62f-141">membros</span><span class="sxs-lookup"><span data-stu-id="7c62f-141">members</span></span>|<span data-ttu-id="7c62f-142">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7c62f-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="7c62f-143">Lista de membros da conversa que devem ser adicionados.</span><span class="sxs-lookup"><span data-stu-id="7c62f-143">List of conversation members that should be added.</span></span> <span data-ttu-id="7c62f-144">Todos os usuários, incluindo o usuário que inicia a solicitação de criação, que participarão do chat devem ser especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="7c62f-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|
|<span data-ttu-id="7c62f-145">installedApps</span><span class="sxs-lookup"><span data-stu-id="7c62f-145">installedApps</span></span>| <span data-ttu-id="7c62f-146">Coleção [teamsApp](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c62f-146">[teamsApp](../resources/teamsapp.md) collection</span></span>|<span data-ttu-id="7c62f-147">Lista de aplicativos que devem ser instalados no chat.</span><span class="sxs-lookup"><span data-stu-id="7c62f-147">List of apps that should be installed in the chat.</span></span>|

> <span data-ttu-id="7c62f-148">**Observação:** Atualmente, há suporte para apenas uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7c62f-148">**Note:** Currently, only one app installation is supported.</span></span> <span data-ttu-id="7c62f-149">Se várias instalações de aplicativos estão listadas na solicitação, a resposta será um `Bad Request` erro.</span><span class="sxs-lookup"><span data-stu-id="7c62f-149">If multiple app installations are listed in the request, the response will be a `Bad Request` error.</span></span>

## <a name="response"></a><span data-ttu-id="7c62f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c62f-150">Response</span></span>

### <a name="response-for-creating-a-one-on-one-chat-without-installed-apps"></a><span data-ttu-id="7c62f-151">Resposta para criar um chat um-a-um sem aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="7c62f-151">Response for creating a one-on-one chat without installed apps</span></span>
<span data-ttu-id="7c62f-152">Se tiver êxito, este método retornará um código `201 Created` de resposta e o recurso de [chat](../resources/chat.md) recém-criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c62f-152">If successful, this method returns a `201 Created` response code and the newly created [chat](../resources/chat.md) resource in the response body.</span></span>

### <a name="response-for-creating-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="7c62f-153">Resposta para criar um chat um-a-um com aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="7c62f-153">Response for creating a one-on-one chat with installed apps</span></span>
<span data-ttu-id="7c62f-154">Se tiver êxito, este método retornará um código de resposta e um header location que contém um `202 Accepted` link para [o teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7c62f-154">If successful, this method returns a `202 Accepted` response code and Location header that contains a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="7c62f-155">O link pode ser usado para obter o status e os detalhes da operação.</span><span class="sxs-lookup"><span data-stu-id="7c62f-155">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="7c62f-156">Para obter detalhes, consulte [Obter operação no chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span><span class="sxs-lookup"><span data-stu-id="7c62f-156">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="examples"></a><span data-ttu-id="7c62f-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7c62f-157">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="7c62f-158">Exemplo 1: Criar um chat um para um</span><span class="sxs-lookup"><span data-stu-id="7c62f-158">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="7c62f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c62f-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7c62f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c62f-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "oneOnOne",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="7c62f-161">C#</span><span class="sxs-lookup"><span data-stu-id="7c62f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chat-oneonone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c62f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c62f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chat-oneonone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c62f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c62f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chat-oneonone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c62f-164">Java</span><span class="sxs-lookup"><span data-stu-id="7c62f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chat-oneonone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="7c62f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c62f-165">Response</span></span>
><span data-ttu-id="7c62f-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c62f-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2020-12-04T23:10:28.51Z",
    "lastUpdatedDateTime": "2020-12-04T23:10:28.51Z",
    "chatType": "oneOnOne",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="7c62f-167">Exemplo 2: Criar um chat em grupo</span><span class="sxs-lookup"><span data-stu-id="7c62f-167">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="7c62f-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c62f-168">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7c62f-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c62f-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chat_group"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "group",
  "topic": "Group chat title",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="7c62f-170">C#</span><span class="sxs-lookup"><span data-stu-id="7c62f-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chat-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c62f-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c62f-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chat-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c62f-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c62f-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chat-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c62f-173">Java</span><span class="sxs-lookup"><span data-stu-id="7c62f-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chat-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="7c62f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c62f-174">Response</span></span>
><span data-ttu-id="7c62f-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c62f-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:11:16.175Z",
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A1c5b01696d2e4a179c292bc9cf04e63b@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

### <a name="example-3-create-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="7c62f-176">Exemplo 3: Criar um chat um-a-um com aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="7c62f-176">Example 3: Create a one-on-one chat with installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="7c62f-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c62f-177">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7c62f-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c62f-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne_with_installed_apps"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "oneOnOne",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ],
  "installedApps": [
    {
      "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="7c62f-179">C#</span><span class="sxs-lookup"><span data-stu-id="7c62f-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chat-oneonone-with-installed-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c62f-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c62f-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chat-oneonone-with-installed-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c62f-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c62f-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chat-oneonone-with-installed-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c62f-182">Java</span><span class="sxs-lookup"><span data-stu-id="7c62f-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chat-oneonone-with-installed-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="7c62f-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c62f-183">Response</span></span>
><span data-ttu-id="7c62f-184">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c62f-184">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /chats('19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_bfb5bb25-3a8d-487d-9828-7875ced51a30@unq.gbl.spaces')/operations('2432b57b-0abd-43db-aa7b-16eadd115d34-861f06db-0208-4815-b67a-965df0d28b7f-10adc8a6-60db-42e2-9761-e56a7e4c7bc9')
```

<span data-ttu-id="7c62f-185">A operação assíncrona é iniciada e a resposta contém um header Location que inclui um link para o [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7c62f-185">The async operation is initiated, and the response contains a Location header which includes a link to the to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="7c62f-186">O link pode ser usado para obter o status e os detalhes da operação.</span><span class="sxs-lookup"><span data-stu-id="7c62f-186">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="7c62f-187">Para obter detalhes, consulte [Obter operação no chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span><span class="sxs-lookup"><span data-stu-id="7c62f-187">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="see-also"></a><span data-ttu-id="7c62f-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="7c62f-188">See also</span></span>
- [<span data-ttu-id="7c62f-189">Obter teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="7c62f-189">Get teamsAsyncOperation</span></span>](teamsasyncoperation-get.md)
