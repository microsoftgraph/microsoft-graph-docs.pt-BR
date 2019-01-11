---
title: tipo de recurso mailFolder
description: Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.
localization_priority: Priority
ms.openlocfilehash: 32af125f57e02394c4d01913aaf783df11809242
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888155"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="33dfc-104">tipo de recurso mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-104">mailFolder resource type</span></span>

<span data-ttu-id="33dfc-105">Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="33dfc-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="33dfc-106">As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.</span><span class="sxs-lookup"><span data-stu-id="33dfc-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="33dfc-107">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="33dfc-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="33dfc-108">**Nomes de pasta conhecido**</span><span class="sxs-lookup"><span data-stu-id="33dfc-108">**Well-known folder names**</span></span>

<span data-ttu-id="33dfc-109">O Outlook cria determinadas pastas para usuários por padrão.</span><span class="sxs-lookup"><span data-stu-id="33dfc-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="33dfc-110">Em vez de usar o valor de **id** de pasta correspondente, para sua conveniência, você pode usar os nomes de pasta conhecido da tabela abaixo ao acessar essas pastas.</span><span class="sxs-lookup"><span data-stu-id="33dfc-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="33dfc-111">Por exemplo, você pode obter a pasta Rascunhos usando seu nome conhecido com a seguinte consulta.</span><span class="sxs-lookup"><span data-stu-id="33dfc-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="33dfc-112">Nomes conhecidos funcionam independentemente da localidade da caixa de correio do usuário, portanto, a consulta acima retornará sempre na pasta Rascunhos do usuário independentemente de como ele é chamado.</span><span class="sxs-lookup"><span data-stu-id="33dfc-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="33dfc-113">Nome da pasta conhecido</span><span class="sxs-lookup"><span data-stu-id="33dfc-113">Well-known folder name</span></span> | <span data-ttu-id="33dfc-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dfc-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="33dfc-115">arquivo morto</span><span class="sxs-lookup"><span data-stu-id="33dfc-115">archive</span></span> | <span data-ttu-id="33dfc-116">As mensagens de pasta de arquivo morto são enviadas ao usar o recurso de arquivamento One_Click nos clientes do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="33dfc-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="33dfc-117">**Observação:** isso não é o mesmo que o recurso de caixa de correio de arquivamento do Exchange online.</span><span class="sxs-lookup"><span data-stu-id="33dfc-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="33dfc-118">desorganização</span><span class="sxs-lookup"><span data-stu-id="33dfc-118">clutter</span></span> | <span data-ttu-id="33dfc-119">As mensagens de baixa prioridade de pasta desorganização são movidas para ao usar o recurso desorganização.</span><span class="sxs-lookup"><span data-stu-id="33dfc-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="33dfc-120">conflitos</span><span class="sxs-lookup"><span data-stu-id="33dfc-120">conflicts</span></span> | <span data-ttu-id="33dfc-121">A pasta que contém itens conflitantes na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="33dfc-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="33dfc-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="33dfc-122">conversationhistory</span></span> | <span data-ttu-id="33dfc-123">A pasta onde o Skype salva conversas de mensagens Instantâneas (se Skype estiver configurada para fazê-lo).</span><span class="sxs-lookup"><span data-stu-id="33dfc-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="33dfc-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="33dfc-124">deleteditems</span></span> | <span data-ttu-id="33dfc-125">Os itens da pasta são movidos para quando eles são excluídos.</span><span class="sxs-lookup"><span data-stu-id="33dfc-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="33dfc-126">rascunhos</span><span class="sxs-lookup"><span data-stu-id="33dfc-126">drafts</span></span> | <span data-ttu-id="33dfc-127">A pasta que contém as mensagens não enviadas.</span><span class="sxs-lookup"><span data-stu-id="33dfc-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="33dfc-128">caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="33dfc-128">inbox</span></span> | <span data-ttu-id="33dfc-129">A pasta de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="33dfc-129">The inbox folder.</span></span> |
| <span data-ttu-id="33dfc-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="33dfc-130">junkemail</span></span> | <span data-ttu-id="33dfc-131">A pasta de lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="33dfc-131">The junk email folder.</span></span> |
| <span data-ttu-id="33dfc-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="33dfc-132">localfailures</span></span> | <span data-ttu-id="33dfc-133">A pasta que contém itens que existem no cliente local, mas não puderam ser carregados no servidor.</span><span class="sxs-lookup"><span data-stu-id="33dfc-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="33dfc-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="33dfc-134">msgfolderroot</span></span> | <span data-ttu-id="33dfc-135">A pasta "Superior do armazenamento de informações".</span><span class="sxs-lookup"><span data-stu-id="33dfc-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="33dfc-136">Essa pasta é a pasta pai para as pastas que são exibidos em clientes de email normal, como a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="33dfc-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="33dfc-137">caixa de saída</span><span class="sxs-lookup"><span data-stu-id="33dfc-137">outbox</span></span> | <span data-ttu-id="33dfc-138">A pasta caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="33dfc-138">The outbox folder.</span></span> |
| <span data-ttu-id="33dfc-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="33dfc-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="33dfc-140">A pasta que contém itens excluída: excluído da pasta Itens excluídos ou por pressionar shift + delete no Outlook.</span><span class="sxs-lookup"><span data-stu-id="33dfc-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="33dfc-141">Essa pasta não é visível em qualquer cliente de email do Outlook, mas os usuários finais podem interagir com ele por meio do recurso de **Recuperar itens excluídos do servidor** do Outlook ou do Outlook na web.</span><span class="sxs-lookup"><span data-stu-id="33dfc-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="33dfc-142">agendado</span><span class="sxs-lookup"><span data-stu-id="33dfc-142">scheduled</span></span> | <span data-ttu-id="33dfc-143">A pasta que contém as mensagens que são agendadas reaparecem na caixa de entrada usando o recurso de agendamento no Outlook para iOS.</span><span class="sxs-lookup"><span data-stu-id="33dfc-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="33dfc-144">SearchFolders</span><span class="sxs-lookup"><span data-stu-id="33dfc-144">searchfolders</span></span> | <span data-ttu-id="33dfc-145">A pasta pai para todas as pastas de pesquisa definido na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="33dfc-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="33dfc-146">itens enviados</span><span class="sxs-lookup"><span data-stu-id="33dfc-146">sentitems</span></span> | <span data-ttu-id="33dfc-147">A pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="33dfc-147">The sent items folder.</span></span> |
| <span data-ttu-id="33dfc-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="33dfc-148">serverfailures</span></span> | <span data-ttu-id="33dfc-149">A pasta que contém itens que existem no servidor, mas não pôde ser sincronizados no cliente local.</span><span class="sxs-lookup"><span data-stu-id="33dfc-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="33dfc-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="33dfc-150">syncissues</span></span> | <span data-ttu-id="33dfc-151">A pasta que contém os logs de sincronização criados pelo Outlook.</span><span class="sxs-lookup"><span data-stu-id="33dfc-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="33dfc-152">Métodos</span><span class="sxs-lookup"><span data-stu-id="33dfc-152">Methods</span></span>

| <span data-ttu-id="33dfc-153">Método</span><span class="sxs-lookup"><span data-stu-id="33dfc-153">Method</span></span> | <span data-ttu-id="33dfc-154">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33dfc-154">Return Type</span></span> | <span data-ttu-id="33dfc-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dfc-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="33dfc-156">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="33dfc-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="33dfc-158">Leia as propriedades e os relacionamentos do objeto mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="33dfc-159">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="33dfc-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="33dfc-161">Crie uma nova mailFolder na atual postando na coleção childFolders.</span><span class="sxs-lookup"><span data-stu-id="33dfc-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="33dfc-162">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="33dfc-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="33dfc-163">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="33dfc-p107">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="33dfc-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="33dfc-166">Criar Mensagem</span><span class="sxs-lookup"><span data-stu-id="33dfc-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="33dfc-167">Mensagem</span><span class="sxs-lookup"><span data-stu-id="33dfc-167">Message</span></span>](message.md)| <span data-ttu-id="33dfc-168">Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="33dfc-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="33dfc-169">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="33dfc-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="33dfc-170">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-170">[Message](message.md) collection</span></span>| <span data-ttu-id="33dfc-171">Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="33dfc-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="33dfc-172">Update</span><span class="sxs-lookup"><span data-stu-id="33dfc-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="33dfc-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="33dfc-174">Atualize o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="33dfc-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="33dfc-175">Delete</span><span class="sxs-lookup"><span data-stu-id="33dfc-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="33dfc-176">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="33dfc-176">None</span></span> |<span data-ttu-id="33dfc-177">Exclua o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="33dfc-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="33dfc-178">copy</span><span class="sxs-lookup"><span data-stu-id="33dfc-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="33dfc-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="33dfc-180">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="33dfc-181">delta</span><span class="sxs-lookup"><span data-stu-id="33dfc-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="33dfc-182">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="33dfc-183">Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="33dfc-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="33dfc-184">move</span><span class="sxs-lookup"><span data-stu-id="33dfc-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="33dfc-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="33dfc-186">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="33dfc-187">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="33dfc-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="33dfc-188">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="33dfc-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="33dfc-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="33dfc-190">Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="33dfc-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="33dfc-191">Obter mailFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="33dfc-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="33dfc-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="33dfc-193">Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="33dfc-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="33dfc-194">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="33dfc-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="33dfc-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="33dfc-196">Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="33dfc-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="33dfc-197">Obter mailFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="33dfc-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="33dfc-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="33dfc-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="33dfc-199">Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="33dfc-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="33dfc-200">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33dfc-200">Properties</span></span>

| <span data-ttu-id="33dfc-201">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33dfc-201">Property</span></span> | <span data-ttu-id="33dfc-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="33dfc-202">Type</span></span> | <span data-ttu-id="33dfc-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dfc-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="33dfc-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="33dfc-204">childFolderCount</span></span>|<span data-ttu-id="33dfc-205">Int32</span><span class="sxs-lookup"><span data-stu-id="33dfc-205">Int32</span></span>|<span data-ttu-id="33dfc-206">O número de mailFolders filho imediatas na mailFolder atual.</span><span class="sxs-lookup"><span data-stu-id="33dfc-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="33dfc-207">displayName</span><span class="sxs-lookup"><span data-stu-id="33dfc-207">displayName</span></span>|<span data-ttu-id="33dfc-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33dfc-208">String</span></span>|<span data-ttu-id="33dfc-209">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="33dfc-210">id</span><span class="sxs-lookup"><span data-stu-id="33dfc-210">id</span></span>|<span data-ttu-id="33dfc-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33dfc-211">String</span></span>|<span data-ttu-id="33dfc-212">Identificador exclusivo do mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="33dfc-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="33dfc-213">parentFolderId</span></span>|<span data-ttu-id="33dfc-214">String</span><span class="sxs-lookup"><span data-stu-id="33dfc-214">String</span></span>|<span data-ttu-id="33dfc-215">O identificador exclusivo de mailFolder do mailFolder pai.</span><span class="sxs-lookup"><span data-stu-id="33dfc-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="33dfc-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="33dfc-216">totalItemCount</span></span>|<span data-ttu-id="33dfc-217">Int32</span><span class="sxs-lookup"><span data-stu-id="33dfc-217">Int32</span></span>|<span data-ttu-id="33dfc-218">O número de itens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="33dfc-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="33dfc-219">unreadItemCount</span></span>|<span data-ttu-id="33dfc-220">Int32</span><span class="sxs-lookup"><span data-stu-id="33dfc-220">Int32</span></span>|<span data-ttu-id="33dfc-221">O número de itens na mailFolder marcados como não lidos.</span><span class="sxs-lookup"><span data-stu-id="33dfc-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="33dfc-222">**Acessar contagens de itens de forma eficiente**</span><span class="sxs-lookup"><span data-stu-id="33dfc-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="33dfc-223">O `TotalItemCount` e `UnreadItemCount` propriedades de uma pasta permitem que você convenientemente calcular o número de itens de leitura na pasta.</span><span class="sxs-lookup"><span data-stu-id="33dfc-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="33dfc-224">Eles permitem evitar consultas semelhante ao seguinte que pode acarretar uma latência significativa:</span><span class="sxs-lookup"><span data-stu-id="33dfc-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="33dfc-225">Pastas de email no Outlook podem conter mais de um tipo de itens, por exemplo, a caixa de entrada pode conter itens que são diferentes dos itens de email da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="33dfc-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="33dfc-226">`TotalItemCount`e `UnreadItemCount` incluir itens em uma pasta de email, independentemente de seus tipos de item.</span><span class="sxs-lookup"><span data-stu-id="33dfc-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="33dfc-227">Relações</span><span class="sxs-lookup"><span data-stu-id="33dfc-227">Relationships</span></span>

| <span data-ttu-id="33dfc-228">Relação</span><span class="sxs-lookup"><span data-stu-id="33dfc-228">Relationship</span></span> | <span data-ttu-id="33dfc-229">Tipo</span><span class="sxs-lookup"><span data-stu-id="33dfc-229">Type</span></span> | <span data-ttu-id="33dfc-230">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dfc-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="33dfc-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="33dfc-231">childFolders</span></span>|<span data-ttu-id="33dfc-232">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="33dfc-233">A coleção de pastas filho na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="33dfc-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="33dfc-234">messageRules</span></span> | <span data-ttu-id="33dfc-235">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="33dfc-236">A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="33dfc-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="33dfc-237">mensagens</span><span class="sxs-lookup"><span data-stu-id="33dfc-237">messages</span></span>|<span data-ttu-id="33dfc-238">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-238">[Message](message.md) collection</span></span>|<span data-ttu-id="33dfc-239">A coleção de mensagens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="33dfc-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="33dfc-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="33dfc-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="33dfc-241">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="33dfc-p110">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="33dfc-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="33dfc-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="33dfc-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="33dfc-246">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="33dfc-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="33dfc-p111">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="33dfc-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33dfc-250">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33dfc-250">JSON representation</span></span>

<span data-ttu-id="33dfc-251">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="33dfc-251">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="33dfc-252">Confira também</span><span class="sxs-lookup"><span data-stu-id="33dfc-252">See also</span></span>

- [<span data-ttu-id="33dfc-253">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="33dfc-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="33dfc-254">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="33dfc-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
