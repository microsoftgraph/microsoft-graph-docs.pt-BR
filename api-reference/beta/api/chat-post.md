---
title: Criar chat
description: Crie um novo objeto de chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ea5de5a32754125c5016bee536c8b8d1802a8d1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030814"
---
# <a name="create-chat"></a><span data-ttu-id="b99e5-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="b99e5-103">Create chat</span></span>
<span data-ttu-id="b99e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b99e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b99e5-105">Crie um novo [objeto de chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="b99e5-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b99e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b99e5-106">Permissions</span></span>
<span data-ttu-id="b99e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b99e5-109">Permission type</span></span>|<span data-ttu-id="b99e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b99e5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b99e5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b99e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b99e5-112">Chat.Create, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b99e5-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="b99e5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b99e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99e5-114">Not supported.</span></span> |
|<span data-ttu-id="b99e5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b99e5-115">Application</span></span> | <span data-ttu-id="b99e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b99e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b99e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="b99e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b99e5-118">Request headers</span></span>
|<span data-ttu-id="b99e5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b99e5-119">Name</span></span>|<span data-ttu-id="b99e5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99e5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b99e5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b99e5-121">Authorization</span></span>|<span data-ttu-id="b99e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99e5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b99e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b99e5-124">Content-Type</span></span>|<span data-ttu-id="b99e5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99e5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99e5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b99e5-127">Request body</span></span>
<span data-ttu-id="b99e5-128">No corpo da solicitação, fornece uma representação JSON do [objeto chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="b99e5-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="b99e5-129">A tabela a seguir lista as propriedades necessárias para criar um objeto de chat.</span><span class="sxs-lookup"><span data-stu-id="b99e5-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="b99e5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b99e5-130">Property</span></span>|<span data-ttu-id="b99e5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b99e5-131">Type</span></span>|<span data-ttu-id="b99e5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99e5-133">topic</span><span class="sxs-lookup"><span data-stu-id="b99e5-133">topic</span></span>|<span data-ttu-id="b99e5-134">(Opcional) Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b99e5-134">(Optional) String</span></span>|<span data-ttu-id="b99e5-135">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="b99e5-135">The title of the chat.</span></span> <span data-ttu-id="b99e5-136">O título do chat só poderá ser fornecido se o chat for do `group` tipo.</span><span class="sxs-lookup"><span data-stu-id="b99e5-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="b99e5-137">chatType</span><span class="sxs-lookup"><span data-stu-id="b99e5-137">chatType</span></span>|[<span data-ttu-id="b99e5-138">chatType</span><span class="sxs-lookup"><span data-stu-id="b99e5-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="b99e5-139">Especifica o tipo de chat.</span><span class="sxs-lookup"><span data-stu-id="b99e5-139">Specifies the type of chat.</span></span> <span data-ttu-id="b99e5-140">Os valores possíveis são: `group` e `oneOnOne` .</span><span class="sxs-lookup"><span data-stu-id="b99e5-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="b99e5-141">membros</span><span class="sxs-lookup"><span data-stu-id="b99e5-141">members</span></span>|<span data-ttu-id="b99e5-142">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b99e5-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="b99e5-143">Lista de membros da conversa que devem ser adicionados.</span><span class="sxs-lookup"><span data-stu-id="b99e5-143">List of conversation members that should be added.</span></span> <span data-ttu-id="b99e5-144">Todos os usuários, incluindo o usuário que inicia a solicitação de criação, que participarão do chat devem ser especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="b99e5-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|
|<span data-ttu-id="b99e5-145">installedApps</span><span class="sxs-lookup"><span data-stu-id="b99e5-145">installedApps</span></span>| <span data-ttu-id="b99e5-146">Coleção [teamsApp](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="b99e5-146">[teamsApp](../resources/teamsapp.md) collection</span></span>|<span data-ttu-id="b99e5-147">Lista de aplicativos que devem ser instalados no chat.</span><span class="sxs-lookup"><span data-stu-id="b99e5-147">List of apps that should be installed in the chat.</span></span>|

> <span data-ttu-id="b99e5-148">**Observação:** Atualmente, há suporte para apenas uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b99e5-148">**Note:** Currently, only one app installation is supported.</span></span> <span data-ttu-id="b99e5-149">Se várias instalações de aplicativos estão listadas na solicitação, a resposta será um `Bad Request` erro.</span><span class="sxs-lookup"><span data-stu-id="b99e5-149">If multiple app installations are listed in the request, the response will be a `Bad Request` error.</span></span>

## <a name="response"></a><span data-ttu-id="b99e5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99e5-150">Response</span></span>

### <a name="response-for-creating-a-one-on-one-chat-without-installed-apps"></a><span data-ttu-id="b99e5-151">Resposta para criar um chat um-a-um sem aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="b99e5-151">Response for creating a one-on-one chat without installed apps</span></span>
<span data-ttu-id="b99e5-152">Se tiver êxito, este método retornará um código `201 Created` de resposta e o recurso de [chat](../resources/chat.md) recém-criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99e5-152">If successful, this method returns a `201 Created` response code and the newly created [chat](../resources/chat.md) resource in the response body.</span></span>

### <a name="response-for-creating-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="b99e5-153">Resposta para criar um chat um-a-um com aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="b99e5-153">Response for creating a one-on-one chat with installed apps</span></span>
<span data-ttu-id="b99e5-154">Se tiver êxito, este método retornará um código de resposta e um header location que contém um `202 Accepted` link para [o teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b99e5-154">If successful, this method returns a `202 Accepted` response code and Location header that contains a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="b99e5-155">O link pode ser usado para obter o status e os detalhes da operação.</span><span class="sxs-lookup"><span data-stu-id="b99e5-155">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="b99e5-156">Para obter detalhes, consulte [Obter operação no chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span><span class="sxs-lookup"><span data-stu-id="b99e5-156">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="examples"></a><span data-ttu-id="b99e5-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b99e5-157">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="b99e5-158">Exemplo 1: Criar um chat um para um</span><span class="sxs-lookup"><span data-stu-id="b99e5-158">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="b99e5-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99e5-159">Request</span></span>
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

---

#### <a name="response"></a><span data-ttu-id="b99e5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99e5-160">Response</span></span>
><span data-ttu-id="b99e5-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b99e5-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="b99e5-162">Exemplo 2: Criar um chat em grupo</span><span class="sxs-lookup"><span data-stu-id="b99e5-162">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="b99e5-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99e5-163">Request</span></span>
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

---

#### <a name="response"></a><span data-ttu-id="b99e5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99e5-164">Response</span></span>
><span data-ttu-id="b99e5-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b99e5-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-create-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="b99e5-166">Exemplo 3: Criar um chat um-a-um com aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="b99e5-166">Example 3: Create a one-on-one chat with installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="b99e5-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99e5-167">Request</span></span>
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

---

#### <a name="response"></a><span data-ttu-id="b99e5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99e5-168">Response</span></span>
><span data-ttu-id="b99e5-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b99e5-169">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /chats('19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_bfb5bb25-3a8d-487d-9828-7875ced51a30@unq.gbl.spaces')/operations('2432b57b-0abd-43db-aa7b-16eadd115d34-861f06db-0208-4815-b67a-965df0d28b7f-10adc8a6-60db-42e2-9761-e56a7e4c7bc9')
```

<span data-ttu-id="b99e5-170">A operação assíncrona é iniciada e a resposta contém um header Location que inclui um link para o [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b99e5-170">The async operation is initiated, and the response contains a Location header which includes a link to the to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="b99e5-171">O link pode ser usado para obter o status e os detalhes da operação.</span><span class="sxs-lookup"><span data-stu-id="b99e5-171">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="b99e5-172">Para obter detalhes, consulte [Obter operação no chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span><span class="sxs-lookup"><span data-stu-id="b99e5-172">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="see-also"></a><span data-ttu-id="b99e5-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="b99e5-173">See also</span></span>
- [<span data-ttu-id="b99e5-174">Obter teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="b99e5-174">Get teamsAsyncOperation</span></span>](teamsasyncoperation-get.md)
