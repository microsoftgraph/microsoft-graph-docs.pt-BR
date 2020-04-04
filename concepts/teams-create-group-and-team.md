---
title: Criar equipes e gerenciar membros usando o Microsoft Graph
description: 'Criar um grupo que inclui uma equipe envolve as seguintes etapas: '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3eb6871cbe4b68addf3924b3641cf5559a78374f
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144335"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a><span data-ttu-id="16d14-103">Criar equipes e gerenciar membros usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d14-103">Creating teams and managing members using Microsoft Graph</span></span>

<span data-ttu-id="16d14-104">Você pode usar a API do Microsoft Teams no Microsoft Graph para criar equipes de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="16d14-104">You can use the Microsoft Teams API in Microsoft Graph to create teams in multiple ways.</span></span> <span data-ttu-id="16d14-105">Este artigo descreve a abordagem que recomendamos para obter os melhores resultados.</span><span class="sxs-lookup"><span data-stu-id="16d14-105">This article describes the approach that we recommend for the best results.</span></span>


## <a name="initial-team-creation"></a><span data-ttu-id="16d14-106">Criação da equipe inicial</span><span class="sxs-lookup"><span data-stu-id="16d14-106">Initial team creation</span></span>

<span data-ttu-id="16d14-107">Todas as equipes têm o suporte de grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="16d14-107">All teams are backed by Office 365 groups.</span></span> <span data-ttu-id="16d14-108">A maneira mais rápida de configurar e utilizar sua equipe ao criar novas equipes através do Microsoft Graph é configurar um novo grupo do Office 365, todos os proprietários e membros e convertê-los em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="16d14-108">The quickest way to get your team up and running when you create new teams via Microsoft Graph is to set up a new Office 365 group, all all owners and members, and convert that into a team.</span></span>

1. <span data-ttu-id="16d14-109">Criar um [grupo do Office 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) usando a operação [criar grupo](/graph/api/group-post-groups?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="16d14-109">Create an [Office 365 group](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) using the [create group](/graph/api/group-post-groups?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="16d14-110">Se você estiver tentando configurar uma equipe de classe, use a operação [criar educationClass](/graph/api/educationroot-post-classes?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="16d14-110">If you're trying to set up a class team, use the [create educationClass](/graph/api/educationroot-post-classes?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="16d14-111">Você pode especificar os proprietários e os membros.</span><span class="sxs-lookup"><span data-stu-id="16d14-111">You can specify owners and members.</span></span> <span data-ttu-id="16d14-112">Certifique-se de que tenha os proprietários certos para a equipe recém-criada, conforme descrito na Etapa 2.</span><span class="sxs-lookup"><span data-stu-id="16d14-112">Make sure that you have the right owners for the newly created team, as described in Step 2.</span></span>

    <span data-ttu-id="16d14-113">Para incluir uma equipe, é necessário definir os seguintes valores de propriedade, conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="16d14-113">In order to include a team, you need to set the following property values, as shown:</span></span>

    - <span data-ttu-id="16d14-114">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="16d14-114">**groupTypes** = { "Unified" }</span></span> 
    - <span data-ttu-id="16d14-115">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="16d14-115">**mailEnabled** = true</span></span>
    - <span data-ttu-id="16d14-116">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="16d14-116">**securityEnabled** = false</span></span>

    ```http
    POST /groups
    {
        "displayName":"Flight 157",
        "mailNickname":"flight157",
        "description":"Everything about flight 157",
        "visibility":"Private",
        "groupTypes":["Unified"],
        "mailEnabled":true,
        "securityEnabled":false,
        "members@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
            "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
        ],
        "owners@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
        ]
    }
    ```

    <span data-ttu-id="16d14-117">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="16d14-117">The following example shows the response.</span></span> 

    ><span data-ttu-id="16d14-118">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16d14-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="16d14-119">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16d14-119">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. <span data-ttu-id="16d14-120">Certifique-se de que a equipe tenha dois ou mais proprietários.</span><span class="sxs-lookup"><span data-stu-id="16d14-120">Ensure the team has two or more owners.</span></span> <span data-ttu-id="16d14-121">É possível fazer isso por meio da operação [adicionar proprietário](/graph/api/group-post-owners?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="16d14-121">You can do so via the [add owner](/graph/api/group-post-owners?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="16d14-122">Elas devem ser contas de usuários reais e não contas de serviço.</span><span class="sxs-lookup"><span data-stu-id="16d14-122">These should be real user accounts and not service accounts.</span></span> <span data-ttu-id="16d14-123">Ter dois proprietários ajuda a lidar com casos em que um proprietário sai da empresa ou não está disponível para realizar operações de gerenciamento de equipe.</span><span class="sxs-lookup"><span data-stu-id="16d14-123">Having two owners helps handle cases where one owner leaves the company or is unavailable to perform team management operations.</span></span>

3. <span data-ttu-id="16d14-124">Adicione todos os membros (e convidados, se necessário) ao grupo usando a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-beta), caso não tenha feito isso na Etapa 1.</span><span class="sxs-lookup"><span data-stu-id="16d14-124">Add all members (and guests if necessary) to the group using the [add member](/graph/api/group-post-members?view=graph-rest-beta) operation, if you did not do so in Step 1.</span></span>

4. <span data-ttu-id="16d14-125">Depois que o grupo for criado com êxito, o que pode levar até 15 minutos após concluir a Etapa 1, crie uma equipe do Microsoft Teams usando a operação [criar equipe a partir do grupo](/graph/api/team-put-teams?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="16d14-125">After the group is successfully created, which can take upto 15 minutes after completing Step 1, create a Microsoft Teams team using the [create team from group](/graph/api/team-put-teams?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="16d14-126">Se houver um erro, o processo de criação de grupo pode não ser concluído, tente esperar alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="16d14-126">If you run into an error, the group creation process might not be completed; try waiting a few more minutes.</span></span>

    ```http
    PUT /groups/{id}/team
    { }
    ```

    <span data-ttu-id="16d14-127">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="16d14-127">The following example shows the response.</span></span> 

    ><span data-ttu-id="16d14-128">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16d14-128">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="16d14-129">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16d14-129">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
        "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
        "webUrl" : "https://example.com",
        "isArchived" : null,
        "memberSettings" : { },
        "guestSettings" : { },
        "messagingSettings" : { },
        "funSettings" : {}
    }
    ```

    <span data-ttu-id="16d14-130">A equipe criada tem a mesma ID do que o grupo.</span><span class="sxs-lookup"><span data-stu-id="16d14-130">The created team has the same ID as the group.</span></span>

5. <span data-ttu-id="16d14-131">Após concluir o processo, todos os proprietários e membros poderão ver a equipe recém-criada no cliente do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-131">After this process finishes, all owners and members should be able to see the newly created team in their Teams client.</span></span>

## <a name="adding-or-managing-members"></a><span data-ttu-id="16d14-132">Adicionar ou gerenciar membros</span><span class="sxs-lookup"><span data-stu-id="16d14-132">Adding or managing members</span></span>

<span data-ttu-id="16d14-133">Para adicionar membros depois de criar uma equipe, use a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="16d14-133">To add members after a team is created, you use the [add member](/graph/api/group-post-members?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="16d14-134">Observe o seguinte em relação às alterações de associação:</span><span class="sxs-lookup"><span data-stu-id="16d14-134">Note the following with respect to membership changes:</span></span>

1. <span data-ttu-id="16d14-135">As alterações de associação aplicadas ao grupos do Office 365 sincronizam com o Teams por meio de um mecanismo de sincronização em segundo plano que geralmente leva 24 horas (ou mais em alguns casos).</span><span class="sxs-lookup"><span data-stu-id="16d14-135">Membership changes made to Office 365 groups sync to Teams via a background sync mechanism that typically takes 24 hours (or more in some cases).</span></span>

2. <span data-ttu-id="16d14-136">O processo em segundo plano será acionado somente se um ou mais usuários na equipe (proprietário ou membro) estiverem ativos no cliente da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-136">The background process is triggered only if one or more users in the team (owner or member) is active in the Teams desktop client.</span></span> <span data-ttu-id="16d14-137">A inicialização do aplicativo Teams e/ou sua execução constitui atividade. Um usuário não precisa visitar especificamente a equipe que está sendo modificada.</span><span class="sxs-lookup"><span data-stu-id="16d14-137">Launching the Teams application and/or having it running constitutes activity — a user does not need to visit the team that is being modified specifically.</span></span>

    ><span data-ttu-id="16d14-138">**Observação:** os clientes móveis do Teams não acionam a sincronização de associações. Pelo menos um usuário deve estar no cliente da área de trabalho para garantir que o processo em segundo plano corra bem.</span><span class="sxs-lookup"><span data-stu-id="16d14-138">**Note:** The Teams mobile clients do not trigger the membership sync. At least one user should be on the desktop client to that ensure this background process goes smoothly.</span></span>

## <a name="checklist-for-validation"></a><span data-ttu-id="16d14-139">Lista de verificação para validação</span><span class="sxs-lookup"><span data-stu-id="16d14-139">Checklist for validation</span></span>

<span data-ttu-id="16d14-140">Depois de criar uma equipe, você pode usar a lista de verificação a seguir para verificar se a equipe foi criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="16d14-140">After you create a team, you can use the following checklist to verify that the team was created successfully.</span></span>

### <a name="validate-team-creation"></a><span data-ttu-id="16d14-141">Validar a criação de equipe</span><span class="sxs-lookup"><span data-stu-id="16d14-141">Validate team creation</span></span>

1. <span data-ttu-id="16d14-142">Verifique se o grupo do Office 365 que reforça a equipe foi criado por meio do Azure AD ou do centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16d14-142">Verify that the Office 365 group backing the team is created via the Azure AD or Microsoft 365 admin centers.</span></span>

2. <span data-ttu-id="16d14-143">Verifique se a criação da equipe foi bem-sucedida por meio do portal de administração do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-143">Verify that the team creation succeeded via the Teams admin portal.</span></span>

3. <span data-ttu-id="16d14-144">Verifique se a equipe possui os proprietários e membros corretos listados por meio do portal de administração do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-144">Verify that the team has the correct owners and members listed via the Teams admin portal.</span></span>

4. <span data-ttu-id="16d14-145">Verifique se os proprietários da equipe conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-145">Verify that the team owners can see the team after signing into the Teams desktop or web client.</span></span>

5. <span data-ttu-id="16d14-146">Verifique se os membros conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-146">Verify that members can see the team after signing into the Teams desktop or web client.</span></span>

### <a name="validate-addition-of-members"></a><span data-ttu-id="16d14-147">Validar a adição de membros</span><span class="sxs-lookup"><span data-stu-id="16d14-147">Validate addition of members</span></span>

1. <span data-ttu-id="16d14-148">Verifique se os novos membros aparecem no grupo por meio do Azure AD ou do centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16d14-148">Verify that newly members show up in the group via the Azure AD or Microsoft 365 admin center.</span></span>

2. <span data-ttu-id="16d14-149">Verifique se os membros recém-adicionados conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-149">Verify that newly added members can see the team after signing into the Teams desktop or web client.</span></span>



## <a name="how-office-365-group-membership-changes-are-synchronized-to-microsoft-teams"></a><span data-ttu-id="16d14-150">Como as alterações de associação de grupo do Office 365 são sincronizadas com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-150">How Office 365 group membership changes are synchronized to Microsoft Teams</span></span>

<span data-ttu-id="16d14-151">As alterações de associação feitas em grupo do Office 365 que reforça uma equipe por meio da API do Microsoft Graph ou através do portal de administração (fora do cliente do Teams) devem ser sincronizadas com o serviço do Teams para que os usuários recém-adicionados possam ver e participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="16d14-151">Membership changes made to an Office 365 group backing a team via the Microsoft Graph API or through the admin portal (outside of the Teams client) have to sync to the Teams service in order for newly added users to be able to see and participate in the team.</span></span> <span data-ttu-id="16d14-152">As alterações feitas diretamente à associação de grupo são sincronizadas com o serviço do Teams por meio de um processo em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="16d14-152">Changes made directly to the group membership are synchronized to the Teams service via a background process.</span></span> <span data-ttu-id="16d14-153">Esse processo em segundo plano é executado no serviço do Teams e é acionado pela atividade do usuário nos clientes da Web e da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="16d14-153">This background process runs in the Teams service and is triggered by user activity in Teams desktop and web clients.</span></span>

<span data-ttu-id="16d14-154">Para que o processo seja acionado, um proprietário ou membro atual da equipe (alguém que consiga ver a equipe no cliente do Teams) deve estar com o cliente da área de trabalho (ideal) ou da Web aberto.</span><span class="sxs-lookup"><span data-stu-id="16d14-154">For the process to get triggered, a current owner or member of that team (someone who can see the team in the Teams client) must have the Teams desktop (ideally) or web client open.</span></span> <span data-ttu-id="16d14-155">Os clientes móveis não acionam essa sincronização.</span><span class="sxs-lookup"><span data-stu-id="16d14-155">Mobile clients do not trigger this sync.</span></span>

<span data-ttu-id="16d14-156">O SLA atual para sincronizar as alterações de associação aplicada aos grupos no Teams é de até 24 horas após a sincronização ser acionada por atividade do cliente.</span><span class="sxs-lookup"><span data-stu-id="16d14-156">The current SLA for synchronizing membership changes made to groups to Teams is up to 24 hours after the sync is triggered by client activity.</span></span> <span data-ttu-id="16d14-157">Pode levar mais tempo em determinadas circunstâncias (devido à carga do serviço, por exemplo).</span><span class="sxs-lookup"><span data-stu-id="16d14-157">It can take longer under certain circumstances (due to service load, for example).</span></span>


![Processo de sincronização da lista de participação.](images/teams-roster-sync.png)

