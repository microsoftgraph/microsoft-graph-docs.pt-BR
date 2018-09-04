# <a name="mailfolder-resource-type"></a><span data-ttu-id="298d6-101">tipo de recurso mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-101">mailFolder resource type</span></span>

<span data-ttu-id="298d6-102">Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="298d6-102">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="298d6-103">As pastas de e-mail podem conter mensagens, outros itens do Outlook e pastas filho e-mails.</span><span class="sxs-lookup"><span data-stu-id="298d6-103">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="298d6-104">Esse recurso tem suporte para o uso da [consulta delta](../../../concepts/delta_query_overview.md) para acompanhar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder_delta.md).</span><span class="sxs-lookup"><span data-stu-id="298d6-104">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

<span data-ttu-id="298d6-105">**Nomes conhecidos de pasta**</span><span class="sxs-lookup"><span data-stu-id="298d6-105">**Well-known folder names**</span></span>

<span data-ttu-id="298d6-106">O Outlook cria determinadas pastas para usuários por padrão.</span><span class="sxs-lookup"><span data-stu-id="298d6-106">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="298d6-107">Em vez de usar o valor correspondente de **id** da pasta, para facilitar, você pode usar os nomes conhecidos listados na tabela abaixo para acessar as pastas.</span><span class="sxs-lookup"><span data-stu-id="298d6-107">Instead of using the corresponding folder id value, for convenience, you can use the following well-known folder names when accessing these folders in a mailFolder collection: , , , , , , , and .</span></span> <span data-ttu-id="298d6-108">Por exemplo, você pode obter a pasta Rascunhos usando seu nome conhecido com a seguinte consulta.</span><span class="sxs-lookup"><span data-stu-id="298d6-108">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="298d6-109">Os nomes conhecidos funcionam de forma independente da localidade da caixa de correio do usuário, portanto, a consulta acima sempre retorna a pasta Rascunhos, não importando como ela é chamada.</span><span class="sxs-lookup"><span data-stu-id="298d6-109">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="298d6-110">Nome conhecido de pasta</span><span class="sxs-lookup"><span data-stu-id="298d6-110">Well-known folder name</span></span> | <span data-ttu-id="298d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="298d6-111">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="298d6-112">archive</span><span class="sxs-lookup"><span data-stu-id="298d6-112">Archive</span></span> | <span data-ttu-id="298d6-113">As mensagens são enviadas para a pasta arquivo morto através do recurso de arquivamento com um clique nos clientes do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="298d6-113">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="298d6-114">**Observação:** isso não é o mesmo que o recurso de caixa de correio de arquivo morto do Exchange online.</span><span class="sxs-lookup"><span data-stu-id="298d6-114">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="298d6-115">clutter</span><span class="sxs-lookup"><span data-stu-id="298d6-115">Clutter</span></span> | <span data-ttu-id="298d6-116">As mensagens de baixa prioridade são movidas para a pasta de e-mail secundário ao usar o recurso de Email secundário.</span><span class="sxs-lookup"><span data-stu-id="298d6-116">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="298d6-117">conflicts</span><span class="sxs-lookup"><span data-stu-id="298d6-117">Conflicts</span></span> | <span data-ttu-id="298d6-118">A pasta que contém itens conflitantes na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="298d6-118">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="298d6-119">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="298d6-119">conversationhistory</span></span> | <span data-ttu-id="298d6-120">A pasta onde o Skype salva conversas de mensagens Instantâneas (se o Skype estiver configurado para isso).</span><span class="sxs-lookup"><span data-stu-id="298d6-120">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="298d6-121">deleteditems</span><span class="sxs-lookup"><span data-stu-id="298d6-121">deleteditems</span></span> | <span data-ttu-id="298d6-122">A pasta para onde os itens são movidos para quando são excluídos.</span><span class="sxs-lookup"><span data-stu-id="298d6-122">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="298d6-123">drafts</span><span class="sxs-lookup"><span data-stu-id="298d6-123">drafts</span></span> | <span data-ttu-id="298d6-124">A pasta que contém as mensagens não enviadas.</span><span class="sxs-lookup"><span data-stu-id="298d6-124">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="298d6-125">inbox</span><span class="sxs-lookup"><span data-stu-id="298d6-125">Inbox</span></span> | <span data-ttu-id="298d6-126">A pasta Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="298d6-126">The Inbox folder.</span></span> |
| <span data-ttu-id="298d6-127">junkemail</span><span class="sxs-lookup"><span data-stu-id="298d6-127">junkemail</span></span> | <span data-ttu-id="298d6-128">A pasta de lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="298d6-128">The Junk E-Mail folder.</span></span> |
| <span data-ttu-id="298d6-129">localfailures</span><span class="sxs-lookup"><span data-stu-id="298d6-129">localfailures</span></span> | <span data-ttu-id="298d6-130">A pasta que contém itens que existem no cliente local, mas não puderam ser carregados no servidor.</span><span class="sxs-lookup"><span data-stu-id="298d6-130">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="298d6-131">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="298d6-131">msgfolderroot</span></span> | <span data-ttu-id="298d6-132">A pasta da "Parte superior do armazenamento de informações".</span><span class="sxs-lookup"><span data-stu-id="298d6-132">The "Top of Information Store" folder.</span></span> <span data-ttu-id="298d6-133">Essa pasta é a pasta pai das pastas exibidas em clientes normais de e-mail, como a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="298d6-133">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="298d6-134">outbox</span><span class="sxs-lookup"><span data-stu-id="298d6-134">Outbox</span></span> | <span data-ttu-id="298d6-135">A pasta Caixa de Saída.</span><span class="sxs-lookup"><span data-stu-id="298d6-135">The Outbox folder.</span></span> |
| <span data-ttu-id="298d6-136">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="298d6-136">recoverableitemsdeletions</span></span> | <span data-ttu-id="298d6-137">A pasta que contém itens excluídos permanentemente: excluídos da pasta Itens excluídos ou pressionando shift + delete no Outlook.</span><span class="sxs-lookup"><span data-stu-id="298d6-137">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="298d6-138">Essa pasta não é visível em nenhum cliente de e-mail do Outlook, mas os usuários finais podem interagir com ela por meio do recurso **Recuperar itens excluídos do servidor** do Outlook ou do Outlook na web.</span><span class="sxs-lookup"><span data-stu-id="298d6-138">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="298d6-139">scheduled</span><span class="sxs-lookup"><span data-stu-id="298d6-139">scheduled</span></span> | <span data-ttu-id="298d6-140">A pasta que contém mensagens agendadas para reaparecer na caixa de entrada usando o recurso de Agendamento do Outlook para iOS.</span><span class="sxs-lookup"><span data-stu-id="298d6-140">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="298d6-141">searchfolders</span><span class="sxs-lookup"><span data-stu-id="298d6-141">searchfolders</span></span> | <span data-ttu-id="298d6-142">A pasta pai de todas as pastas de pesquisa definidas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="298d6-142">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="298d6-143">sentitems</span><span class="sxs-lookup"><span data-stu-id="298d6-143">sentitems</span></span> | <span data-ttu-id="298d6-144">A pasta itens enviados.</span><span class="sxs-lookup"><span data-stu-id="298d6-144">sent items folder</span></span> |
| <span data-ttu-id="298d6-145">serverfailures</span><span class="sxs-lookup"><span data-stu-id="298d6-145">serverfailures</span></span> | <span data-ttu-id="298d6-146">A pasta que contém itens que existem no servidor, mas que não puderam ser sincronizados no cliente local.</span><span class="sxs-lookup"><span data-stu-id="298d6-146">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="298d6-147">syncissues</span><span class="sxs-lookup"><span data-stu-id="298d6-147">syncissues</span></span> | <span data-ttu-id="298d6-148">A pasta que contém os logs de sincronização criados pelo Outlook.</span><span class="sxs-lookup"><span data-stu-id="298d6-148">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="298d6-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="298d6-149">Methods</span></span>

| <span data-ttu-id="298d6-150">Método</span><span class="sxs-lookup"><span data-stu-id="298d6-150">Method</span></span> | <span data-ttu-id="298d6-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="298d6-151">Return Type</span></span> | <span data-ttu-id="298d6-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="298d6-152">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="298d6-153">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-153">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="298d6-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-154">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="298d6-155">Leia as propriedades e os relacionamentos do objeto mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-155">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="298d6-156">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-156">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="298d6-157">MailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-157">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="298d6-158">Crie uma nova mailFolder na atual postando na coleção childFolders.</span><span class="sxs-lookup"><span data-stu-id="298d6-158">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="298d6-159">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="298d6-159">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="298d6-160">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-160">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="298d6-p106">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="298d6-p106">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="298d6-163">Criar Mensagem</span><span class="sxs-lookup"><span data-stu-id="298d6-163">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="298d6-164">Mensagem</span><span class="sxs-lookup"><span data-stu-id="298d6-164">Message</span></span>](message.md)| <span data-ttu-id="298d6-165">Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="298d6-165">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="298d6-166">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="298d6-166">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="298d6-167">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-167">[Message](message.md) collection</span></span>| <span data-ttu-id="298d6-168">Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="298d6-168">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="298d6-169">Update</span><span class="sxs-lookup"><span data-stu-id="298d6-169">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="298d6-170">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-170">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="298d6-171">Atualize o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="298d6-171">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="298d6-172">Delete</span><span class="sxs-lookup"><span data-stu-id="298d6-172">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="298d6-173">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="298d6-173">None</span></span> |<span data-ttu-id="298d6-174">Exclua o objeto mailFolder especificado.</span><span class="sxs-lookup"><span data-stu-id="298d6-174">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="298d6-175">copy</span><span class="sxs-lookup"><span data-stu-id="298d6-175">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="298d6-176">MailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-176">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="298d6-177">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-177">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="298d6-178">delta</span><span class="sxs-lookup"><span data-stu-id="298d6-178">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="298d6-179">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-179">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="298d6-180">Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="298d6-180">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="298d6-181">move</span><span class="sxs-lookup"><span data-stu-id="298d6-181">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="298d6-182">MailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-182">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="298d6-183">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-183">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="298d6-184">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="298d6-184">**Extended properties**</span></span>| | |
|[<span data-ttu-id="298d6-185">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="298d6-185">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="298d6-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-186">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="298d6-187">Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="298d6-187">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="298d6-188">Obter mailFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="298d6-188">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="298d6-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-189">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="298d6-190">Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="298d6-190">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="298d6-191">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="298d6-191">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="298d6-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-192">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="298d6-193">Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="298d6-193">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="298d6-194">Obter mailFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="298d6-194">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="298d6-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="298d6-195">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="298d6-196">Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="298d6-196">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="298d6-197">Propriedades</span><span class="sxs-lookup"><span data-stu-id="298d6-197">Properties</span></span>

| <span data-ttu-id="298d6-198">Propriedade</span><span class="sxs-lookup"><span data-stu-id="298d6-198">Property</span></span> | <span data-ttu-id="298d6-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="298d6-199">Type</span></span> | <span data-ttu-id="298d6-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="298d6-200">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="298d6-201">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="298d6-201">childFolderCount</span></span>|<span data-ttu-id="298d6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="298d6-202">Int32</span></span>|<span data-ttu-id="298d6-203">O número de mailFolders filho imediatas na mailFolder atual.</span><span class="sxs-lookup"><span data-stu-id="298d6-203">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="298d6-204">displayName</span><span class="sxs-lookup"><span data-stu-id="298d6-204">displayName</span></span>|<span data-ttu-id="298d6-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="298d6-205">String</span></span>|<span data-ttu-id="298d6-206">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-206">The mailFolder's display name.</span></span>|
|<span data-ttu-id="298d6-207">id</span><span class="sxs-lookup"><span data-stu-id="298d6-207">id</span></span>|<span data-ttu-id="298d6-208">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="298d6-208">String</span></span>|<span data-ttu-id="298d6-209">O Identificador exclusivo de mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-209">The folder's unique identifier.</span></span>|
|<span data-ttu-id="298d6-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="298d6-210">parentFolderId</span></span>|<span data-ttu-id="298d6-211">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="298d6-211">String</span></span>|<span data-ttu-id="298d6-212">O identificador exclusivo de mailFolder do mailFolder pai.</span><span class="sxs-lookup"><span data-stu-id="298d6-212">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="298d6-213">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="298d6-213">totalItemCount</span></span>|<span data-ttu-id="298d6-214">Int32</span><span class="sxs-lookup"><span data-stu-id="298d6-214">Int32</span></span>|<span data-ttu-id="298d6-215">O número de itens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-215">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="298d6-216">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="298d6-216">unreadItemCount</span></span>|<span data-ttu-id="298d6-217">Int32</span><span class="sxs-lookup"><span data-stu-id="298d6-217">Int32</span></span>|<span data-ttu-id="298d6-218">O número de itens na mailFolder marcados como não lidos.</span><span class="sxs-lookup"><span data-stu-id="298d6-218">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="298d6-219">**Acessar contagens de itens de forma eficiente**</span><span class="sxs-lookup"><span data-stu-id="298d6-219">**Access item counts efficiently**</span></span>

<span data-ttu-id="298d6-220">As propriedades `TotalItemCount` e `UnreadItemCount` de uma pasta permitem que você calcule convenientemente o número de itens lidos na pasta.</span><span class="sxs-lookup"><span data-stu-id="298d6-220">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
<span data-ttu-id="298d6-221">Eles permitem que você evite consultas como as seguintes, que podem incorrer em latência significativa:</span><span class="sxs-lookup"><span data-stu-id="298d6-221">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="298d6-222">Pastas de e-mail no Outlook podem conter mais de um tipo de item, por exemplo, a Caixa de entrada pode conter itens de solicitação de reunião que são distintos dos itens de e-mail.</span><span class="sxs-lookup"><span data-stu-id="298d6-222">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span> <span data-ttu-id="298d6-223">`TotalItemCount` e `UnreadItemCount` incluem itens em uma pasta de e-mail, independentemente de seus tipos de item.</span><span class="sxs-lookup"><span data-stu-id="298d6-223">`TotalItemCount` and `UnreadItemCount` include items in a folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="298d6-224">Relações</span><span class="sxs-lookup"><span data-stu-id="298d6-224">Relationships</span></span>

| <span data-ttu-id="298d6-225">Relação</span><span class="sxs-lookup"><span data-stu-id="298d6-225">Relationship</span></span> | <span data-ttu-id="298d6-226">Tipo</span><span class="sxs-lookup"><span data-stu-id="298d6-226">Type</span></span> | <span data-ttu-id="298d6-227">Descrição</span><span class="sxs-lookup"><span data-stu-id="298d6-227">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="298d6-228">childFolders</span><span class="sxs-lookup"><span data-stu-id="298d6-228">childFolders</span></span>|<span data-ttu-id="298d6-229">Coleção [MailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-229">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="298d6-230">A coleção de pastas filho na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-230">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="298d6-231">messageRules</span><span class="sxs-lookup"><span data-stu-id="298d6-231">messageRules</span></span> | <span data-ttu-id="298d6-232">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-232">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="298d6-233">A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="298d6-233">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="298d6-234">mensagens</span><span class="sxs-lookup"><span data-stu-id="298d6-234">messages</span></span>|<span data-ttu-id="298d6-235">Coleção [Message](message.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-235">[Message](message.md) collection</span></span>|<span data-ttu-id="298d6-236">A coleção de mensagens na mailFolder.</span><span class="sxs-lookup"><span data-stu-id="298d6-236">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="298d6-237">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="298d6-237">multiValueExtendedProperties</span></span>|<span data-ttu-id="298d6-238">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-238">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="298d6-p109">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="298d6-p109">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="298d6-242">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="298d6-242">singleValueExtendedProperties</span></span>|<span data-ttu-id="298d6-243">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="298d6-243">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="298d6-p110">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="298d6-p110">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="298d6-247">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="298d6-247">JSON representation</span></span>

<span data-ttu-id="298d6-248">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="298d6-248">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="298d6-249">Confira também</span><span class="sxs-lookup"><span data-stu-id="298d6-249">See also</span></span>

- [<span data-ttu-id="298d6-250">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="298d6-250">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="298d6-251">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="298d6-251">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
