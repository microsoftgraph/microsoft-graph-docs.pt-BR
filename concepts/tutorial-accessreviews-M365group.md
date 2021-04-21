---
title: 'Tutorial: Use a API de críticas de acesso para revisar o acesso de convidados aos seus grupos do Microsoft 365'
description: Usar a API de críticas de acesso para revisar o acesso de convidados aos seus grupos do Microsoft 365
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: 216d6e345fcbb2919593f95b327a2b83037e4535
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921065"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a><span data-ttu-id="15f85-103">Tutorial: Use a API de críticas de acesso para revisar o acesso de convidados aos seus grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15f85-103">Tutorial: Use the access reviews API to review guest access to your Microsoft 365 groups</span></span>

<span data-ttu-id="15f85-104">Neste tutorial, você usará o Graph Explorer para criar e ler avaliações de acesso que direcionam todos os grupos do Microsoft 365 com usuários convidados no locatário.</span><span class="sxs-lookup"><span data-stu-id="15f85-104">In this tutorial, you will use Graph Explorer to create and read access reviews that targets all Microsoft 365 groups with guest users in the tenant.</span></span> <span data-ttu-id="15f85-105">Para isso, você primeiro usará o Azure AD B2B para convidar e criar um usuário convidado, também conhecido como identidade externa, em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="15f85-105">To achieve this, you'll first use Azure AD B2B to invite and create a guest user, also referred to as an external identity, in your tenant.</span></span> <span data-ttu-id="15f85-106">Em seguida, você adicionará esse usuário convidado ao grupo do Microsoft 365 antes de criar e ler a revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-106">Then, you'll add this guest user to your Microsoft 365 group prior to creating and reading the access review.</span></span>

>[!NOTE]
><span data-ttu-id="15f85-107">Os objetos de resposta mostrados neste tutorial podem ser reduzidos para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="15f85-107">The response objects shown in this tutorial might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15f85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15f85-108">Prerequisites</span></span>

<span data-ttu-id="15f85-109">Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:</span><span class="sxs-lookup"><span data-stu-id="15f85-109">To complete this tutorial, you need the following resources and privileges:</span></span>

+ <span data-ttu-id="15f85-110">Um locatário do Azure AD funcionando com uma licença Azure AD Premium P2 ou EMS E5 habilitada.</span><span class="sxs-lookup"><span data-stu-id="15f85-110">A working Azure AD tenant with an Azure AD Premium P2 or EMS E5 license enabled.</span></span> 
+ <span data-ttu-id="15f85-111">Uma conta em um locatário diferente do Azure AD ou uma identidade social que você pode convidar como usuário convidado (usuário B2B).</span><span class="sxs-lookup"><span data-stu-id="15f85-111">An account in a different Azure AD tenant or a social identity that you can invite as a guest user (B2B user).</span></span>
+ <span data-ttu-id="15f85-112">Entre no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) como usuário em uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="15f85-112">Sign in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) as a user in a global administrator role.</span></span> 
+ <span data-ttu-id="15f85-113">As seguintes permissões delegadas: `User.Invite.All` , `AccessReview.ReadWrite.All` , , `Group.ReadWrite.All` `User.ReadWrite.All` .</span><span class="sxs-lookup"><span data-stu-id="15f85-113">The following delegated permissions: `User.Invite.All`, `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`, `User.ReadWrite.All`.</span></span>

<span data-ttu-id="15f85-114">Para consentir com as permissões necessárias no Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="15f85-114">To consent to the required permissions in Graph Explorer:</span></span>
1. <span data-ttu-id="15f85-115">Selecione o ícone de configurações à direita dos detalhes da conta do usuário e escolha **Selecionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="15f85-115">Select the settings icon to the right of the user account details, and then choose **Select permissions**.</span></span>
   
   <span data-ttu-id="15f85-116">![Selecionar as permissões do Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   </span><span class="sxs-lookup"><span data-stu-id="15f85-116">![Select the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. <span data-ttu-id="15f85-117">Role a lista de permissões para essas permissões:</span><span class="sxs-lookup"><span data-stu-id="15f85-117">Scroll through the list of permissions to these permissions:</span></span>
   + <span data-ttu-id="15f85-118">AccessReviews (3), expanda e selecione **AccessReviews.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="15f85-118">AccessReviews (3), expand and then select **AccessReviews.ReadWrite.All**.</span></span>
   + <span data-ttu-id="15f85-119">Grupo (2), expanda e selecione **Group.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="15f85-119">Group (2), expand and then select **Group.ReadWrite.All**.</span></span>
   + <span data-ttu-id="15f85-120">Usuário (8), expanda e selecione **User.Invite.All** e **User.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="15f85-120">User (8), expand and then select **User.Invite.All** and **User.ReadWrite.All**.</span></span>
   
   <span data-ttu-id="15f85-121">Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="15f85-121">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="15f85-122">Você não precisa consentir em nome da organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="15f85-122">You do not need to consent on behalf of your organization for these permissions.</span></span>
   
   <span data-ttu-id="15f85-123">![Consentimento para as permissões do Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
   </span><span class="sxs-lookup"><span data-stu-id="15f85-123">![Consent to the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-a-test-user-in-your-tenant"></a><span data-ttu-id="15f85-124">Etapa 1: Criar um usuário de teste em seu locatário</span><span class="sxs-lookup"><span data-stu-id="15f85-124">Step 1: Create a test user in your tenant</span></span>

### <a name="request"></a><span data-ttu-id="15f85-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-125">Request</span></span>

```http
POST /users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a><span data-ttu-id="15f85-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-126">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a><span data-ttu-id="15f85-127">Etapa 2: convidar um usuário convidado para seu locatário</span><span class="sxs-lookup"><span data-stu-id="15f85-127">Step 2: Invite a guest user into your tenant</span></span>

<span data-ttu-id="15f85-128">Convide um usuário convidado com o endereço de email **john@tailspintoys.com** seu locatário.</span><span class="sxs-lookup"><span data-stu-id="15f85-128">Invite a guest user with the email address **john@tailspintoys.com** to your tenant.</span></span>

### <a name="request"></a><span data-ttu-id="15f85-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-129">Request</span></span>

```http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a><span data-ttu-id="15f85-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-130">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a><span data-ttu-id="15f85-131">Etapa 3: criar um novo grupo do Microsoft 365 e adicionar o usuário convidado</span><span class="sxs-lookup"><span data-stu-id="15f85-131">Step 3: Create a new Microsoft 365 group and add the guest user</span></span>

<span data-ttu-id="15f85-132">Nesta etapa:</span><span class="sxs-lookup"><span data-stu-id="15f85-132">In this step:</span></span>
1. <span data-ttu-id="15f85-133">Crie um novo grupo do Microsoft 365 chamado **campanha de marketing Feelgood.**</span><span class="sxs-lookup"><span data-stu-id="15f85-133">Create a new Microsoft 365 group named **Feelgood marketing campaign**.</span></span>
2. <span data-ttu-id="15f85-134">Atribua a si mesmo como o proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="15f85-134">Assign yourself as the group owner.</span></span>
3. <span data-ttu-id="15f85-135">Adicione john@tailspintoys.com como membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="15f85-135">Add john@tailspintoys.com as a group member.</span></span> <span data-ttu-id="15f85-136">O acesso ao grupo é assunto de revisão por você, o proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="15f85-136">Their access to the group is the subject of review by you, the group owner.</span></span>

### <a name="request"></a><span data-ttu-id="15f85-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-137">Request</span></span>
<span data-ttu-id="15f85-138">Nesta chamada, substitua:</span><span class="sxs-lookup"><span data-stu-id="15f85-138">In this call, replace:</span></span>
+ <span data-ttu-id="15f85-139">`cdb555e3-b33e-4fd5-a427-17fadacbdfa7` com sua **id**. Para recuperar sua **id,** execute `GET` em `https://graph.microsoft.com/beta/me` .</span><span class="sxs-lookup"><span data-stu-id="15f85-139">`cdb555e3-b33e-4fd5-a427-17fadacbdfa7` with your **id**. To retrieve your **id**, run `GET` on `https://graph.microsoft.com/beta/me`.</span></span>
+ <span data-ttu-id="15f85-140">`baf1b0a0-1f9a-4a56-9884-6a30824f8d20` com **john@tailspintoys.com** **id** da resposta na Etapa 2.</span><span class="sxs-lookup"><span data-stu-id="15f85-140">`baf1b0a0-1f9a-4a56-9884-6a30824f8d20` with **john@tailspintoys.com**'s **id** from the response in Step 2.</span></span>

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Feelgood Marketing Campaign with external partners and vendors.",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ],
    "mailEnabled": true,
    "mailNickname": "FeelGoodCampaign",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a><span data-ttu-id="15f85-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-141">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

<span data-ttu-id="15f85-142">Agora você tem um grupo do Microsoft 365 com um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="15f85-142">You now have a Microsoft 365 group with a guest user.</span></span>

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a><span data-ttu-id="15f85-143">Etapa 4: Criar uma revisão de acesso para todos os grupos do Microsoft 365 com usuários convidados</span><span class="sxs-lookup"><span data-stu-id="15f85-143">Step 4: Create an access review for all Microsoft 365 groups with guest users</span></span>

<span data-ttu-id="15f85-144">Ao criar uma série de revisão de acesso recorrente para todos os grupos do Microsoft 365 com usuários convidados, agende uma revisão periódica do acesso dos convidados ao grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="15f85-144">When you create a recurring access review series for all Microsoft 365 groups with guest users, you schedule a periodic review of the guests' access to the Microsoft 365 group.</span></span> <span data-ttu-id="15f85-145">Faça isso para o **grupo Campanha de Marketing da Feelgood.**</span><span class="sxs-lookup"><span data-stu-id="15f85-145">Do this for the **Feelgood Marketing Campaign** group.</span></span>

<span data-ttu-id="15f85-146">A série de revisão de acesso usa as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="15f85-146">The access review series uses following settings:</span></span>
+ <span data-ttu-id="15f85-147">É uma revisão de acesso recorrente e revisada trimestralmente.</span><span class="sxs-lookup"><span data-stu-id="15f85-147">It's a recurring access review and reviewed quarterly.</span></span>
+ <span data-ttu-id="15f85-148">Os proprietários do grupo analisam o acesso contínuo de usuários convidados.</span><span class="sxs-lookup"><span data-stu-id="15f85-148">The group owners review the continued access of guest users.</span></span>
+ <span data-ttu-id="15f85-149">O escopo de revisão é limitado a grupos do Microsoft 365 somente **com usuários convidados.**</span><span class="sxs-lookup"><span data-stu-id="15f85-149">The review scope is limited to Microsoft 365 groups with **Guest users** only.</span></span>
+ <span data-ttu-id="15f85-150">Um revistor de backup.</span><span class="sxs-lookup"><span data-stu-id="15f85-150">A backup reviewer.</span></span> <span data-ttu-id="15f85-151">Pode ser um usuário de fallback ou um grupo que pode revisar o acesso caso o grupo não tenha proprietários atribuídos.</span><span class="sxs-lookup"><span data-stu-id="15f85-151">This can be a fallback user or a group that can review the access in case the group doesn't have any owners assigned.</span></span>
+ <span data-ttu-id="15f85-152">**autoApplyDecisionsEnabled** está definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="15f85-152">**autoApplyDecisionsEnabled** is set to `true`.</span></span> <span data-ttu-id="15f85-153">Nesse caso, as decisões são aplicadas automaticamente quando o revistor conclui a revisão de acesso ou a duração da revisão de acesso termina.</span><span class="sxs-lookup"><span data-stu-id="15f85-153">In this case, decisions are applied automatically once the reviewer completes the access review or the access review duration ends.</span></span> <span data-ttu-id="15f85-154">Se não estiver habilitado, um usuário deverá, após a conclusão da revisão, aplicar as decisões manualmente.</span><span class="sxs-lookup"><span data-stu-id="15f85-154">If not enabled, a user must, after the review completes, apply the decisions manually.</span></span>
+ <span data-ttu-id="15f85-155">Aplique **a ação removeAccessApplyAction** a usuários convidados negados.</span><span class="sxs-lookup"><span data-stu-id="15f85-155">Apply **removeAccessApplyAction** action to denied guest users.</span></span> <span data-ttu-id="15f85-156">Isso remove a associação no grupo do convidado negado.</span><span class="sxs-lookup"><span data-stu-id="15f85-156">This removes the membership in the group of the denied guest.</span></span> <span data-ttu-id="15f85-157">O usuário convidado ainda pode entrar no locatário.</span><span class="sxs-lookup"><span data-stu-id="15f85-157">The guest user can still sign in to your tenant.</span></span>

### <a name="request"></a><span data-ttu-id="15f85-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-158">Request</span></span>
<span data-ttu-id="15f85-159">Nesta chamada, substitua o seguinte:</span><span class="sxs-lookup"><span data-stu-id="15f85-159">In this call, replace the following:</span></span>

+ <span data-ttu-id="15f85-160">`c9a5aff7-9298-4d71-adab-0a222e0a05e4` com a **id** do usuário que você está projetando como revistor de backup.</span><span class="sxs-lookup"><span data-stu-id="15f85-160">`c9a5aff7-9298-4d71-adab-0a222e0a05e4` with the **id** of the user you are designating as a backup reviewer.</span></span> <span data-ttu-id="15f85-161">Esta é a **id** da resposta na Etapa 1.</span><span class="sxs-lookup"><span data-stu-id="15f85-161">This is the **id** from the response in Step 1.</span></span>
+ <span data-ttu-id="15f85-162">Valor de **startDate** com a data de hoje e o valor de **endDate** com uma data de um ano a partir da data de início.</span><span class="sxs-lookup"><span data-stu-id="15f85-162">Value of **startDate** with today's date and value of **endDate** with a date one year from the start date.</span></span> 

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

### <a name="response"></a><span data-ttu-id="15f85-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-163">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "c22ae540-b89a-4d24-bac0-4ef35e6591ea",
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "status": "NotStarted",
    "createdBy": {
        "id": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-5-list-instances-of-the-access-review"></a><span data-ttu-id="15f85-164">Etapa 5: Listar instâncias da revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="15f85-164">Step 5: List instances of the access review</span></span>

<span data-ttu-id="15f85-165">A consulta a seguir lista todas as instâncias da definição de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-165">The following query lists all instances of the access review definition.</span></span> <span data-ttu-id="15f85-166">Se o locatário de teste contiver outros grupos do Microsoft 365 com usuários convidados, essa solicitação retornará uma instância para cada grupo do Microsoft 365 com usuários convidados no locatário.</span><span class="sxs-lookup"><span data-stu-id="15f85-166">If your test tenant contains other Microsoft 365 groups with guest users, this request will return one instance for every Microsoft 365 group with guest users in the tenant.</span></span>

### <a name="request"></a><span data-ttu-id="15f85-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-167">Request</span></span>
<span data-ttu-id="15f85-168">Nesta chamada, substitua pela id da definição de revisão de `c22ae540-b89a-4d24-bac0-4ef35e6591ea` acesso retornada na Etapa 4. </span><span class="sxs-lookup"><span data-stu-id="15f85-168">In this call, replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition returned in Step 4.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a><span data-ttu-id="15f85-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-169">Response</span></span>
<span data-ttu-id="15f85-170">Nesta resposta, o escopo inclui um grupo com **id** (o grupo de campanhas de marketing Feelgood criado na Etapa 3) porque tem `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` um usuário convidado. </span><span class="sxs-lookup"><span data-stu-id="15f85-170">In this response, the scope includes a group with **id** `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` (the **Feelgood marketing campaign** group created in Step 3) because it has a guest user.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
    "value": [
        {
            "id": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "startDateTime": "2021-02-10T17:00:36.96Z",
            "endDateTime": "2021-02-10T17:00:36.96Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
<span data-ttu-id="15f85-171">Nesta resposta, a instância de revisão de acesso atualmente é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="15f85-171">In this response, the access review instance is currently `InProgress`.</span></span> <span data-ttu-id="15f85-172">Como essa é uma revisão trimestral, a cada três meses, uma nova instância de revisão é criada automaticamente e você, o revistor, pode aplicar novas decisões.</span><span class="sxs-lookup"><span data-stu-id="15f85-172">Because this is a quarterly review, every 3 months, a new review instance is created automatically and you—the reviewer—can apply new decisions.</span></span>

## <a name="step-6-get-decisions"></a><span data-ttu-id="15f85-173">Etapa 6: Obter decisões</span><span class="sxs-lookup"><span data-stu-id="15f85-173">Step 6: Get decisions</span></span>

<span data-ttu-id="15f85-174">Obter as decisões tomadas para a instância de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-174">Get the decisions taken for the instance of an access review.</span></span>

### <a name="request"></a><span data-ttu-id="15f85-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-175">Request</span></span>
<span data-ttu-id="15f85-176">Nesta chamada:</span><span class="sxs-lookup"><span data-stu-id="15f85-176">In this call:</span></span>
+ <span data-ttu-id="15f85-177">Substitua `c22ae540-b89a-4d24-bac0-4ef35e6591ea` pela **id da definição** de revisão de acesso retornada na Etapa 4.</span><span class="sxs-lookup"><span data-stu-id="15f85-177">Replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition returned in Step 4.</span></span>
+ <span data-ttu-id="15f85-178">Substitua pela id da sua instância de revisão `6392b1a7-9c25-4844-83e5-34e23c88e16a` de acesso retornada na Etapa 5. </span><span class="sxs-lookup"><span data-stu-id="15f85-178">Replace `6392b1a7-9c25-4844-83e5-34e23c88e16a` with the **id** of your access review instance returned in Step 5.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a><span data-ttu-id="15f85-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-179">Response</span></span>

<span data-ttu-id="15f85-180">A resposta a seguir mostra a decisão tomada para a instância da revisão.</span><span class="sxs-lookup"><span data-stu-id="15f85-180">The following response shows the decision taken for the instance of the review.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "0e76ee07-b4c6-469e-bc9d-e73fc9a8d660",
            "accessReviewId": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "reviewedDateTime": "2021-02-10T17:06:26.147Z",
            "decision": "Approve",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "AAD Access Reviews",
                "userPrincipalName": "AAD Access Reviews"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "userDisplayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "displayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            }
        }
    ]
}
```

<span data-ttu-id="15f85-181">Como esta é uma revisão trimestral e enquanto a definição ainda estiver ativa, ou seja, a recorrência **endDate** não é uma data passada, a cada três meses, quando uma nova instância de revisão é criada, você como o revistor pode aplicar novas decisões.</span><span class="sxs-lookup"><span data-stu-id="15f85-181">Because this is a quarterly review and as long as the definition is still active, that is, the recurrence **endDate** is not a past date, every 3 months when a new review instance is created, you as the reviewer can apply new decisions.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="15f85-182">Etapa 7: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="15f85-182">Step 7: Clean up resources</span></span>

<span data-ttu-id="15f85-183">Exclua os recursos criados para este tutorial: grupo de campanhas de **marketing feelgood,** definição de agenda de revisão de acesso, usuário convidado e usuário de teste.</span><span class="sxs-lookup"><span data-stu-id="15f85-183">Delete the resources that you created for this tutorial—**Feelgood marketing campaign** group, the access review schedule definition, the guest user, and the test user.</span></span>

### <a name="delete-the-microsoft-365-group"></a><span data-ttu-id="15f85-184">Excluir o grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15f85-184">Delete the Microsoft 365 group</span></span>

#### <a name="request"></a><span data-ttu-id="15f85-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-185">Request</span></span>
<span data-ttu-id="15f85-186">Nesta chamada, substitua pela id da campanha `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **de marketing do Feelgood do** Microsoft 365. </span><span class="sxs-lookup"><span data-stu-id="15f85-186">In this call, replace `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` with the **id** of your **Feelgood marketing campaign** Microsoft 365 group.</span></span>

```http
DELETE https://graph.microsoft.com/beta/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a><span data-ttu-id="15f85-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-187">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a><span data-ttu-id="15f85-188">Excluir a definição de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="15f85-188">Delete the access review definition</span></span>

<span data-ttu-id="15f85-189">Nesta chamada, substitua pela id da `c22ae540-b89a-4d24-bac0-4ef35e6591ea` **sua definição** de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-189">In this call, replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition.</span></span> <span data-ttu-id="15f85-190">Como a definição de agenda de revisão de acesso é o modelo para a revisão de acesso, excluir a definição removerá as configurações, instâncias e decisões associadas à revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-190">Since the access review schedule definition is the blueprint for the access review, deleting the definition will remove the settings, instances, and decisions associated with the access review.</span></span>

#### <a name="request"></a><span data-ttu-id="15f85-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-191">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a><span data-ttu-id="15f85-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-192">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```
### <a name="remove-the-guest-user"></a><span data-ttu-id="15f85-193">Remover o usuário convidado</span><span class="sxs-lookup"><span data-stu-id="15f85-193">Remove the guest user</span></span>

<span data-ttu-id="15f85-194">Nesta chamada, substitua `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` pela **id** do usuário convidado, john@tailspintoys.com.</span><span class="sxs-lookup"><span data-stu-id="15f85-194">In this call, replace `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` with the **id** of the guest user, john@tailspintoys.com.</span></span>

#### <a name="request"></a><span data-ttu-id="15f85-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-195">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a><span data-ttu-id="15f85-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-196">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a><span data-ttu-id="15f85-197">Excluir o usuário de teste</span><span class="sxs-lookup"><span data-stu-id="15f85-197">Delete the test user</span></span>

#### <a name="request"></a><span data-ttu-id="15f85-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f85-198">Request</span></span>
<span data-ttu-id="15f85-199">Nesta chamada, substitua `c9a5aff7-9298-4d71-adab-0a222e0a05e4` pela **id do** usuário de teste.</span><span class="sxs-lookup"><span data-stu-id="15f85-199">In this call, replace `c9a5aff7-9298-4d71-adab-0a222e0a05e4` with the **id** of your test user.</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a><span data-ttu-id="15f85-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f85-200">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

<span data-ttu-id="15f85-201">Parabéns!</span><span class="sxs-lookup"><span data-stu-id="15f85-201">Congratulations!</span></span> <span data-ttu-id="15f85-202">Você criou uma revisão de acesso para todos os usuários convidados nos grupos do Microsoft 365 em seu locatário e agendou trimestralmente para a avaliação e atestado do acesso dos usuários convidados.</span><span class="sxs-lookup"><span data-stu-id="15f85-202">You have created an access review for all guest users in Microsoft 365 groups in your tenant, and scheduled quarterly for the evaluation and attestation of the guest users' access.</span></span> <span data-ttu-id="15f85-203">Os proprietários do grupo revisarão o acesso durante esses ciclos, escolhendo aprovar ou negar o acesso.</span><span class="sxs-lookup"><span data-stu-id="15f85-203">The group owners will review access during these cycles, choosing either to approve or deny access.</span></span>

## <a name="see-also"></a><span data-ttu-id="15f85-204">Confira também</span><span class="sxs-lookup"><span data-stu-id="15f85-204">See also</span></span>

+ [<span data-ttu-id="15f85-205">Visão geral de avaliações do Access e requisitos de licença</span><span class="sxs-lookup"><span data-stu-id="15f85-205">Access Reviews overview and license requirements</span></span>](/azure/active-directory/governance/access-reviews-overview)
+ [<span data-ttu-id="15f85-206">Cenários de licença do Access Reviews</span><span class="sxs-lookup"><span data-stu-id="15f85-206">Access Reviews license scenarios</span></span>](/azure/active-directory/governance/access-reviews-overview#example-license-scenarios)
+ [<span data-ttu-id="15f85-207">Criar uma revisão de acesso de grupos & aplicativos</span><span class="sxs-lookup"><span data-stu-id="15f85-207">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)
+ [<span data-ttu-id="15f85-208">Convidar/adicionar usuários convidados à sua organização</span><span class="sxs-lookup"><span data-stu-id="15f85-208">Invite/add guest users to your organization</span></span>](/graph/api/resources/invitation?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="15f85-209">Referência da API de Avaliações do Access</span><span class="sxs-lookup"><span data-stu-id="15f85-209">Access Reviews API Reference</span></span>](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="15f85-210">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="15f85-210">Create accessReviewScheduleDefinition</span></span>](/graph/api/accessreviewscheduledefinition-create?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="15f85-211">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="15f85-211">List accessReviewInstance</span></span>](/graph/api/accessreviewinstance-list?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="15f85-212">Listar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="15f85-212">List accessReviewInstanceDecisionItem</span></span>](/graph/api/accessreviewinstancedecisionitem-list?view=graph-rest-beta&preserve-view=true)

