---
title: Criar chat
description: Crie um novo objeto de chat.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b187624d00a4f51255e767761d4a3c2c675d83db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776127"
---
# <a name="create-chat"></a><span data-ttu-id="6e58a-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="6e58a-103">Create chat</span></span>
<span data-ttu-id="6e58a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e58a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e58a-105">Crie um novo [objeto de chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="6e58a-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e58a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e58a-106">Permissions</span></span>
<span data-ttu-id="6e58a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e58a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e58a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e58a-109">Permission type</span></span>|<span data-ttu-id="6e58a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e58a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e58a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e58a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e58a-112">Chat.Create, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e58a-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="6e58a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e58a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e58a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e58a-114">Not supported.</span></span> |
|<span data-ttu-id="6e58a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e58a-115">Application</span></span> | <span data-ttu-id="6e58a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e58a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e58a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e58a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="6e58a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e58a-118">Request headers</span></span>
|<span data-ttu-id="6e58a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6e58a-119">Name</span></span>|<span data-ttu-id="6e58a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e58a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e58a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e58a-121">Authorization</span></span>|<span data-ttu-id="6e58a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e58a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e58a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e58a-124">Content-Type</span></span>|<span data-ttu-id="6e58a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e58a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e58a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e58a-127">Request body</span></span>
<span data-ttu-id="6e58a-128">No corpo da solicitação, fornece uma representação JSON do [objeto chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="6e58a-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="6e58a-129">A tabela a seguir lista as propriedades necessárias para criar um objeto de chat.</span><span class="sxs-lookup"><span data-stu-id="6e58a-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="6e58a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e58a-130">Property</span></span>|<span data-ttu-id="6e58a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e58a-131">Type</span></span>|<span data-ttu-id="6e58a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e58a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e58a-133">topic</span><span class="sxs-lookup"><span data-stu-id="6e58a-133">topic</span></span>|<span data-ttu-id="6e58a-134">(Opcional) Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e58a-134">(Optional) String</span></span>|<span data-ttu-id="6e58a-135">O título do chat.</span><span class="sxs-lookup"><span data-stu-id="6e58a-135">The title of the chat.</span></span> <span data-ttu-id="6e58a-136">O título do chat só poderá ser fornecido se o chat for do `group` tipo.</span><span class="sxs-lookup"><span data-stu-id="6e58a-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="6e58a-137">chatType</span><span class="sxs-lookup"><span data-stu-id="6e58a-137">chatType</span></span>|[<span data-ttu-id="6e58a-138">chatType</span><span class="sxs-lookup"><span data-stu-id="6e58a-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="6e58a-139">Especifica o tipo de chat.</span><span class="sxs-lookup"><span data-stu-id="6e58a-139">Specifies the type of chat.</span></span> <span data-ttu-id="6e58a-140">Os valores possíveis são: `group` e `oneOnOne` .</span><span class="sxs-lookup"><span data-stu-id="6e58a-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="6e58a-141">membros</span><span class="sxs-lookup"><span data-stu-id="6e58a-141">members</span></span>|<span data-ttu-id="6e58a-142">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6e58a-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="6e58a-143">Lista de membros da conversa que devem ser adicionados.</span><span class="sxs-lookup"><span data-stu-id="6e58a-143">List of conversation members that should be added.</span></span> <span data-ttu-id="6e58a-144">Todos os usuários, incluindo o usuário que inicia a solicitação de criação, que participarão do chat devem ser especificados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="6e58a-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|

## <a name="response"></a><span data-ttu-id="6e58a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e58a-145">Response</span></span>

<span data-ttu-id="6e58a-146">Se tiver êxito, este método retornará um código de resposta Criado 201 e o recurso de **chat** recém-criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e58a-146">If successful, this method returns a 201 Created response code and the newly created **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e58a-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6e58a-147">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="6e58a-148">Exemplo 1: Criar um chat um para um</span><span class="sxs-lookup"><span data-stu-id="6e58a-148">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="6e58a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e58a-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats
Content-Type: application/json

{
  "chatType": "oneOnOne",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/v1.0/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ]
}
```


#### <a name="response"></a><span data-ttu-id="6e58a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e58a-150">Response</span></span>
><span data-ttu-id="6e58a-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e58a-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
    "id": "19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2020-12-04T23:10:28.51Z",
    "lastUpdatedDateTime": "2020-12-04T23:10:28.51Z",
    "chatType": "oneOnOne"
}
```

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="6e58a-152">Exemplo 2: Criar um chat em grupo</span><span class="sxs-lookup"><span data-stu-id="6e58a-152">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="6e58a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e58a-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chat_group"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats
Content-Type: application/json

{
  "chatType": "group",
  "topic": "Group chat title",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/v1.0/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/v1.0/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
    }
  ]
}
```


#### <a name="response"></a><span data-ttu-id="6e58a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e58a-154">Response</span></span>
><span data-ttu-id="6e58a-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e58a-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:11:16.175Z",
    "chatType": "group"
}
```

