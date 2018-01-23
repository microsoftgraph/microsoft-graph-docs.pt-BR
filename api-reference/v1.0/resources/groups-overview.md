# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="b24e2-101">Trabalhando com grupos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b24e2-101">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="b24e2-102">Os grupos são coleções de [usuários](user.md) e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b24e2-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="b24e2-103">O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="b24e2-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="b24e2-104">Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.</span><span class="sxs-lookup"><span data-stu-id="b24e2-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="b24e2-105">**Observação**: os grupos só podem ser criados por meio de contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="b24e2-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="b24e2-106">As contas pessoais da Microsoft não são compatíveis com grupos.</span><span class="sxs-lookup"><span data-stu-id="b24e2-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="b24e2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b24e2-107">Type</span></span>              | <span data-ttu-id="b24e2-108">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="b24e2-108">Use case diagram</span></span> | <span data-ttu-id="b24e2-109">groupType</span><span class="sxs-lookup"><span data-stu-id="b24e2-109">groupType</span></span> | <span data-ttu-id="b24e2-110">habilitado para email</span><span class="sxs-lookup"><span data-stu-id="b24e2-110">mailEnabled</span></span> | <span data-ttu-id="b24e2-111">habilitado para segurança</span><span class="sxs-lookup"><span data-stu-id="b24e2-111">securityEnabled</span></span> | <span data-ttu-id="b24e2-112">Pode ser criado por meio de API?</span><span class="sxs-lookup"><span data-stu-id="b24e2-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="b24e2-113">Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="b24e2-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="b24e2-114">Facilitar a colaboração entre usuários com os recursos compartilhados online da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b24e2-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="b24e2-115">Sim</span><span class="sxs-lookup"><span data-stu-id="b24e2-115">Yes</span></span> | [<span data-ttu-id="b24e2-116">usuário</span><span class="sxs-lookup"><span data-stu-id="b24e2-116">user</span></span>](user.md) |
| [<span data-ttu-id="b24e2-117">Grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="b24e2-117">Security Groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="b24e2-118">Controlar o acesso do usuário aos recursos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b24e2-118">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="b24e2-119">Sim</span><span class="sxs-lookup"><span data-stu-id="b24e2-119">Yes</span></span> |
| [<span data-ttu-id="b24e2-120">Grupos de segurança habilitados para email</span><span class="sxs-lookup"><span data-stu-id="b24e2-120">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="b24e2-121">Controlar o acesso do usuário aos recursos do aplicativo, com uma caixa de correio de grupo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="b24e2-121">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="b24e2-122">Não</span><span class="sxs-lookup"><span data-stu-id="b24e2-122">No</span></span> |
| <span data-ttu-id="b24e2-123">Grupos de distribuição</span><span class="sxs-lookup"><span data-stu-id="b24e2-123">Distribution groups</span></span> | <span data-ttu-id="b24e2-124">Distribuir emails aos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="b24e2-124">Distributing mail to the members of the group.</span></span> <span data-ttu-id="b24e2-125">É recomendável usar os grupos do Office 365 devido ao conjunto de recursos mais sofisticado que ele oferece.</span><span class="sxs-lookup"><span data-stu-id="b24e2-125">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="b24e2-126">Não</span><span class="sxs-lookup"><span data-stu-id="b24e2-126">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="b24e2-127">Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="b24e2-127">Office 365 groups</span></span>
<span data-ttu-id="b24e2-128">O diferencial dos grupos do Office 365 é a natureza colaborativa, ideal para pessoas que trabalham juntas em um projeto ou em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b24e2-128">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="b24e2-129">Eles são criados com recursos compartilhados pelos membros do grupo, entre eles:</span><span class="sxs-lookup"><span data-stu-id="b24e2-129">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="b24e2-130">Conversas do Outlook</span><span class="sxs-lookup"><span data-stu-id="b24e2-130">Outlook conversations</span></span>
- <span data-ttu-id="b24e2-131">Calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="b24e2-131">Outlook calendar</span></span>
- <span data-ttu-id="b24e2-132">Arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b24e2-132">SharePoint files</span></span>
- <span data-ttu-id="b24e2-133">Bloco de anotações do OneNote</span><span class="sxs-lookup"><span data-stu-id="b24e2-133">A OneNote notebook.</span></span>
- <span data-ttu-id="b24e2-134">Site de equipe do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b24e2-134">SharePoint team site</span></span>
- <span data-ttu-id="b24e2-135">Planos do Planner</span><span class="sxs-lookup"><span data-stu-id="b24e2-135">Planner plans</span></span>
- <span data-ttu-id="b24e2-136">Gerenciamento de dispositivos do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b24e2-136">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="b24e2-137">Grupo em um exemplo do Outlook</span><span class="sxs-lookup"><span data-stu-id="b24e2-137">Group in Outlook example</span></span>

<span data-ttu-id="b24e2-138">Veja a seguir uma representação JSON dos grupos no Outlook.</span><span class="sxs-lookup"><span data-stu-id="b24e2-138">The following is a JSON representation of groups in Outlook.</span></span> 

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```
<span data-ttu-id="b24e2-139">Saiba mais sobre os grupos do Office 365 e as experiências de administrador no tópico [Saiba mais sobre grupos do Office 365](https://support.office.com/pt-BR/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="b24e2-139">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/pt-BR/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="b24e2-140">Grupos de segurança e grupos de segurança habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="b24e2-140">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="b24e2-141">Os grupos de segurança servem para controlar o acesso de usuários aos recursos.</span><span class="sxs-lookup"><span data-stu-id="b24e2-141">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="b24e2-142">Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b24e2-142">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="b24e2-143">Os grupos de segurança podem ter como membros usuários e outros grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="b24e2-143">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="b24e2-144">Os grupos de segurança habilitados para email são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada para os grupos.</span><span class="sxs-lookup"><span data-stu-id="b24e2-144">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="b24e2-145">Não é possível criar grupos de segurança habilitados para email por meio da API, mas as outras operações do grupo ainda funcionarão aqui.</span><span class="sxs-lookup"><span data-stu-id="b24e2-145">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span> <span data-ttu-id="b24e2-146">Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](https://technet.microsoft.com/pt-BR/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b24e2-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/pt-BR/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="b24e2-147">Exemplo de grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="b24e2-147">Security group example</span></span>

<span data-ttu-id="b24e2-148">Veja a seguir uma representação JSON de um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="b24e2-148">The following is a JSON representation of a security group.</span></span> 

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```
## <a name="dynamic-membership"></a><span data-ttu-id="b24e2-149">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="b24e2-149">Dynamic membership</span></span> 

<span data-ttu-id="b24e2-150">Todos os tipos de grupo podem ter regras de associação dinâmica que adicionam ou removem automaticamente membros do grupo com base nas propriedades do usuário.</span><span class="sxs-lookup"><span data-stu-id="b24e2-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="b24e2-151">Por exemplo, um grupo de "funcionários do Marketing" pode incluir todo usuário que tiver a propriedade departament definida como "Marketing". Dessa forma, os novos funcionários de marketing são adicionados automaticamente ao grupo, enquanto os que saem do departamento são automaticamente removidos dele.</span><span class="sxs-lookup"><span data-stu-id="b24e2-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="b24e2-152">Essa regra pode ser especificada em um campo "membershipRule" durante a criação de grupo como `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="b24e2-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="b24e2-153">O GroupType também deve incluir a `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="b24e2-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="b24e2-154">A solicitação a seguir cria um novo grupo do Office 365 para os funcionários de marketing:</span><span class="sxs-lookup"><span data-stu-id="b24e2-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

<span data-ttu-id="b24e2-155">Saiba como formular membershipRules no artigo [Criar regras baseadas em atributo para associação dinâmica de grupo no Azure Active Directory](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="b24e2-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="b24e2-156">**Observação**: as regras de associação dinâmica exigem que o locatário tenha uma licença ao nível [Azure Active Directory Premium P1](https://azure.microsoft.com/pt-BR/pricing/details/active-directory/) ou posterior.</span><span class="sxs-lookup"><span data-stu-id="b24e2-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/pt-BR/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="b24e2-157">Outros tipos de grupos</span><span class="sxs-lookup"><span data-stu-id="b24e2-157">Other types of groups</span></span>

<span data-ttu-id="b24e2-158">Os grupos do Office 365 no Yammer são usados para facilitar a colaboração de usuários por meio de publicações do Yammer.</span><span class="sxs-lookup"><span data-stu-id="b24e2-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="b24e2-159">Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API.</span><span class="sxs-lookup"><span data-stu-id="b24e2-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="b24e2-160">Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas em grupo do Office 365 são desabilitadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="b24e2-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="b24e2-161">Saiba mais em [Documentos API do desenvolvedor do Yammer](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="b24e2-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="b24e2-162">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="b24e2-162">Common use cases</span></span>

<span data-ttu-id="b24e2-163">Ao usar o Microsoft Graph, você pode executar as seguintes operações comuns.</span><span class="sxs-lookup"><span data-stu-id="b24e2-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="b24e2-164">**Casos de uso**</span><span class="sxs-lookup"><span data-stu-id="b24e2-164">**Use cases**</span></span>  | <span data-ttu-id="b24e2-165">**Recursos REST**</span><span class="sxs-lookup"><span data-stu-id="b24e2-165">**REST resources**</span></span> | <span data-ttu-id="b24e2-166">**Confira também**</span><span class="sxs-lookup"><span data-stu-id="b24e2-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b24e2-167">**Métodos e objetos de grupo**</span><span class="sxs-lookup"><span data-stu-id="b24e2-167">**Directory object and methods**</span></span> | | |
| <span data-ttu-id="b24e2-168">Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos.</span><span class="sxs-lookup"><span data-stu-id="b24e2-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="b24e2-169">Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="b24e2-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="b24e2-170">grupo</span><span class="sxs-lookup"><span data-stu-id="b24e2-170">group</span></span>](group.md) | [<span data-ttu-id="b24e2-171">Criar novos grupos</span><span class="sxs-lookup"><span data-stu-id="b24e2-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="b24e2-172">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="b24e2-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="b24e2-173">Atualizar grupos</span><span class="sxs-lookup"><span data-stu-id="b24e2-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="b24e2-174">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="b24e2-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="b24e2-175">**Métodos de associação a grupos**</span><span class="sxs-lookup"><span data-stu-id="b24e2-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="b24e2-176">Listar os membros de um grupo e adicionar ou remover membros.</span><span class="sxs-lookup"><span data-stu-id="b24e2-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="b24e2-177">usuário</span><span class="sxs-lookup"><span data-stu-id="b24e2-177">user</span></span>](user.md) <br/> [<span data-ttu-id="b24e2-178">grupo</span><span class="sxs-lookup"><span data-stu-id="b24e2-178">group</span></span>](group.md)| [<span data-ttu-id="b24e2-179">Listar membros</span><span class="sxs-lookup"><span data-stu-id="b24e2-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="b24e2-180">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="b24e2-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="b24e2-181">Remover membro</span><span class="sxs-lookup"><span data-stu-id="b24e2-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="b24e2-182">Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="b24e2-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="b24e2-183">usuário</span><span class="sxs-lookup"><span data-stu-id="b24e2-183">user</span></span>](user.md) <br/> [<span data-ttu-id="b24e2-184">grupo</span><span class="sxs-lookup"><span data-stu-id="b24e2-184">group</span></span>](group.md)| [<span data-ttu-id="b24e2-185">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="b24e2-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="b24e2-186">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="b24e2-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="b24e2-187">Listar os proprietários de um grupo e adicionar ou remover proprietários.</span><span class="sxs-lookup"><span data-stu-id="b24e2-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="b24e2-188">usuário</span><span class="sxs-lookup"><span data-stu-id="b24e2-188">user</span></span>](user.md) <br/> [<span data-ttu-id="b24e2-189">grupo</span><span class="sxs-lookup"><span data-stu-id="b24e2-189">group</span></span>](group.md)| [<span data-ttu-id="b24e2-190">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="b24e2-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="b24e2-191">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="b24e2-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="b24e2-192">Remover membro</span><span class="sxs-lookup"><span data-stu-id="b24e2-192">Remove member</span></span>](../api/group_delete_members.md)|
