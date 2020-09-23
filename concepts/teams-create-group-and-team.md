---
title: Criar equipes e gerenciar membros usando o Microsoft Graph
description: 'Criar um grupo que inclui uma equipe envolve as seguintes etapas: '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 28729e0116e0b2959690449694197ac6acbfa501
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192767"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a><span data-ttu-id="4e53d-103">Criar equipes e gerenciar membros usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4e53d-103">Creating teams and managing members using Microsoft Graph</span></span>

<span data-ttu-id="4e53d-104">Você pode usar a API do Microsoft Teams no Microsoft Graph para criar equipes de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="4e53d-104">You can use the Microsoft Teams API in Microsoft Graph to create teams in multiple ways.</span></span> <span data-ttu-id="4e53d-105">Este artigo descreve a abordagem que recomendamos para obter os melhores resultados.</span><span class="sxs-lookup"><span data-stu-id="4e53d-105">This article describes the approach that we recommend for the best results.</span></span>


## <a name="initial-team-creation"></a><span data-ttu-id="4e53d-106">Criação da equipe inicial</span><span class="sxs-lookup"><span data-stu-id="4e53d-106">Initial team creation</span></span>

<span data-ttu-id="4e53d-107">Todas as equipes têm o respaldo de grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4e53d-107">All teams are backed by Microsoft 365 groups.</span></span> <span data-ttu-id="4e53d-108">A maneira mais rápida de configurar e utilizar sua equipe ao criar novas equipes através do Microsoft Graph é configurar um novo grupo do Microsoft 365, todos os proprietários e membros e convertê-los em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="4e53d-108">The quickest way to get your team up and running when you create new teams via Microsoft Graph is to set up a new Microsoft 365 group, all owners and members, and convert that into a team.</span></span>

1. <span data-ttu-id="4e53d-109">Criar um [grupo do Microsoft 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) usando a operação [criar grupo](/graph/api/group-post-groups?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="4e53d-109">Create an [Microsoft 365 group](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) using the [create group](/graph/api/group-post-groups?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="4e53d-110">Você pode especificar os proprietários e os membros.</span><span class="sxs-lookup"><span data-stu-id="4e53d-110">You can specify owners and members.</span></span> <span data-ttu-id="4e53d-111">Certifique-se de que tenha os proprietários certos do grupo recém-criado, conforme descrito na Etapa 2.</span><span class="sxs-lookup"><span data-stu-id="4e53d-111">Make sure that you have the right owners for the newly created group, as described in Step 2.</span></span>

    <span data-ttu-id="4e53d-112">Para criar uma equipe para esse grupo, é necessário definir os seguintes valores de propriedade, conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="4e53d-112">In order to create a team for this group, you need to set the following property values, as shown:</span></span>

    - <span data-ttu-id="4e53d-113">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="4e53d-113">**groupTypes** = { "Unified" }</span></span> 
    - <span data-ttu-id="4e53d-114">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="4e53d-114">**mailEnabled** = true</span></span>
    - <span data-ttu-id="4e53d-115">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="4e53d-115">**securityEnabled** = false</span></span>

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

    <span data-ttu-id="4e53d-116">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e53d-116">The following example shows the response.</span></span> 

    ><span data-ttu-id="4e53d-117">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4e53d-117">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="4e53d-118">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e53d-118">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. <span data-ttu-id="4e53d-119">Certifique-se de que o grupo tenha dois ou mais proprietários.</span><span class="sxs-lookup"><span data-stu-id="4e53d-119">Ensure the group has two or more owners.</span></span> <span data-ttu-id="4e53d-120">É possível fazer isso por meio da operação [adicionar proprietário](/graph/api/group-post-owners?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="4e53d-120">You can do so via the [add owner](/graph/api/group-post-owners?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="4e53d-121">Elas devem ser contas de usuários reais e não contas de serviço.</span><span class="sxs-lookup"><span data-stu-id="4e53d-121">These should be real user accounts and not service accounts.</span></span> <span data-ttu-id="4e53d-122">Ter dois proprietários ajuda a lidar com casos em que um proprietário sai da empresa ou não está disponível para realizar operações de gerenciamento de equipe.</span><span class="sxs-lookup"><span data-stu-id="4e53d-122">Having two owners helps handle cases where one owner leaves the company or is unavailable to perform team management operations.</span></span>

3. <span data-ttu-id="4e53d-123">Adicione todos os membros (e convidados, se necessário) ao grupo usando a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0), caso não tenha feito isso na Etapa 1.</span><span class="sxs-lookup"><span data-stu-id="4e53d-123">Add all members (and guests if necessary) to the group using the [add member](/graph/api/group-post-members?view=graph-rest-1.0) operation, if you did not do so in Step 1.</span></span> <span data-ttu-id="4e53d-124">Se você estiver adicionando vários membros, adicione um atraso de 1 segundo após cada operação de adição.</span><span class="sxs-lookup"><span data-stu-id="4e53d-124">If you're adding multiple members, add a 1 second delay after each add operation.</span></span> 

4. <span data-ttu-id="4e53d-125">Depois que o grupo for criado com sucesso, o que pode levar até 15 minutos após a conclusão da Etapa 1, crie uma equipe do Microsoft Teams usando a operação [criar equipe a partir de grupo](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group).</span><span class="sxs-lookup"><span data-stu-id="4e53d-125">After the group is successfully created, which can take up to 15 minutes after completing Step 1, create a Microsoft Teams team using the [create team from group](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group) operation.</span></span> <span data-ttu-id="4e53d-126">Se houver um erro, o processo de criação de grupo pode não ser concluído, tente esperar alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="4e53d-126">If you run into an error, the group creation process might not be completed; try waiting a few more minutes.</span></span> 

    ```http
    POST https://graph.microsoft.com/beta/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    <span data-ttu-id="4e53d-127">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e53d-127">The following example shows the response.</span></span> 

    ><span data-ttu-id="4e53d-128">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4e53d-128">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="4e53d-129">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e53d-129">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 202 Accepted
    Content-Type: application/json
    Location: /teams/{teamId}/operations/{operationId}
    Content-Location: /teams/{teamId}
    {
    }
    ```

    <span data-ttu-id="4e53d-130">A equipe criada tem a mesma ID do que o grupo.</span><span class="sxs-lookup"><span data-stu-id="4e53d-130">The created team has the same ID as the group.</span></span>

5. <span data-ttu-id="4e53d-131">Após concluir o processo, todos os proprietários e membros poderão ver a equipe recém-criada no cliente do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-131">After this process finishes, all owners and members should be able to see the newly created team in their Teams client.</span></span>

## <a name="adding-or-managing-members"></a><span data-ttu-id="4e53d-132">Adicionar ou gerenciar membros</span><span class="sxs-lookup"><span data-stu-id="4e53d-132">Adding or managing members</span></span>

<span data-ttu-id="4e53d-133">Para adicionar membros depois de criar uma equipe, use a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="4e53d-133">To add members after a team is created, you use the [add member](/graph/api/group-post-members?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="4e53d-134">É recomendável adicionar um atraso de 1 segundo entre as operações adicionar.</span><span class="sxs-lookup"><span data-stu-id="4e53d-134">We recommend adding a 1 second delay between add operations.</span></span> <span data-ttu-id="4e53d-135">Observe o seguinte em relação às alterações de associação:</span><span class="sxs-lookup"><span data-stu-id="4e53d-135">Note the following with respect to membership changes:</span></span>

1. <span data-ttu-id="4e53d-136">As alterações de associação feitas nos grupos do Microsoft 365 são sincronizadas com o Teams por meio de um mecanismo de sincronização de tela de fundo que geralmente demora 24 horas ou mais, em alguns casos.</span><span class="sxs-lookup"><span data-stu-id="4e53d-136">Membership changes made to Microsoft 365 groups sync to Teams via a background sync mechanism that typically takes 24 hours (or more in some cases).</span></span>

2. <span data-ttu-id="4e53d-137">O processo em segundo plano será acionado somente se um ou mais usuários na equipe (proprietário ou membro) estiverem ativos no cliente da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-137">The background process is triggered only if one or more users in the team (owner or member) is active in the Teams desktop client.</span></span> <span data-ttu-id="4e53d-138">A inicialização do aplicativo Teams e/ou sua execução constitui atividade. Um usuário não precisa visitar especificamente a equipe que está sendo modificada.</span><span class="sxs-lookup"><span data-stu-id="4e53d-138">Launching the Teams application and/or having it running constitutes activity — a user does not need to visit the team that is being modified specifically.</span></span>

    ><span data-ttu-id="4e53d-139">**Observação:** os clientes móveis do Teams não acionam a sincronização de associações. Pelo menos um usuário deve estar no cliente da área de trabalho para garantir que o processo em segundo plano corra bem.</span><span class="sxs-lookup"><span data-stu-id="4e53d-139">**Note:** The Teams mobile clients do not trigger the membership sync. At least one user should be on the desktop client to that ensure this background process goes smoothly.</span></span>

## <a name="checklist-for-validation"></a><span data-ttu-id="4e53d-140">Lista de verificação para validação</span><span class="sxs-lookup"><span data-stu-id="4e53d-140">Checklist for validation</span></span>

<span data-ttu-id="4e53d-141">Depois de criar uma equipe, você pode usar a lista de verificação a seguir para verificar se a equipe foi criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="4e53d-141">After you create a team, you can use the following checklist to verify that the team was created successfully.</span></span>

### <a name="validate-team-creation"></a><span data-ttu-id="4e53d-142">Validar a criação de equipe</span><span class="sxs-lookup"><span data-stu-id="4e53d-142">Validate team creation</span></span>

1. <span data-ttu-id="4e53d-143">Verifique se o grupo do Microsoft 365 que reforça a equipe foi criado por meio do Azure AD ou do centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4e53d-143">Verify that the Microsoft 365 group backing the team is created via the Azure AD or Microsoft 365 admin centers.</span></span>

2. <span data-ttu-id="4e53d-144">Verifique se a criação da equipe foi bem-sucedida por meio do portal de administração do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-144">Verify that the team creation succeeded via the Teams admin portal.</span></span>

3. <span data-ttu-id="4e53d-145">Verifique se a equipe possui os proprietários e membros corretos listados por meio do portal de administração do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-145">Verify that the team has the correct owners and members listed via the Teams admin portal.</span></span>

4. <span data-ttu-id="4e53d-146">Verifique se os proprietários da equipe conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-146">Verify that the team owners can see the team after signing into the Teams desktop or web client.</span></span>

5. <span data-ttu-id="4e53d-147">Verifique se os membros conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-147">Verify that members can see the team after signing into the Teams desktop or web client.</span></span>

### <a name="validate-addition-of-members"></a><span data-ttu-id="4e53d-148">Validar a adição de membros</span><span class="sxs-lookup"><span data-stu-id="4e53d-148">Validate addition of members</span></span>

1. <span data-ttu-id="4e53d-149">Verifique se os novos membros aparecem no grupo por meio do Azure AD ou do centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4e53d-149">Verify that newly members show up in the group via the Azure AD or Microsoft 365 admin center.</span></span>

2. <span data-ttu-id="4e53d-150">Verifique se os membros recém-adicionados conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.</span><span class="sxs-lookup"><span data-stu-id="4e53d-150">Verify that newly added members can see the team after signing into the Teams desktop or web client.</span></span>
