---
title: tipo de recurso mailFolder
description: Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9918e611c767cb791908d16307c91fd3483c4e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965593"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="e99d7-104">tipo de recurso mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-104">mailFolder resource type</span></span>

<span data-ttu-id="e99d7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e99d7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e99d7-106">Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="e99d7-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="e99d7-107">As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.</span><span class="sxs-lookup"><span data-stu-id="e99d7-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="e99d7-108">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="e99d7-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="e99d7-109">**Nomes de pasta conhecidos**</span><span class="sxs-lookup"><span data-stu-id="e99d7-109">**Well-known folder names**</span></span>

<span data-ttu-id="e99d7-110">O Outlook cria determinadas pastas para usuários por padrão.</span><span class="sxs-lookup"><span data-stu-id="e99d7-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="e99d7-111">Em vez de usar a pasta correspondente com valor **id** para sua conveniência, você pode usar os nomes das pastas conhecidas na tabela abaixo ao acessar essas pastas.</span><span class="sxs-lookup"><span data-stu-id="e99d7-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="e99d7-112">Por exemplo, você encontra a pasta de Rascunhos usando seu nome reconhecido com a seguinte consulta.</span><span class="sxs-lookup"><span data-stu-id="e99d7-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="e99d7-113">Nomes conhecidos funcionam independentemente da localidade da caixa de correio do usuário, então a consulta acima sempre retornará a pasta de Rascunhos do usuário independentemente de como será nomeada.</span><span class="sxs-lookup"><span data-stu-id="e99d7-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="e99d7-114">Nome da pasta conhecida</span><span class="sxs-lookup"><span data-stu-id="e99d7-114">Well-known folder name</span></span> | <span data-ttu-id="e99d7-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99d7-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="e99d7-116">arquivar</span><span class="sxs-lookup"><span data-stu-id="e99d7-116">archive</span></span> | <span data-ttu-id="e99d7-117">As mensagens da pasta arquivo morto são enviadas ao usar o recurso arquivar One_Click em clientes do Outlook que são compatíveis com ele.</span><span class="sxs-lookup"><span data-stu-id="e99d7-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="e99d7-118">**Observação:** esse não é o mesmo recurso de Caixa de Correio de Arquivamento do Exchange online.</span><span class="sxs-lookup"><span data-stu-id="e99d7-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="e99d7-119">Email secundário</span><span class="sxs-lookup"><span data-stu-id="e99d7-119">clutter</span></span> | <span data-ttu-id="e99d7-120">As mensagens de baixa prioridade da pasta de email secundário são movidas ao usar o recurso email secundário.</span><span class="sxs-lookup"><span data-stu-id="e99d7-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="e99d7-121">Conflitos</span><span class="sxs-lookup"><span data-stu-id="e99d7-121">conflicts</span></span> | <span data-ttu-id="e99d7-122">A pasta que contém itens conflitantes na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e99d7-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="e99d7-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="e99d7-123">conversationhistory</span></span> | <span data-ttu-id="e99d7-124">A pasta em que o Skype salva conversas de mensagens Instantâneas (se o Skype está configurado para fazer isso).</span><span class="sxs-lookup"><span data-stu-id="e99d7-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="e99d7-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="e99d7-125">deleteditems</span></span> | <span data-ttu-id="e99d7-126">Os itens da pasta são movidos quando são excluídas.</span><span class="sxs-lookup"><span data-stu-id="e99d7-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="e99d7-127">rascunhos</span><span class="sxs-lookup"><span data-stu-id="e99d7-127">drafts</span></span> | <span data-ttu-id="e99d7-128">A pasta que contém as mensagens não enviadas.</span><span class="sxs-lookup"><span data-stu-id="e99d7-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="e99d7-129">caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="e99d7-129">inbox</span></span> | <span data-ttu-id="e99d7-130">A pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="e99d7-130">The inbox folder.</span></span> |
| <span data-ttu-id="e99d7-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="e99d7-131">junkemail</span></span> | <span data-ttu-id="e99d7-132">A pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="e99d7-132">The junk email folder.</span></span> |
| <span data-ttu-id="e99d7-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="e99d7-133">localfailures</span></span> | <span data-ttu-id="e99d7-134">A pasta que contém itens que existem no cliente local, mas não podem ser carregados para o servidor.</span><span class="sxs-lookup"><span data-stu-id="e99d7-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="e99d7-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="e99d7-135">msgfolderroot</span></span> | <span data-ttu-id="e99d7-136">A pasta "Superior do repositório de informações".</span><span class="sxs-lookup"><span data-stu-id="e99d7-136">The "Top of Information Store" folder.</span></span> <span data-ttu-id="e99d7-137">Esta pasta é a pasta pai das pastas que são exibidas em clientes de email normais, como a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="e99d7-137">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="e99d7-138">Caixa de saída</span><span class="sxs-lookup"><span data-stu-id="e99d7-138">outbox</span></span> | <span data-ttu-id="e99d7-139">A pasta caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="e99d7-139">The outbox folder.</span></span> |
| <span data-ttu-id="e99d7-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="e99d7-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="e99d7-141">A pasta que contém itens excluídos de modo reversível: excluído da pasta Itens excluídos ou ao pressionar shift + delete no Outlook.</span><span class="sxs-lookup"><span data-stu-id="e99d7-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="e99d7-142">Esta pasta não está visível em qualquer cliente de email do Outlook, mas os usuários finais podem interagir com ela pelo recurso **Recuperar itens excluídos do servidor** no Outlook ou no Outlook na web.</span><span class="sxs-lookup"><span data-stu-id="e99d7-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="e99d7-143">agendado</span><span class="sxs-lookup"><span data-stu-id="e99d7-143">scheduled</span></span> | <span data-ttu-id="e99d7-144">A pasta que contém mensagens que estão agendadas para serem exibidas na caixa de entrada usando o recurso de cronograma do Outlook para iOS.</span><span class="sxs-lookup"><span data-stu-id="e99d7-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="e99d7-145">SearchFolders</span><span class="sxs-lookup"><span data-stu-id="e99d7-145">searchfolders</span></span> | <span data-ttu-id="e99d7-146">A pasta pai para todas as pastas de pesquisa definida na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e99d7-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="e99d7-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="e99d7-147">sentitems</span></span> | <span data-ttu-id="e99d7-148">A pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="e99d7-148">The sent items folder.</span></span> |
| <span data-ttu-id="e99d7-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="e99d7-149">serverfailures</span></span> | <span data-ttu-id="e99d7-150">A pasta que contém itens que existem no servidor, mas não podem ser sincronizados para o cliente local.</span><span class="sxs-lookup"><span data-stu-id="e99d7-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="e99d7-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="e99d7-151">syncissues</span></span> | <span data-ttu-id="e99d7-152">A pasta que contém os logs de sincronização criados pelo Outlook.</span><span class="sxs-lookup"><span data-stu-id="e99d7-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="e99d7-153">Métodos</span><span class="sxs-lookup"><span data-stu-id="e99d7-153">Methods</span></span>

| <span data-ttu-id="e99d7-154">Método</span><span class="sxs-lookup"><span data-stu-id="e99d7-154">Method</span></span> | <span data-ttu-id="e99d7-155">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e99d7-155">Return Type</span></span> | <span data-ttu-id="e99d7-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99d7-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="e99d7-157">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-157">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="e99d7-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-158">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="e99d7-159">Leia as propriedades e os relacionamentos do objeto mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-159">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="e99d7-160">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-160">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="e99d7-161">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-161">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="e99d7-162">Crie uma nova mailFolder na atual postando na coleção childFolders.</span><span class="sxs-lookup"><span data-stu-id="e99d7-162">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="e99d7-163">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="e99d7-163">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="e99d7-164">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-164">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="e99d7-p107">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="e99d7-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="e99d7-167">Criar Mensagem</span><span class="sxs-lookup"><span data-stu-id="e99d7-167">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="e99d7-168">Mensagem</span><span class="sxs-lookup"><span data-stu-id="e99d7-168">Message</span></span>](message.md)| <span data-ttu-id="e99d7-169">Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="e99d7-169">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="e99d7-170">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="e99d7-170">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="e99d7-171">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-171">[Message](message.md) collection</span></span>| <span data-ttu-id="e99d7-172">Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e99d7-172">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="e99d7-173">Update</span><span class="sxs-lookup"><span data-stu-id="e99d7-173">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="e99d7-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-174">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e99d7-175">Atualize o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="e99d7-175">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="e99d7-176">Delete</span><span class="sxs-lookup"><span data-stu-id="e99d7-176">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="e99d7-177">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e99d7-177">None</span></span> |<span data-ttu-id="e99d7-178">Exclua o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="e99d7-178">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="e99d7-179">copy</span><span class="sxs-lookup"><span data-stu-id="e99d7-179">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="e99d7-180">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-180">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e99d7-181">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-181">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="e99d7-182">delta</span><span class="sxs-lookup"><span data-stu-id="e99d7-182">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="e99d7-183">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-183">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="e99d7-184">Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e99d7-184">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="e99d7-185">move</span><span class="sxs-lookup"><span data-stu-id="e99d7-185">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="e99d7-186">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-186">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e99d7-187">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-187">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="e99d7-188">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="e99d7-188">**Extended properties**</span></span>| | |
|[<span data-ttu-id="e99d7-189">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="e99d7-189">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e99d7-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-190">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="e99d7-191">Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="e99d7-191">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="e99d7-192">Obter mailFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="e99d7-192">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e99d7-193">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-193">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="e99d7-194">Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e99d7-194">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e99d7-195">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="e99d7-195">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e99d7-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-196">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="e99d7-197">Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="e99d7-197">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="e99d7-198">Obter mailFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="e99d7-198">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e99d7-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e99d7-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="e99d7-200">Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="e99d7-200">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e99d7-201">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e99d7-201">Properties</span></span>

| <span data-ttu-id="e99d7-202">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e99d7-202">Property</span></span> | <span data-ttu-id="e99d7-203">Tipo</span><span class="sxs-lookup"><span data-stu-id="e99d7-203">Type</span></span> | <span data-ttu-id="e99d7-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99d7-204">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="e99d7-205">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="e99d7-205">childFolderCount</span></span>|<span data-ttu-id="e99d7-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e99d7-206">Int32</span></span>|<span data-ttu-id="e99d7-207">O número de mailFolders filho imediatas na mailFolder atual.</span><span class="sxs-lookup"><span data-stu-id="e99d7-207">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="e99d7-208">displayName</span><span class="sxs-lookup"><span data-stu-id="e99d7-208">displayName</span></span>|<span data-ttu-id="e99d7-209">String</span><span class="sxs-lookup"><span data-stu-id="e99d7-209">String</span></span>|<span data-ttu-id="e99d7-210">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-210">The mailFolder's display name.</span></span>|
|<span data-ttu-id="e99d7-211">id</span><span class="sxs-lookup"><span data-stu-id="e99d7-211">id</span></span>|<span data-ttu-id="e99d7-212">String</span><span class="sxs-lookup"><span data-stu-id="e99d7-212">String</span></span>|<span data-ttu-id="e99d7-213">Identificador exclusivo de mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-213">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="e99d7-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e99d7-214">parentFolderId</span></span>|<span data-ttu-id="e99d7-215">String</span><span class="sxs-lookup"><span data-stu-id="e99d7-215">String</span></span>|<span data-ttu-id="e99d7-216">O identificador exclusivo de mailFolder do mailFolder pai.</span><span class="sxs-lookup"><span data-stu-id="e99d7-216">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="e99d7-217">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="e99d7-217">totalItemCount</span></span>|<span data-ttu-id="e99d7-218">Int32</span><span class="sxs-lookup"><span data-stu-id="e99d7-218">Int32</span></span>|<span data-ttu-id="e99d7-219">O número de itens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-219">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="e99d7-220">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="e99d7-220">unreadItemCount</span></span>|<span data-ttu-id="e99d7-221">Int32</span><span class="sxs-lookup"><span data-stu-id="e99d7-221">Int32</span></span>|<span data-ttu-id="e99d7-222">O número de itens na mailFolder marcados como não lidos.</span><span class="sxs-lookup"><span data-stu-id="e99d7-222">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="e99d7-223">**Acessar contagens de itens de forma eficiente**</span><span class="sxs-lookup"><span data-stu-id="e99d7-223">**Access item counts efficiently**</span></span>

<span data-ttu-id="e99d7-224">As propriedades `TotalItemCount` e `UnreadItemCount` de uma pasta permitem convenientemente calcular o número de itens de leitura na pasta.</span><span class="sxs-lookup"><span data-stu-id="e99d7-224">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="e99d7-225">Eles permitem que você evite consultas semelhante à seguinte, que podem causar latência significativa:</span><span class="sxs-lookup"><span data-stu-id="e99d7-225">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="e99d7-226">As pastas de email no Outlook podem conter mais de um tipo de item, por exemplo, a caixa de entrada pode conter itens que são diferentes de itens de email da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e99d7-226">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="e99d7-227">`TotalItemCount` e `UnreadItemCount` incluem itens em uma pasta de email independentemente seus tipos de item.</span><span class="sxs-lookup"><span data-stu-id="e99d7-227">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="e99d7-228">Relações</span><span class="sxs-lookup"><span data-stu-id="e99d7-228">Relationships</span></span>

| <span data-ttu-id="e99d7-229">Relação</span><span class="sxs-lookup"><span data-stu-id="e99d7-229">Relationship</span></span> | <span data-ttu-id="e99d7-230">Tipo</span><span class="sxs-lookup"><span data-stu-id="e99d7-230">Type</span></span> | <span data-ttu-id="e99d7-231">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99d7-231">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="e99d7-232">childFolders</span><span class="sxs-lookup"><span data-stu-id="e99d7-232">childFolders</span></span>|<span data-ttu-id="e99d7-233">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-233">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="e99d7-234">A coleção de pastas filho na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-234">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="e99d7-235">messageRules</span><span class="sxs-lookup"><span data-stu-id="e99d7-235">messageRules</span></span> | <span data-ttu-id="e99d7-236">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-236">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="e99d7-237">A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="e99d7-237">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="e99d7-238">mensagens</span><span class="sxs-lookup"><span data-stu-id="e99d7-238">messages</span></span>|<span data-ttu-id="e99d7-239">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-239">[Message](message.md) collection</span></span>|<span data-ttu-id="e99d7-240">A coleção de mensagens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e99d7-240">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="e99d7-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e99d7-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="e99d7-242">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e99d7-p110">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e99d7-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e99d7-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e99d7-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="e99d7-247">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e99d7-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e99d7-p111">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e99d7-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e99d7-251">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e99d7-251">JSON representation</span></span>

<span data-ttu-id="e99d7-252">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e99d7-252">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="e99d7-253">Confira também</span><span class="sxs-lookup"><span data-stu-id="e99d7-253">See also</span></span>

- [<span data-ttu-id="e99d7-254">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e99d7-254">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="e99d7-255">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="e99d7-255">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

