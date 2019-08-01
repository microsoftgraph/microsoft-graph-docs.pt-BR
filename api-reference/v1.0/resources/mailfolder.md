---
title: tipo de recurso mailFolder
description: Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7e829929df46208ee321f56ae2d9f0144c320d4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036327"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="5a06b-104">tipo de recurso mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-104">mailFolder resource type</span></span>

<span data-ttu-id="5a06b-105">Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="5a06b-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="5a06b-106">As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.</span><span class="sxs-lookup"><span data-stu-id="5a06b-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="5a06b-107">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="5a06b-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="5a06b-108">**Nomes de pasta conhecidos**</span><span class="sxs-lookup"><span data-stu-id="5a06b-108">**Well-known folder names**</span></span>

<span data-ttu-id="5a06b-109">O Outlook cria determinadas pastas para usuários por padrão.</span><span class="sxs-lookup"><span data-stu-id="5a06b-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="5a06b-110">Em vez de usar a pasta correspondente com valor **id** para sua conveniência, você pode usar os nomes das pastas conhecidas na tabela abaixo ao acessar essas pastas.</span><span class="sxs-lookup"><span data-stu-id="5a06b-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="5a06b-111">Por exemplo, você encontra a pasta de Rascunhos usando seu nome reconhecido com a seguinte consulta.</span><span class="sxs-lookup"><span data-stu-id="5a06b-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="5a06b-112">Nomes conhecidos funcionam independentemente da localidade da caixa de correio do usuário, então a consulta acima sempre retornará a pasta de Rascunhos do usuário independentemente de como será nomeada.</span><span class="sxs-lookup"><span data-stu-id="5a06b-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="5a06b-113">Nome da pasta conhecida</span><span class="sxs-lookup"><span data-stu-id="5a06b-113">Well-known folder name</span></span> | <span data-ttu-id="5a06b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a06b-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="5a06b-115">arquivar</span><span class="sxs-lookup"><span data-stu-id="5a06b-115">archive</span></span> | <span data-ttu-id="5a06b-116">As mensagens da pasta arquivo morto são enviadas ao usar o recurso arquivar One_Click em clientes do Outlook que são compatíveis com ele.</span><span class="sxs-lookup"><span data-stu-id="5a06b-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="5a06b-117">**Observação:** esse não é o mesmo recurso de Caixa de Correio de Arquivamento do Exchange online.</span><span class="sxs-lookup"><span data-stu-id="5a06b-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="5a06b-118">Email secundário</span><span class="sxs-lookup"><span data-stu-id="5a06b-118">clutter</span></span> | <span data-ttu-id="5a06b-119">As mensagens de baixa prioridade da pasta de email secundário são movidas ao usar o recurso email secundário.</span><span class="sxs-lookup"><span data-stu-id="5a06b-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="5a06b-120">Conflitos</span><span class="sxs-lookup"><span data-stu-id="5a06b-120">conflicts</span></span> | <span data-ttu-id="5a06b-121">A pasta que contém itens conflitantes na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5a06b-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="5a06b-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="5a06b-122">conversationhistory</span></span> | <span data-ttu-id="5a06b-123">A pasta em que o Skype salva conversas de mensagens Instantâneas (se o Skype está configurado para fazer isso).</span><span class="sxs-lookup"><span data-stu-id="5a06b-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="5a06b-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="5a06b-124">deleteditems</span></span> | <span data-ttu-id="5a06b-125">Os itens da pasta são movidos quando são excluídas.</span><span class="sxs-lookup"><span data-stu-id="5a06b-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="5a06b-126">rascunhos</span><span class="sxs-lookup"><span data-stu-id="5a06b-126">drafts</span></span> | <span data-ttu-id="5a06b-127">A pasta que contém as mensagens não enviadas.</span><span class="sxs-lookup"><span data-stu-id="5a06b-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="5a06b-128">caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="5a06b-128">inbox</span></span> | <span data-ttu-id="5a06b-129">A pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="5a06b-129">The inbox folder.</span></span> |
| <span data-ttu-id="5a06b-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="5a06b-130">junkemail</span></span> | <span data-ttu-id="5a06b-131">A pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="5a06b-131">The junk email folder.</span></span> |
| <span data-ttu-id="5a06b-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="5a06b-132">localfailures</span></span> | <span data-ttu-id="5a06b-133">A pasta que contém itens que existem no cliente local, mas não podem ser carregados para o servidor.</span><span class="sxs-lookup"><span data-stu-id="5a06b-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="5a06b-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="5a06b-134">msgfolderroot</span></span> | <span data-ttu-id="5a06b-135">A pasta "Superior do repositório de informações".</span><span class="sxs-lookup"><span data-stu-id="5a06b-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="5a06b-136">Esta pasta é a pasta pai das pastas que são exibidas em clientes de email normais, como a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="5a06b-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="5a06b-137">Caixa de saída</span><span class="sxs-lookup"><span data-stu-id="5a06b-137">outbox</span></span> | <span data-ttu-id="5a06b-138">A pasta caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="5a06b-138">The outbox folder.</span></span> |
| <span data-ttu-id="5a06b-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="5a06b-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="5a06b-140">A pasta que contém itens excluídos de modo reversível: excluído da pasta Itens excluídos ou ao pressionar shift + delete no Outlook.</span><span class="sxs-lookup"><span data-stu-id="5a06b-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="5a06b-141">Esta pasta não está visível em qualquer cliente de email do Outlook, mas os usuários finais podem interagir com ela pelo recurso **Recuperar itens excluídos do servidor** no Outlook ou no Outlook na web.</span><span class="sxs-lookup"><span data-stu-id="5a06b-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="5a06b-142">agendado</span><span class="sxs-lookup"><span data-stu-id="5a06b-142">scheduled</span></span> | <span data-ttu-id="5a06b-143">A pasta que contém mensagens que estão agendadas para serem exibidas na caixa de entrada usando o recurso de cronograma do Outlook para iOS.</span><span class="sxs-lookup"><span data-stu-id="5a06b-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="5a06b-144">SearchFolders</span><span class="sxs-lookup"><span data-stu-id="5a06b-144">searchfolders</span></span> | <span data-ttu-id="5a06b-145">A pasta pai para todas as pastas de pesquisa definida na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5a06b-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="5a06b-146">sentitems</span><span class="sxs-lookup"><span data-stu-id="5a06b-146">sentitems</span></span> | <span data-ttu-id="5a06b-147">A pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="5a06b-147">The sent items folder.</span></span> |
| <span data-ttu-id="5a06b-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="5a06b-148">serverfailures</span></span> | <span data-ttu-id="5a06b-149">A pasta que contém itens que existem no servidor, mas não podem ser sincronizados para o cliente local.</span><span class="sxs-lookup"><span data-stu-id="5a06b-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="5a06b-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="5a06b-150">syncissues</span></span> | <span data-ttu-id="5a06b-151">A pasta que contém os logs de sincronização criados pelo Outlook.</span><span class="sxs-lookup"><span data-stu-id="5a06b-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="5a06b-152">Métodos</span><span class="sxs-lookup"><span data-stu-id="5a06b-152">Methods</span></span>

| <span data-ttu-id="5a06b-153">Método</span><span class="sxs-lookup"><span data-stu-id="5a06b-153">Method</span></span> | <span data-ttu-id="5a06b-154">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5a06b-154">Return Type</span></span> | <span data-ttu-id="5a06b-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a06b-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="5a06b-156">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="5a06b-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="5a06b-158">Leia as propriedades e os relacionamentos do objeto mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="5a06b-159">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="5a06b-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="5a06b-161">Crie uma nova mailFolder na atual postando na coleção childFolders.</span><span class="sxs-lookup"><span data-stu-id="5a06b-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="5a06b-162">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="5a06b-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="5a06b-163">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="5a06b-p107">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="5a06b-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="5a06b-166">Criar Mensagem</span><span class="sxs-lookup"><span data-stu-id="5a06b-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="5a06b-167">Mensagem</span><span class="sxs-lookup"><span data-stu-id="5a06b-167">Message</span></span>](message.md)| <span data-ttu-id="5a06b-168">Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="5a06b-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="5a06b-169">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="5a06b-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="5a06b-170">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-170">[Message](message.md) collection</span></span>| <span data-ttu-id="5a06b-171">Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5a06b-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="5a06b-172">Update</span><span class="sxs-lookup"><span data-stu-id="5a06b-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="5a06b-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="5a06b-174">Atualize o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="5a06b-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="5a06b-175">Delete</span><span class="sxs-lookup"><span data-stu-id="5a06b-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="5a06b-176">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5a06b-176">None</span></span> |<span data-ttu-id="5a06b-177">Exclua o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="5a06b-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="5a06b-178">copy</span><span class="sxs-lookup"><span data-stu-id="5a06b-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="5a06b-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="5a06b-180">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="5a06b-181">delta</span><span class="sxs-lookup"><span data-stu-id="5a06b-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="5a06b-182">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="5a06b-183">Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5a06b-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="5a06b-184">move</span><span class="sxs-lookup"><span data-stu-id="5a06b-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="5a06b-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="5a06b-186">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="5a06b-187">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="5a06b-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="5a06b-188">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="5a06b-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="5a06b-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="5a06b-190">Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="5a06b-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="5a06b-191">Obter mailFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="5a06b-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="5a06b-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="5a06b-193">Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5a06b-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="5a06b-194">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="5a06b-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="5a06b-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="5a06b-196">Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="5a06b-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="5a06b-197">Obter mailFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="5a06b-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="5a06b-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a06b-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="5a06b-199">Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="5a06b-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a06b-200">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a06b-200">Properties</span></span>

| <span data-ttu-id="5a06b-201">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a06b-201">Property</span></span> | <span data-ttu-id="5a06b-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a06b-202">Type</span></span> | <span data-ttu-id="5a06b-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a06b-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="5a06b-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="5a06b-204">childFolderCount</span></span>|<span data-ttu-id="5a06b-205">Int32</span><span class="sxs-lookup"><span data-stu-id="5a06b-205">Int32</span></span>|<span data-ttu-id="5a06b-206">O número de mailFolders filho imediatas na mailFolder atual.</span><span class="sxs-lookup"><span data-stu-id="5a06b-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="5a06b-207">displayName</span><span class="sxs-lookup"><span data-stu-id="5a06b-207">displayName</span></span>|<span data-ttu-id="5a06b-208">String</span><span class="sxs-lookup"><span data-stu-id="5a06b-208">String</span></span>|<span data-ttu-id="5a06b-209">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="5a06b-210">id</span><span class="sxs-lookup"><span data-stu-id="5a06b-210">id</span></span>|<span data-ttu-id="5a06b-211">String</span><span class="sxs-lookup"><span data-stu-id="5a06b-211">String</span></span>|<span data-ttu-id="5a06b-212">Identificador exclusivo de mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="5a06b-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="5a06b-213">parentFolderId</span></span>|<span data-ttu-id="5a06b-214">String</span><span class="sxs-lookup"><span data-stu-id="5a06b-214">String</span></span>|<span data-ttu-id="5a06b-215">O identificador exclusivo de mailFolder do mailFolder pai.</span><span class="sxs-lookup"><span data-stu-id="5a06b-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="5a06b-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="5a06b-216">totalItemCount</span></span>|<span data-ttu-id="5a06b-217">Int32</span><span class="sxs-lookup"><span data-stu-id="5a06b-217">Int32</span></span>|<span data-ttu-id="5a06b-218">O número de itens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="5a06b-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="5a06b-219">unreadItemCount</span></span>|<span data-ttu-id="5a06b-220">Int32</span><span class="sxs-lookup"><span data-stu-id="5a06b-220">Int32</span></span>|<span data-ttu-id="5a06b-221">O número de itens na mailFolder marcados como não lidos.</span><span class="sxs-lookup"><span data-stu-id="5a06b-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="5a06b-222">**Acessar contagens de itens de forma eficiente**</span><span class="sxs-lookup"><span data-stu-id="5a06b-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="5a06b-223">As propriedades `TotalItemCount` e `UnreadItemCount` de uma pasta permitem convenientemente calcular o número de itens de leitura na pasta.</span><span class="sxs-lookup"><span data-stu-id="5a06b-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="5a06b-224">Eles permitem que você evite consultas semelhante à seguinte, que podem causar latência significativa:</span><span class="sxs-lookup"><span data-stu-id="5a06b-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="5a06b-225">As pastas de email no Outlook podem conter mais de um tipo de item, por exemplo, a caixa de entrada pode conter itens que são diferentes de itens de email da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="5a06b-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="5a06b-226">`TotalItemCount` e `UnreadItemCount` incluem itens em uma pasta de email independentemente seus tipos de item.</span><span class="sxs-lookup"><span data-stu-id="5a06b-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="5a06b-227">Relações</span><span class="sxs-lookup"><span data-stu-id="5a06b-227">Relationships</span></span>

| <span data-ttu-id="5a06b-228">Relação</span><span class="sxs-lookup"><span data-stu-id="5a06b-228">Relationship</span></span> | <span data-ttu-id="5a06b-229">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a06b-229">Type</span></span> | <span data-ttu-id="5a06b-230">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a06b-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="5a06b-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="5a06b-231">childFolders</span></span>|<span data-ttu-id="5a06b-232">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="5a06b-233">A coleção de pastas filho na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="5a06b-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="5a06b-234">messageRules</span></span> | <span data-ttu-id="5a06b-235">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="5a06b-236">A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="5a06b-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="5a06b-237">mensagens</span><span class="sxs-lookup"><span data-stu-id="5a06b-237">messages</span></span>|<span data-ttu-id="5a06b-238">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-238">[Message](message.md) collection</span></span>|<span data-ttu-id="5a06b-239">A coleção de mensagens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a06b-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="5a06b-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5a06b-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="5a06b-241">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5a06b-p110">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5a06b-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="5a06b-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5a06b-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="5a06b-246">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5a06b-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5a06b-p111">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5a06b-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a06b-250">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a06b-250">JSON representation</span></span>

<span data-ttu-id="5a06b-251">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5a06b-251">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="5a06b-252">Confira também</span><span class="sxs-lookup"><span data-stu-id="5a06b-252">See also</span></span>

- [<span data-ttu-id="5a06b-253">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5a06b-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="5a06b-254">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="5a06b-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
