---
title: Trabalhando com grupos no Microsoft Graph
description: Os grupos são conjuntos de usuários e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo. O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário. Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: c3766f7b8e7be3a97ff95d43bd61147e8c1c4fb7
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673865"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="0a9d5-105">Trabalhando com grupos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0a9d5-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="0a9d5-106">Os grupos são coleções de [usuários](user.md) e de outras entidades de segurança que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="0a9d5-107">O Microsoft Graph fornece APIs que você pode usar para criar e gerenciar os diferentes tipos e funcionalidades de grupo de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="0a9d5-108">Todas as operações relacionadas a grupos no Microsoft Graph exigem autorização do administrador.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="0a9d5-109">**Observação**: os grupos só podem ser criados por meio de contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="0a9d5-110">As contas pessoais da Microsoft não são compatíveis com grupos.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="0a9d5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-111">Type</span></span>              | <span data-ttu-id="0a9d5-112">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="0a9d5-112">Use case</span></span> | <span data-ttu-id="0a9d5-113">groupTypes</span><span class="sxs-lookup"><span data-stu-id="0a9d5-113">groupTypes</span></span> | <span data-ttu-id="0a9d5-114">habilitado para email</span><span class="sxs-lookup"><span data-stu-id="0a9d5-114">mail-enabled</span></span> | <span data-ttu-id="0a9d5-115">habilitado para segurança</span><span class="sxs-lookup"><span data-stu-id="0a9d5-115">security-enabled</span></span> | <span data-ttu-id="0a9d5-116">Podem ser criados e gerenciados via API?</span><span class="sxs-lookup"><span data-stu-id="0a9d5-116">Can be created and managed via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="0a9d5-117">Grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0a9d5-117">Microsoft 365 groups</span></span>](#microsoft-365-groups) | <span data-ttu-id="0a9d5-118">Facilitar a colaboração entre usuários com os recursos compartilhados online da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="0a9d5-119">Sim</span><span class="sxs-lookup"><span data-stu-id="0a9d5-119">Yes</span></span> |
| [<span data-ttu-id="0a9d5-120">Grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="0a9d5-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="0a9d5-121">Controlar o acesso do usuário aos recursos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="0a9d5-122">Sim</span><span class="sxs-lookup"><span data-stu-id="0a9d5-122">Yes</span></span> |
| [<span data-ttu-id="0a9d5-123">Grupos de segurança habilitados para email</span><span class="sxs-lookup"><span data-stu-id="0a9d5-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="0a9d5-124">Controlar o acesso do usuário aos recursos do aplicativo, com uma caixa de correio de grupo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="0a9d5-125">Não</span><span class="sxs-lookup"><span data-stu-id="0a9d5-125">No</span></span> |
| <span data-ttu-id="0a9d5-126">Grupos de distribuição</span><span class="sxs-lookup"><span data-stu-id="0a9d5-126">Distribution groups</span></span> | <span data-ttu-id="0a9d5-127">Distribuir emails aos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="0a9d5-128">É recomendável usar os grupos do Microsoft 365 devido a grande quantidade de recursos que ele fornece.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-128">It is recommended to use Microsoft 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="0a9d5-129">Não</span><span class="sxs-lookup"><span data-stu-id="0a9d5-129">No</span></span> |

## <a name="microsoft-365-groups"></a><span data-ttu-id="0a9d5-130">Grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0a9d5-130">Microsoft 365 groups</span></span>
<span data-ttu-id="0a9d5-131">O diferencial dos grupos da Microsoft 365 está na natureza cooperativa, perfeito para as pessoas que trabalham em conjunto em um projeto ou uma equipe.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-131">The power of Microsoft 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="0a9d5-132">Eles são criados com recursos compartilhados pelos membros do grupo, entre eles:</span><span class="sxs-lookup"><span data-stu-id="0a9d5-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="0a9d5-133">Conversas do Outlook</span><span class="sxs-lookup"><span data-stu-id="0a9d5-133">Outlook conversations</span></span>
- <span data-ttu-id="0a9d5-134">Calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="0a9d5-134">Outlook calendar</span></span>
- <span data-ttu-id="0a9d5-135">Arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="0a9d5-135">SharePoint files</span></span>
- <span data-ttu-id="0a9d5-136">Bloco de anotações do OneNote</span><span class="sxs-lookup"><span data-stu-id="0a9d5-136">OneNote notebook</span></span>
- <span data-ttu-id="0a9d5-137">Site de equipe do SharePoint</span><span class="sxs-lookup"><span data-stu-id="0a9d5-137">SharePoint team site</span></span>
- <span data-ttu-id="0a9d5-138">Planos do Planner</span><span class="sxs-lookup"><span data-stu-id="0a9d5-138">Planner plans</span></span>
- <span data-ttu-id="0a9d5-139">Gerenciamento de dispositivos do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0a9d5-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="0a9d5-140">Grupo em um exemplo do Outlook</span><span class="sxs-lookup"><span data-stu-id="0a9d5-140">Group in Outlook example</span></span>

<span data-ttu-id="0a9d5-141">Veja a seguir uma representação JSON dos grupos no Outlook.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-141">The following is a JSON representation of groups in Outlook.</span></span>

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
<span data-ttu-id="0a9d5-142">Para saber mais sobre os grupos do Microsoft 365 e as experiências de administrador, confira [Saiba mais sobre grupos do Microsoft 365](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="0a9d5-142">To learn more about Microsoft 365 groups and the administrator experiences, see [Learn about Microsoft 365 groups](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="0a9d5-143">Grupos de segurança e grupos de segurança habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="0a9d5-144">Os grupos de segurança servem para controlar o acesso de usuários aos recursos.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="0a9d5-145">Ao verificar se um usuário faz parte de um grupo de segurança, seu aplicativo pode tomar decisões de autorização quando esse usuário tentar acessar alguns recursos seguros do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="0a9d5-146">Os grupos de segurança podem ter como membros usuários e outros grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="0a9d5-147">Os grupos de segurança habilitados para email são usados da mesma forma que os grupos de segurança, mas com o recurso adicional de uma caixa de correio compartilhada para os grupos.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="0a9d5-148">Não é possível criar grupos de segurança habilitados para email por meio da API, mas as outras operações do grupo funcionarão.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="0a9d5-149">Grupos de segurança habilitados para email são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="0a9d5-150">Saiba mais no artigo [Gerenciar de grupos de segurança habilitados para email no Exchange](https://technet.microsoft.com/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0a9d5-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="0a9d5-151">Exemplo de grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="0a9d5-151">Security group example</span></span>

<span data-ttu-id="0a9d5-152">Veja a seguir uma representação JSON de um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-152">The following is a JSON representation of a security group.</span></span>

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
## <a name="dynamic-membership"></a><span data-ttu-id="0a9d5-153">Associação dinâmica</span><span class="sxs-lookup"><span data-stu-id="0a9d5-153">Dynamic membership</span></span>

<span data-ttu-id="0a9d5-154">Todos os tipos de grupo podem ter regras de associação dinâmica que adicionam ou removem automaticamente membros do grupo com base nas propriedades do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="0a9d5-155">Por exemplo, um grupo de "funcionários do Marketing" pode incluir todo usuário que tiver a propriedade departament definida como "Marketing". Dessa forma, os novos funcionários de marketing são adicionados automaticamente ao grupo, enquanto os que saem do departamento são automaticamente removidos dele.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="0a9d5-156">Essa regra pode ser especificada em um campo "membershipRule" durante a criação de grupo como `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="0a9d5-157">O GroupType também deve incluir a `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-157">GroupTypes must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="0a9d5-158">A solicitação a seguir cria um novo grupo do Microsoft 365 para os funcionários de marketing:</span><span class="sxs-lookup"><span data-stu-id="0a9d5-158">The following request creates a new Microsoft 365 group for the marketing employees:</span></span>

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

<span data-ttu-id="0a9d5-159">Saiba como formular membershipRules no artigo [Criar regras baseadas em atributo para associação dinâmica de grupo no Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="0a9d5-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="0a9d5-160">**Observação**: as regras de associação dinâmica exigem que o locatário tenha uma licença ao nível [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) ou posterior.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="0a9d5-161">Outros tipos de grupos</span><span class="sxs-lookup"><span data-stu-id="0a9d5-161">Other types of groups</span></span>

<span data-ttu-id="0a9d5-162">Os grupos do Microsoft 365 no Yammer são usados para facilitar a colaboração de usuários por meio de postagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-162">Microsoft 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="0a9d5-163">Esse tipo de grupo pode ser retornado por meio de uma solicitação de leitura, mas as postagens nele não podem ser acessadas por meio da API.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="0a9d5-164">Quando as postagens e os feeds de conversas do Yammer são habilitados em um grupo, as conversas padrão em grupo do Microsoft 365 são desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-164">When Yammer posts and conversation feeds are enabled on a group, default Microsoft 365 group conversations are disabled.</span></span> <span data-ttu-id="0a9d5-165">Saiba mais em [Documentos de API do desenvolvedor do Yammer](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="0a9d5-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="0a9d5-166">Licenciamento com base em grupo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-166">Group-based licensing</span></span>

<span data-ttu-id="0a9d5-167">Você pode usar o licenciamento com base em grupo para atribuir uma ou mais licenças de produto a um grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-167">You can use group-based licensing to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="0a9d5-168">O Azure AD garante que as licenças sejam atribuídas a todos os membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-168">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="0a9d5-169">Todos os novos membros que ingressarem no grupo receberão as licenças apropriadas.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-169">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="0a9d5-170">Quando eles deixarem o grupo, essas licenças serão removidas.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-170">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="0a9d5-171">O recurso só pode ser usado com os grupos de segurança e grupos do Microsoft 365 que possuam `securityEnabled=TRUE`.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-171">The feature can only be used with security groups and Microsoft 365 groups that have `securityEnabled=TRUE`.</span></span> <span data-ttu-id="0a9d5-172">Para saber mais sobre o licenciamento com base em grupo, confira [O que é licenciamento com base em grupo no Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="0a9d5-172">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="0a9d5-173">Casos de usos comuns</span><span class="sxs-lookup"><span data-stu-id="0a9d5-173">Common use cases</span></span>

<span data-ttu-id="0a9d5-174">Ao usar o Microsoft Graph, você pode executar as seguintes operações comuns.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-174">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="0a9d5-175">**Casos de uso**</span><span class="sxs-lookup"><span data-stu-id="0a9d5-175">**Use cases**</span></span>  | <span data-ttu-id="0a9d5-176">**Recursos REST**</span><span class="sxs-lookup"><span data-stu-id="0a9d5-176">**REST resources**</span></span> | <span data-ttu-id="0a9d5-177">**Confira também**</span><span class="sxs-lookup"><span data-stu-id="0a9d5-177">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="0a9d5-178">**Métodos e objetos de grupo**</span><span class="sxs-lookup"><span data-stu-id="0a9d5-178">**Group object and methods**</span></span> | | |
| <span data-ttu-id="0a9d5-179">Criar novos grupos, obter os grupos existentes, atualizar as propriedades nos grupos e excluir grupos.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-179">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="0a9d5-180">Atualmente, somente os grupos de segurança e grupos no Outlook podem ser criados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-180">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="0a9d5-181">grupo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-181">group</span></span>](group.md) | [<span data-ttu-id="0a9d5-182">Criar novos grupos</span><span class="sxs-lookup"><span data-stu-id="0a9d5-182">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="0a9d5-183">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="0a9d5-183">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="0a9d5-184">Atualizar grupos</span><span class="sxs-lookup"><span data-stu-id="0a9d5-184">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="0a9d5-185">Excluir grupos</span><span class="sxs-lookup"><span data-stu-id="0a9d5-185">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="0a9d5-186">**Métodos de associação a grupos**</span><span class="sxs-lookup"><span data-stu-id="0a9d5-186">**Group membership methods**</span></span> | | |
| <span data-ttu-id="0a9d5-187">Listar os membros de um grupo e adicionar ou remover membros.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-187">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="0a9d5-188">usuário</span><span class="sxs-lookup"><span data-stu-id="0a9d5-188">user</span></span>](user.md) <br/> [<span data-ttu-id="0a9d5-189">grupo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-189">group</span></span>](group.md)| [<span data-ttu-id="0a9d5-190">Listar membros</span><span class="sxs-lookup"><span data-stu-id="0a9d5-190">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="0a9d5-191">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="0a9d5-191">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="0a9d5-192">Remover membro</span><span class="sxs-lookup"><span data-stu-id="0a9d5-192">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="0a9d5-193">Determinar se um usuário faz parte de um grupo, acessar todos os grupos do qual o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-193">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="0a9d5-194">usuário</span><span class="sxs-lookup"><span data-stu-id="0a9d5-194">user</span></span>](user.md) <br/> [<span data-ttu-id="0a9d5-195">grupo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-195">group</span></span>](group.md)| [<span data-ttu-id="0a9d5-196">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="0a9d5-196">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="0a9d5-197">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="0a9d5-197">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="0a9d5-198">Listar os proprietários de um grupo e adicionar ou remover proprietários.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-198">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="0a9d5-199">usuário</span><span class="sxs-lookup"><span data-stu-id="0a9d5-199">user</span></span>](user.md) <br/> [<span data-ttu-id="0a9d5-200">grupo</span><span class="sxs-lookup"><span data-stu-id="0a9d5-200">group</span></span>](group.md)| [<span data-ttu-id="0a9d5-201">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="0a9d5-201">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="0a9d5-202">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="0a9d5-202">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="0a9d5-203">Remover membro</span><span class="sxs-lookup"><span data-stu-id="0a9d5-203">Remove member</span></span>](../api/group-delete-members.md)|

## <a name="whats-new"></a><span data-ttu-id="0a9d5-204">Novidades</span><span class="sxs-lookup"><span data-stu-id="0a9d5-204">What's new</span></span>
<span data-ttu-id="0a9d5-205">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="0a9d5-205">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
