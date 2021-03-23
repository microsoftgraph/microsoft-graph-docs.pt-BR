---
<span data-ttu-id="6c7bf-101">título: descrição "Criar assinatura": "Assina um aplicativo ouvinte para receber notificações de alteração quando os dados no Microsoft Graph são alterados".</span><span class="sxs-lookup"><span data-stu-id="6c7bf-101">title: "Create subscription" description: "Subscribes a listener application to receive change notifications when data on the Microsoft Graph changes."</span></span>
<span data-ttu-id="6c7bf-102">localization_priority: Autor de prioridade: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span><span class="sxs-lookup"><span data-stu-id="6c7bf-102">localization_priority: Priority author: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span></span>
---

# <a name="create-subscription"></a><span data-ttu-id="6c7bf-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="6c7bf-103">Create subscription</span></span>

<span data-ttu-id="6c7bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c7bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c7bf-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="6c7bf-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c7bf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c7bf-107">Permissions</span></span>

<span data-ttu-id="6c7bf-108">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="6c7bf-109">Por exemplo, para receber notificações de alterações por mensagens, seu aplicativo precisa da permissão`Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="6c7bf-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6c7bf-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c7bf-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-112">Supported resource</span></span> | <span data-ttu-id="6c7bf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6c7bf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c7bf-115">Application</span><span class="sxs-lookup"><span data-stu-id="6c7bf-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="6c7bf-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="6c7bf-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="6c7bf-117">Not supported</span></span> | <span data-ttu-id="6c7bf-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="6c7bf-118">Not supported</span></span> | <span data-ttu-id="6c7bf-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6c7bf-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6c7bf-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="6c7bf-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-122">Not supported</span></span> |  <span data-ttu-id="6c7bf-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6c7bf-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6c7bf-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-125">Not supported</span></span> | <span data-ttu-id="6c7bf-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-126">Not supported</span></span> | <span data-ttu-id="6c7bf-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6c7bf-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6c7bf-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-129">Not supported</span></span> | <span data-ttu-id="6c7bf-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-130">Not supported</span></span> | <span data-ttu-id="6c7bf-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="6c7bf-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6c7bf-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-133">Not supported</span></span> | <span data-ttu-id="6c7bf-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-134">Not supported</span></span> | <span data-ttu-id="6c7bf-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6c7bf-136">contato</span><span class="sxs-lookup"><span data-stu-id="6c7bf-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6c7bf-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-137">Contacts.Read</span></span> | <span data-ttu-id="6c7bf-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-138">Contacts.Read</span></span> | <span data-ttu-id="6c7bf-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-139">Contacts.Read</span></span> |
|<span data-ttu-id="6c7bf-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6c7bf-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-141">Not supported</span></span> | <span data-ttu-id="6c7bf-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c7bf-142">Files.ReadWrite</span></span> | <span data-ttu-id="6c7bf-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-143">Not supported</span></span> |
|<span data-ttu-id="6c7bf-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6c7bf-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6c7bf-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="6c7bf-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-146">Not supported</span></span> | <span data-ttu-id="6c7bf-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c7bf-148">evento</span><span class="sxs-lookup"><span data-stu-id="6c7bf-148">event</span></span>](../resources/event.md) | <span data-ttu-id="6c7bf-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-149">Calendars.Read</span></span> | <span data-ttu-id="6c7bf-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-150">Calendars.Read</span></span> | <span data-ttu-id="6c7bf-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-151">Calendars.Read</span></span> |
|[<span data-ttu-id="6c7bf-152">grupo</span><span class="sxs-lookup"><span data-stu-id="6c7bf-152">group</span></span>](../resources/group.md) | <span data-ttu-id="6c7bf-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-153">Group.Read.All</span></span> | <span data-ttu-id="6c7bf-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-154">Not supported</span></span> | <span data-ttu-id="6c7bf-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-155">Group.Read.All</span></span> |
|[<span data-ttu-id="6c7bf-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="6c7bf-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6c7bf-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-157">Group.Read.All</span></span> | <span data-ttu-id="6c7bf-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-158">Not supported</span></span> | <span data-ttu-id="6c7bf-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-159">Not supported</span></span> |
|[<span data-ttu-id="6c7bf-160">list</span><span class="sxs-lookup"><span data-stu-id="6c7bf-160">list</span></span>](../resources/list.md) | <span data-ttu-id="6c7bf-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6c7bf-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-162">Not supported</span></span> | <span data-ttu-id="6c7bf-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c7bf-164">message</span><span class="sxs-lookup"><span data-stu-id="6c7bf-164">message</span></span>](../resources/message.md) | <span data-ttu-id="6c7bf-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6c7bf-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6c7bf-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c7bf-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6c7bf-168">impressora</span><span class="sxs-lookup"><span data-stu-id="6c7bf-168">printer</span></span>](../resources/printer.md) | <span data-ttu-id="6c7bf-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-169">Not supported</span></span> | <span data-ttu-id="6c7bf-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-170">Not supported</span></span> | <span data-ttu-id="6c7bf-171">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-171">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c7bf-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6c7bf-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="6c7bf-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-173">Not supported</span></span> | <span data-ttu-id="6c7bf-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-174">Not supported</span></span> | <span data-ttu-id="6c7bf-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c7bf-176">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="6c7bf-176">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6c7bf-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6c7bf-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6c7bf-178">Not supported</span></span> | <span data-ttu-id="6c7bf-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c7bf-180">Usuário</span><span class="sxs-lookup"><span data-stu-id="6c7bf-180">user</span></span>](../resources/user.md) | <span data-ttu-id="6c7bf-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-181">User.Read.All</span></span> | <span data-ttu-id="6c7bf-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-182">User.Read.All</span></span> | <span data-ttu-id="6c7bf-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c7bf-183">User.Read.All</span></span> |

> <span data-ttu-id="6c7bf-184">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-184">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6c7bf-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c7bf-185">driveItem</span></span>

<span data-ttu-id="6c7bf-186">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6c7bf-187">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6c7bf-188">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6c7bf-189">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6c7bf-190">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6c7bf-191">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6c7bf-192">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="6c7bf-192">contact, event, and message</span></span>

<span data-ttu-id="6c7bf-193">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6c7bf-194">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6c7bf-195">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6c7bf-196">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6c7bf-197">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="6c7bf-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6c7bf-198">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6c7bf-199">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c7bf-200">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7bf-200">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="6c7bf-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7bf-201">Request headers</span></span>

| <span data-ttu-id="6c7bf-202">Nome</span><span class="sxs-lookup"><span data-stu-id="6c7bf-202">Name</span></span>       | <span data-ttu-id="6c7bf-203">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c7bf-203">Type</span></span> | <span data-ttu-id="6c7bf-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c7bf-204">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c7bf-205">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c7bf-205">Authorization</span></span>  | <span data-ttu-id="6c7bf-206">string</span><span class="sxs-lookup"><span data-stu-id="6c7bf-206">string</span></span>  | <span data-ttu-id="6c7bf-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6c7bf-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7bf-209">Response</span></span>

<span data-ttu-id="6c7bf-210">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-210">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="6c7bf-211">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="6c7bf-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6c7bf-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c7bf-212">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6c7bf-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7bf-213">Request</span></span>

<span data-ttu-id="6c7bf-214">Veja a seguir um exemplo da solicitação de envio de uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-214">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c7bf-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7bf-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="6c7bf-216">C#</span><span class="sxs-lookup"><span data-stu-id="6c7bf-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c7bf-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c7bf-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c7bf-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c7bf-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c7bf-219">Java</span><span class="sxs-lookup"><span data-stu-id="6c7bf-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6c7bf-220">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-220">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="6c7bf-221">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-221">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="6c7bf-222">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="6c7bf-222">Resources examples</span></span>

<span data-ttu-id="6c7bf-223">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="6c7bf-223">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="6c7bf-224">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="6c7bf-224">Resource type</span></span> | <span data-ttu-id="6c7bf-225">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c7bf-225">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="6c7bf-226">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="6c7bf-226">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="6c7bf-227">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="6c7bf-227">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6c7bf-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="6c7bf-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="6c7bf-229">Contatos</span><span class="sxs-lookup"><span data-stu-id="6c7bf-229">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="6c7bf-230">Conversas</span><span class="sxs-lookup"><span data-stu-id="6c7bf-230">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="6c7bf-231">Unidades</span><span class="sxs-lookup"><span data-stu-id="6c7bf-231">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="6c7bf-232">Eventos</span><span class="sxs-lookup"><span data-stu-id="6c7bf-232">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="6c7bf-233">Grupos</span><span class="sxs-lookup"><span data-stu-id="6c7bf-233">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="6c7bf-234">Lista</span><span class="sxs-lookup"><span data-stu-id="6c7bf-234">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="6c7bf-235">Email</span><span class="sxs-lookup"><span data-stu-id="6c7bf-235">Mail</span></span>](../resources/message.md)|<span data-ttu-id="6c7bf-236">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="6c7bf-236">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="6c7bf-237">impressora</span><span class="sxs-lookup"><span data-stu-id="6c7bf-237">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="6c7bf-238">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6c7bf-238">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="6c7bf-239">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="6c7bf-239">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|
|[<span data-ttu-id="6c7bf-240">Usuários</span><span class="sxs-lookup"><span data-stu-id="6c7bf-240">Users</span></span>](../resources/user.md)|`users`|

> <span data-ttu-id="6c7bf-241">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-241">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="6c7bf-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7bf-242">Response</span></span>

<span data-ttu-id="6c7bf-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="6c7bf-246">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="6c7bf-246">Notification endpoint validation</span></span>

<span data-ttu-id="6c7bf-247">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="6c7bf-247">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="6c7bf-248">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="6c7bf-248">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

