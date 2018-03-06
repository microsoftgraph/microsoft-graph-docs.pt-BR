# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="4eb22-101">Trabalhando com grupos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4eb22-101">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="4eb22-102">Os grupos são coleções de [usuários](user.md) e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4eb22-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="4eb22-103">O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="4eb22-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="4eb22-104">Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.</span><span class="sxs-lookup"><span data-stu-id="4eb22-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="4eb22-105">**Observação**: os grupos só podem ser criados por meio de contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="4eb22-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="4eb22-106">As contas pessoais da Microsoft não são compatíveis com grupos.</span><span class="sxs-lookup"><span data-stu-id="4eb22-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="4eb22-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb22-107">Type</span></span>              | <span data-ttu-id="4eb22-108">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="4eb22-108">Use case</span></span> | <span data-ttu-id="4eb22-109">groupType</span><span class="sxs-lookup"><span data-stu-id="4eb22-109">groupType</span></span> | <span data-ttu-id="4eb22-110">habilitado para email</span><span class="sxs-lookup"><span data-stu-id="4eb22-110">mail-enabled</span></span> | <span data-ttu-id="4eb22-111">habilitado para segurança</span><span class="sxs-lookup"><span data-stu-id="4eb22-111">security-enabled</span></span> | <span data-ttu-id="4eb22-112">Pode ser criado por meio de API?</span><span class="sxs-lookup"><span data-stu-id="4eb22-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="4eb22-113">Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="4eb22-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="4eb22-114">Facilitar a colaboração entre usuários com os recursos compartilhados online da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4eb22-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="4eb22-115">Sim</span><span class="sxs-lookup"><span data-stu-id="4eb22-115">Yes</span></span> |
| [<span data-ttu-id="4eb22-116">Grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="4eb22-116">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="4eb22-117">Controlar o acesso do usuário aos recursos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4eb22-117">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="4eb22-118">Sim</span><span class="sxs-lookup"><span data-stu-id="4eb22-118">Yes</span></span> |
| [<span data-ttu-id="4eb22-119">Grupos de segurança habilitados para email</span><span class="sxs-lookup"><span data-stu-id="4eb22-119">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="4eb22-120">Controlar o acesso do usuário aos recursos do aplicativo, com uma caixa de correio de grupo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="4eb22-120">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="4eb22-121">Não</span><span class="sxs-lookup"><span data-stu-id="4eb22-121">No</span></span> |
| <span data-ttu-id="4eb22-122">Grupos de distribuição</span><span class="sxs-lookup"><span data-stu-id="4eb22-122">Distribution groups</span></span> | <span data-ttu-id="4eb22-123">Distribuir emails aos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="4eb22-123">Distributing mail to the members of the group.</span></span> <span data-ttu-id="4eb22-124">É recomendável usar os grupos do Office 365 devido ao conjunto de recursos mais sofisticado que ele oferece.</span><span class="sxs-lookup"><span data-stu-id="4eb22-124">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="4eb22-125">Não</span><span class="sxs-lookup"><span data-stu-id="4eb22-125">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="4eb22-126">Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="4eb22-126">Office 365 groups</span></span>
<span data-ttu-id="4eb22-127">O diferencial dos grupos do Office 365 é a natureza colaborativa, ideal para pessoas que trabalham juntas em um projeto ou em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="4eb22-127">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="4eb22-128">Eles são criados com recursos compartilhados pelos membros do grupo, entre eles:</span><span class="sxs-lookup"><span data-stu-id="4eb22-128">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="4eb22-129">Conversas do Outlook</span><span class="sxs-lookup"><span data-stu-id="4eb22-129">Outlook conversations</span></span>
- <span data-ttu-id="4eb22-130">Calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="4eb22-130">Outlook calendar</span></span>
- <span data-ttu-id="4eb22-131">Arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="4eb22-131">SharePoint files</span></span>
- <span data-ttu-id="4eb22-132">Bloco de anotações do OneNote</span><span class="sxs-lookup"><span data-stu-id="4eb22-132">OneNote notebook</span></span>
- <span data-ttu-id="4eb22-133">Site de equipe do SharePoint</span><span class="sxs-lookup"><span data-stu-id="4eb22-133">SharePoint team site</span></span>
- <span data-ttu-id="4eb22-134">Planos do Planner</span><span class="sxs-lookup"><span data-stu-id="4eb22-134">Planner plans</span></span>
- <span data-ttu-id="4eb22-135">Gerenciamento de dispositivos do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4eb22-135">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="4eb22-136">Grupo em um exemplo do Outlook</span><span class="sxs-lookup"><span data-stu-id="4eb22-136">Group in Outlook example</span></span>

<span data-ttu-id="4eb22-137">Veja a seguir uma representação JSON dos grupos no Outlook.</span><span class="sxs-lookup"><span data-stu-id="4eb22-137">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="4eb22-138">Saiba mais sobre os grupos do Office 365 e as experiências de administrador no tópico [Saiba mais sobre grupos do Office 365](https://support.office.com/pt-BR/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="4eb22-138">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/pt-BR/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="4eb22-139">Grupos de segurança e grupos de segurança habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="4eb22-139">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="4eb22-140">Os grupos de segurança servem para controlar o acesso de usuários aos recursos.</span><span class="sxs-lookup"><span data-stu-id="4eb22-140">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="4eb22-141">Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4eb22-141">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="4eb22-142">Os grupos de segurança podem ter como membros usuários e outros grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="4eb22-142">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="4eb22-143">Os grupos de segurança habilitados para email são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada para os grupos.</span><span class="sxs-lookup"><span data-stu-id="4eb22-143">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="4eb22-144">Não é possível criar grupos de segurança habilitados para email por meio da API, mas as outras operações do grupo funcionarão.</span><span class="sxs-lookup"><span data-stu-id="4eb22-144">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span>  <span data-ttu-id="4eb22-145">Grupos de segurança habilitados para email são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4eb22-145">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="4eb22-146">Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](https://technet.microsoft.com/pt-BR/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4eb22-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/pt-BR/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="4eb22-147">Exemplo de grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="4eb22-147">Security group example</span></span>

<span data-ttu-id="4eb22-148">Veja a seguir uma representação JSON de um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="4eb22-148">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="4eb22-149">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="4eb22-149">Dynamic membership</span></span> 

<span data-ttu-id="4eb22-150">Todos os tipos de grupo podem ter regras de associação dinâmica que adicionam ou removem automaticamente membros do grupo com base nas propriedades do usuário.</span><span class="sxs-lookup"><span data-stu-id="4eb22-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="4eb22-151">Por exemplo, um grupo de "funcionários do Marketing" pode incluir todo usuário que tiver a propriedade departament definida como "Marketing". Dessa forma, os novos funcionários de marketing são adicionados automaticamente ao grupo, enquanto os que saem do departamento são automaticamente removidos dele.</span><span class="sxs-lookup"><span data-stu-id="4eb22-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="4eb22-152">Essa regra pode ser especificada em um campo "membershipRule" durante a criação de grupo como `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="4eb22-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="4eb22-153">O GroupType também deve incluir a `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="4eb22-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="4eb22-154">A solicitação a seguir cria um novo grupo do Office 365 para os funcionários de marketing:</span><span class="sxs-lookup"><span data-stu-id="4eb22-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="4eb22-155">Saiba como formular membershipRules no artigo [Criar regras baseadas em atributo para associação dinâmica de grupo no Azure Active Directory](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4eb22-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="4eb22-156">**Observação**: as regras de associação dinâmica exigem que o locatário tenha uma licença ao nível [Azure Active Directory Premium P1](https://azure.microsoft.com/pt-BR/pricing/details/active-directory/) ou posterior.</span><span class="sxs-lookup"><span data-stu-id="4eb22-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/pt-BR/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="4eb22-157">Outros tipos de grupos</span><span class="sxs-lookup"><span data-stu-id="4eb22-157">Other types of groups</span></span>

<span data-ttu-id="4eb22-158">Os grupos do Office 365 no Yammer são usados para facilitar a colaboração de usuários por meio de publicações do Yammer.</span><span class="sxs-lookup"><span data-stu-id="4eb22-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="4eb22-159">Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API.</span><span class="sxs-lookup"><span data-stu-id="4eb22-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="4eb22-160">Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas em grupo do Office 365 são desabilitadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="4eb22-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="4eb22-161">Saiba mais em [Documentos API do desenvolvedor do Yammer](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="4eb22-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="4eb22-162">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="4eb22-162">Common use cases</span></span>

<span data-ttu-id="4eb22-163">Ao usar o Microsoft Graph, você pode executar as seguintes operações comuns.</span><span class="sxs-lookup"><span data-stu-id="4eb22-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="4eb22-164">**Casos de uso**</span><span class="sxs-lookup"><span data-stu-id="4eb22-164">**Use cases**</span></span>  | <span data-ttu-id="4eb22-165">**Recursos REST**</span><span class="sxs-lookup"><span data-stu-id="4eb22-165">**REST resources**</span></span> | <span data-ttu-id="4eb22-166">**Confira também**</span><span class="sxs-lookup"><span data-stu-id="4eb22-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4eb22-167">**Métodos e objetos de grupo**</span><span class="sxs-lookup"><span data-stu-id="4eb22-167">**Group object and methods**</span></span> | | |
| <span data-ttu-id="4eb22-168">Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos.</span><span class="sxs-lookup"><span data-stu-id="4eb22-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="4eb22-169">Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="4eb22-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="4eb22-170">grupo</span><span class="sxs-lookup"><span data-stu-id="4eb22-170">group</span></span>](group.md) | [<span data-ttu-id="4eb22-171">Criar novos grupos</span><span class="sxs-lookup"><span data-stu-id="4eb22-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="4eb22-172">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="4eb22-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="4eb22-173">Atualizar grupos</span><span class="sxs-lookup"><span data-stu-id="4eb22-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="4eb22-174">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="4eb22-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="4eb22-175">**Métodos de associação a grupos**</span><span class="sxs-lookup"><span data-stu-id="4eb22-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="4eb22-176">Listar os membros de um grupo e adicionar ou remover membros.</span><span class="sxs-lookup"><span data-stu-id="4eb22-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="4eb22-177">usuário</span><span class="sxs-lookup"><span data-stu-id="4eb22-177">user</span></span>](user.md) <br/> [<span data-ttu-id="4eb22-178">grupo</span><span class="sxs-lookup"><span data-stu-id="4eb22-178">group</span></span>](group.md)| [<span data-ttu-id="4eb22-179">Listar membros</span><span class="sxs-lookup"><span data-stu-id="4eb22-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="4eb22-180">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="4eb22-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="4eb22-181">Remover membro</span><span class="sxs-lookup"><span data-stu-id="4eb22-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="4eb22-182">Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="4eb22-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="4eb22-183">usuário</span><span class="sxs-lookup"><span data-stu-id="4eb22-183">user</span></span>](user.md) <br/> [<span data-ttu-id="4eb22-184">grupo</span><span class="sxs-lookup"><span data-stu-id="4eb22-184">group</span></span>](group.md)| [<span data-ttu-id="4eb22-185">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="4eb22-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="4eb22-186">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="4eb22-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="4eb22-187">Listar os proprietários de um grupo e adicionar ou remover proprietários.</span><span class="sxs-lookup"><span data-stu-id="4eb22-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="4eb22-188">usuário</span><span class="sxs-lookup"><span data-stu-id="4eb22-188">user</span></span>](user.md) <br/> [<span data-ttu-id="4eb22-189">grupo</span><span class="sxs-lookup"><span data-stu-id="4eb22-189">group</span></span>](group.md)| [<span data-ttu-id="4eb22-190">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="4eb22-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="4eb22-191">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="4eb22-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="4eb22-192">Remover membro</span><span class="sxs-lookup"><span data-stu-id="4eb22-192">Remove member</span></span>](../api/group_delete_members.md)|
