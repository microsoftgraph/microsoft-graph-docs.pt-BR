---
title: Trabalhando com grupos no Microsoft Graph
description: Os grupos são conjuntos de usuários e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo. O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário. Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 5bba894a107c75b1df815579f1d03d97fa964e24
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680085"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="ccc14-105">Trabalhando com grupos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ccc14-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="ccc14-106">Os grupos são coleções de [usuários](user.md) e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccc14-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="ccc14-107">O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="ccc14-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="ccc14-108">Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.</span><span class="sxs-lookup"><span data-stu-id="ccc14-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="ccc14-109">**Observação**: os grupos só podem ser criados por meio de contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="ccc14-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="ccc14-110">As contas pessoais da Microsoft não são compatíveis com grupos.</span><span class="sxs-lookup"><span data-stu-id="ccc14-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="ccc14-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc14-111">Type</span></span>              | <span data-ttu-id="ccc14-112">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="ccc14-112">Use case</span></span> | <span data-ttu-id="ccc14-113">groupTypes</span><span class="sxs-lookup"><span data-stu-id="ccc14-113">groupTypes</span></span> | <span data-ttu-id="ccc14-114">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ccc14-114">mailEnabled</span></span> | <span data-ttu-id="ccc14-115">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ccc14-115">securityEnabled</span></span> | <span data-ttu-id="ccc14-116">Criado e gerenciado via API</span><span class="sxs-lookup"><span data-stu-id="ccc14-116">Created and managed via API</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="ccc14-117">Grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ccc14-117">Microsoft 365 groups</span></span>](#microsoft-365-groups) | <span data-ttu-id="ccc14-118">Facilitar a colaboração entre usuários com os recursos compartilhados online da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ccc14-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | <span data-ttu-id="ccc14-119">`true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="ccc14-119">`true` or `false`</span></span> | <span data-ttu-id="ccc14-120">Sim</span><span class="sxs-lookup"><span data-stu-id="ccc14-120">Yes</span></span> |
| [<span data-ttu-id="ccc14-121">Grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="ccc14-121">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="ccc14-122">Controlar o acesso do usuário aos recursos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccc14-122">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="ccc14-123">Sim</span><span class="sxs-lookup"><span data-stu-id="ccc14-123">Yes</span></span> |
| [<span data-ttu-id="ccc14-124">Grupos de segurança habilitados para email</span><span class="sxs-lookup"><span data-stu-id="ccc14-124">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="ccc14-125">Controlar o acesso do usuário aos recursos do aplicativo, com uma caixa de correio de grupo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="ccc14-125">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="ccc14-126">Não</span><span class="sxs-lookup"><span data-stu-id="ccc14-126">No</span></span> |
| <span data-ttu-id="ccc14-127">Grupos de distribuição</span><span class="sxs-lookup"><span data-stu-id="ccc14-127">Distribution groups</span></span> | <span data-ttu-id="ccc14-128">Distribuir emails aos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="ccc14-128">Distributing mail to the members of the group.</span></span> <span data-ttu-id="ccc14-129">É recomendável usar os grupos do Microsoft 365 devido a grande quantidade de recursos que ele fornece.</span><span class="sxs-lookup"><span data-stu-id="ccc14-129">It is recommended to use Microsoft 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="ccc14-130">Não</span><span class="sxs-lookup"><span data-stu-id="ccc14-130">No</span></span> |

## <a name="microsoft-365-groups"></a><span data-ttu-id="ccc14-131">Grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ccc14-131">Microsoft 365 groups</span></span>
<span data-ttu-id="ccc14-132">O diferencial dos grupos da Microsoft 365 está na natureza cooperativa, perfeito para as pessoas que trabalham em conjunto em um projeto ou uma equipe.</span><span class="sxs-lookup"><span data-stu-id="ccc14-132">The power of Microsoft 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="ccc14-133">Eles são criados com recursos compartilhados pelos membros do grupo, entre eles:</span><span class="sxs-lookup"><span data-stu-id="ccc14-133">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="ccc14-134">Conversas do Outlook</span><span class="sxs-lookup"><span data-stu-id="ccc14-134">Outlook conversations</span></span>
- <span data-ttu-id="ccc14-135">Calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="ccc14-135">Outlook calendar</span></span>
- <span data-ttu-id="ccc14-136">Arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="ccc14-136">SharePoint files</span></span>
- <span data-ttu-id="ccc14-137">Bloco de anotações do OneNote</span><span class="sxs-lookup"><span data-stu-id="ccc14-137">OneNote notebook</span></span>
- <span data-ttu-id="ccc14-138">Site de equipe do SharePoint</span><span class="sxs-lookup"><span data-stu-id="ccc14-138">SharePoint team site</span></span>
- <span data-ttu-id="ccc14-139">Planos do Planner</span><span class="sxs-lookup"><span data-stu-id="ccc14-139">Planner plans</span></span>
- <span data-ttu-id="ccc14-140">Gerenciamento de dispositivos do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ccc14-140">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="ccc14-141">Grupo em um exemplo do Outlook</span><span class="sxs-lookup"><span data-stu-id="ccc14-141">Group in Outlook example</span></span>

<span data-ttu-id="ccc14-142">Veja a seguir uma representação JSON dos grupos no Outlook.</span><span class="sxs-lookup"><span data-stu-id="ccc14-142">The following is a JSON representation of groups in Outlook.</span></span>

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
<span data-ttu-id="ccc14-143">Para saber mais sobre os grupos do Microsoft 365 e as experiências de administrador, confira [Saiba mais sobre grupos do Microsoft 365](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="ccc14-143">To learn more about Microsoft 365 groups and the administrator experiences, see [Learn about Microsoft 365 groups](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="ccc14-144">Grupos de segurança e grupos de segurança habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="ccc14-144">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="ccc14-145">Os grupos de segurança servem para controlar o acesso de usuários aos recursos.</span><span class="sxs-lookup"><span data-stu-id="ccc14-145">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="ccc14-146">Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccc14-146">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="ccc14-147">Os grupos de segurança podem ter como membros usuários e outros grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="ccc14-147">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="ccc14-148">Os grupos de segurança habilitados para email são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada para os grupos.</span><span class="sxs-lookup"><span data-stu-id="ccc14-148">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="ccc14-149">Não é possível criar grupos de segurança habilitados para email por meio da API, mas as outras operações do grupo funcionarão.</span><span class="sxs-lookup"><span data-stu-id="ccc14-149">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="ccc14-150">Grupos de segurança habilitados para email são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc14-150">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="ccc14-151">Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](/Exchange/recipients/mail-enabled-security-groups).</span><span class="sxs-lookup"><span data-stu-id="ccc14-151">Learn more in the [Manage mail-enabled security groups Exchange article](/Exchange/recipients/mail-enabled-security-groups).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="ccc14-152">Exemplo de grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="ccc14-152">Security group example</span></span>

<span data-ttu-id="ccc14-153">Veja a seguir uma representação JSON de um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="ccc14-153">The following is a JSON representation of a security group.</span></span>

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
## <a name="dynamic-membership"></a><span data-ttu-id="ccc14-154">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="ccc14-154">Dynamic membership</span></span>

<span data-ttu-id="ccc14-155">Todos os tipos de grupo podem ter regras de associação dinâmica que adicionam ou removem automaticamente membros do grupo com base nas propriedades do usuário.</span><span class="sxs-lookup"><span data-stu-id="ccc14-155">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="ccc14-156">Por exemplo, um grupo de "funcionários do Marketing" pode incluir todo usuário que tiver a propriedade departament definida como "Marketing". Dessa forma, os novos funcionários de marketing são adicionados automaticamente ao grupo, enquanto os que saem do departamento são automaticamente removidos dele.</span><span class="sxs-lookup"><span data-stu-id="ccc14-156">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="ccc14-157">Essa regra pode ser especificada em um campo "membershipRule" durante a criação de grupo como `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="ccc14-157">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="ccc14-158">O GroupType também deve incluir a `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="ccc14-158">GroupTypes must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="ccc14-159">A solicitação a seguir cria um novo grupo do Microsoft 365 para os funcionários de marketing:</span><span class="sxs-lookup"><span data-stu-id="ccc14-159">The following request creates a new Microsoft 365 group for the marketing employees:</span></span>

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
    "membershipRule": "user.department -eq \"Marketing\"",
    "membershipRuleProcessingState": "on"
}
```

<span data-ttu-id="ccc14-160">Saiba como formular membershipRules no artigo [Criar regras baseadas em atributo para associação dinâmica de grupo no Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="ccc14-160">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="ccc14-161">**Observação**: as regras de associação dinâmica exigem que o locatário tenha uma licença ao nível [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ccc14-161">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="ccc14-162">Outros tipos de grupos</span><span class="sxs-lookup"><span data-stu-id="ccc14-162">Other types of groups</span></span>

<span data-ttu-id="ccc14-163">Os grupos do Microsoft 365 no Yammer são usados para facilitar a colaboração de usuários por meio de postagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="ccc14-163">Microsoft 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="ccc14-164">Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API.</span><span class="sxs-lookup"><span data-stu-id="ccc14-164">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="ccc14-165">Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas padrão em grupo do Microsoft 365 são desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="ccc14-165">When Yammer posts and conversation feeds are enabled on a group, default Microsoft 365 group conversations are disabled.</span></span> <span data-ttu-id="ccc14-166">Saiba mais em [Documentos de API do desenvolvedor do Yammer](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="ccc14-166">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="ccc14-167">Licenciamento com base em grupo</span><span class="sxs-lookup"><span data-stu-id="ccc14-167">Group-based licensing</span></span>

<span data-ttu-id="ccc14-168">Você pode usar o licenciamento com base em grupo para atribuir uma ou mais licenças de produto a um grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ccc14-168">You can use group-based licensing to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="ccc14-169">O Azure AD garante que as licenças sejam atribuídas a todos os membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="ccc14-169">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="ccc14-170">Todos os novos membros que ingressarem no grupo receberão as licenças apropriadas.</span><span class="sxs-lookup"><span data-stu-id="ccc14-170">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="ccc14-171">Quando eles deixarem o grupo, essas licenças serão removidas.</span><span class="sxs-lookup"><span data-stu-id="ccc14-171">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="ccc14-172">O recurso só pode ser usado com os grupos de segurança e grupos do Microsoft 365 que possuam `securityEnabled=TRUE`.</span><span class="sxs-lookup"><span data-stu-id="ccc14-172">The feature can only be used with security groups and Microsoft 365 groups that have `securityEnabled=TRUE`.</span></span> <span data-ttu-id="ccc14-173">Para saber mais sobre o licenciamento com base em grupo, confira [O que é licenciamento com base em grupo no Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="ccc14-173">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="ccc14-174">Casos de usos comuns</span><span class="sxs-lookup"><span data-stu-id="ccc14-174">Common use cases</span></span>

<span data-ttu-id="ccc14-175">Ao usar o Microsoft Graph, você pode executar as seguintes operações comuns.</span><span class="sxs-lookup"><span data-stu-id="ccc14-175">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="ccc14-176">**Casos de uso**</span><span class="sxs-lookup"><span data-stu-id="ccc14-176">**Use cases**</span></span>  | <span data-ttu-id="ccc14-177">**Recursos REST**</span><span class="sxs-lookup"><span data-stu-id="ccc14-177">**REST resources**</span></span> | <span data-ttu-id="ccc14-178">**Confira também**</span><span class="sxs-lookup"><span data-stu-id="ccc14-178">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ccc14-179">**Métodos e objetos de grupo**</span><span class="sxs-lookup"><span data-stu-id="ccc14-179">**Group object and methods**</span></span> | | |
| <span data-ttu-id="ccc14-180">Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos.</span><span class="sxs-lookup"><span data-stu-id="ccc14-180">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="ccc14-181">Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="ccc14-181">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="ccc14-182">grupo</span><span class="sxs-lookup"><span data-stu-id="ccc14-182">group</span></span>](group.md) | [<span data-ttu-id="ccc14-183">Criar novos grupos</span><span class="sxs-lookup"><span data-stu-id="ccc14-183">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="ccc14-184">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="ccc14-184">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="ccc14-185">Atualizar grupos</span><span class="sxs-lookup"><span data-stu-id="ccc14-185">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="ccc14-186">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="ccc14-186">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="ccc14-187">**Métodos de associação a grupos**</span><span class="sxs-lookup"><span data-stu-id="ccc14-187">**Group membership methods**</span></span> | | |
| <span data-ttu-id="ccc14-188">Listar os membros de um grupo e adicionar ou remover membros.</span><span class="sxs-lookup"><span data-stu-id="ccc14-188">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="ccc14-189">usuário</span><span class="sxs-lookup"><span data-stu-id="ccc14-189">user</span></span>](user.md) <br/> [<span data-ttu-id="ccc14-190">grupo</span><span class="sxs-lookup"><span data-stu-id="ccc14-190">group</span></span>](group.md)| [<span data-ttu-id="ccc14-191">Listar membros</span><span class="sxs-lookup"><span data-stu-id="ccc14-191">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="ccc14-192">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="ccc14-192">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="ccc14-193">Remover membro</span><span class="sxs-lookup"><span data-stu-id="ccc14-193">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="ccc14-194">Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="ccc14-194">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="ccc14-195">usuário</span><span class="sxs-lookup"><span data-stu-id="ccc14-195">user</span></span>](user.md) <br/> [<span data-ttu-id="ccc14-196">grupo</span><span class="sxs-lookup"><span data-stu-id="ccc14-196">group</span></span>](group.md)| [<span data-ttu-id="ccc14-197">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="ccc14-197">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="ccc14-198">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="ccc14-198">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="ccc14-199">Listar os proprietários de um grupo e adicionar ou remover proprietários.</span><span class="sxs-lookup"><span data-stu-id="ccc14-199">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="ccc14-200">usuário</span><span class="sxs-lookup"><span data-stu-id="ccc14-200">user</span></span>](user.md) <br/> [<span data-ttu-id="ccc14-201">grupo</span><span class="sxs-lookup"><span data-stu-id="ccc14-201">group</span></span>](group.md)| [<span data-ttu-id="ccc14-202">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="ccc14-202">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="ccc14-203">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="ccc14-203">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="ccc14-204">Remover membro</span><span class="sxs-lookup"><span data-stu-id="ccc14-204">Remove member</span></span>](../api/group-delete-members.md)|

## <a name="whats-new"></a><span data-ttu-id="ccc14-205">Novidades</span><span class="sxs-lookup"><span data-stu-id="ccc14-205">What's new</span></span>
<span data-ttu-id="ccc14-206">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="ccc14-206">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>