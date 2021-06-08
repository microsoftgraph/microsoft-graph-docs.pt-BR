---
title: 'Tutorial: use a API de críticas de acesso para revisar o acesso aos seus grupos de segurança'
description: Usar a API de avaliações de acesso para revisar o acesso aos seus grupos de segurança
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: b3a7ee94f045eb7eb587b58fc6220c304c2b81ff
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787074"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a><span data-ttu-id="a9092-103">Tutorial: use a API de críticas de acesso para revisar o acesso aos seus grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="a9092-103">Tutorial: Use the access reviews API to review access to your security groups</span></span>

<span data-ttu-id="a9092-104">Neste tutorial, você usará o Graph Explorer para revisar o acesso a um grupo de segurança em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a9092-104">In this tutorial, you will use Graph Explorer to review access to a security group in your tenant.</span></span>

<span data-ttu-id="a9092-105">Você pode usar Graph Explorer ou Postman para testar e testar suas chamadas de API de críticas de acesso antes de automatize-las em um script ou em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9092-105">You can use Graph Explorer or Postman to try out and test your access reviews API calls before you automate them into a script or an app.</span></span> <span data-ttu-id="a9092-106">Isso economiza tempo ajudando você a definir e validar corretamente suas consultas sem recompilar repetidamente seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9092-106">This saves you time by helping you properly define and validate your queries without repeatedly recompiling your application.</span></span>

>[!NOTE]
><span data-ttu-id="a9092-107">Os objetos de resposta mostrados neste tutorial podem ser reduzidos para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="a9092-107">The response objects shown in this tutorial might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9092-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9092-108">Prerequisites</span></span>

<span data-ttu-id="a9092-109">Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:</span><span class="sxs-lookup"><span data-stu-id="a9092-109">To complete this tutorial, you need the following resources and privileges:</span></span>

+ <span data-ttu-id="a9092-110">Um locatário do Azure AD funcionando com uma licença do Azure AD Premium P2 ou EMS E5 habilitada.</span><span class="sxs-lookup"><span data-stu-id="a9092-110">A working Azure AD tenant with an Azure AD Premium P2 or EMS E5 license enabled.</span></span>
+ <span data-ttu-id="a9092-111">Entre no Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) como usuário em uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="a9092-111">Log in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) as a user in a global administrator role.</span></span>
  + <span data-ttu-id="a9092-112">[Opcional] Inicie uma nova **sessão de navegador incógnita** ou **InPrivate** ou inicie uma sessão em um navegador anônimo.</span><span class="sxs-lookup"><span data-stu-id="a9092-112">[Optional] Start a new **incognito** or **InPrivate browser** session or start a session in an anonymous browser.</span></span> <span data-ttu-id="a9092-113">Você fará logoff mais adiante neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="a9092-113">You will log in later in this tutorial.</span></span>
+ <span data-ttu-id="a9092-114">As seguintes permissões delegadas: `AccessReview.ReadWrite.All` , `Group.ReadWrite.All` .</span><span class="sxs-lookup"><span data-stu-id="a9092-114">The following delegated permissions: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.</span></span>

<span data-ttu-id="a9092-115">Para consentir com as permissões necessárias no Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="a9092-115">To consent to the required permissions in Graph Explorer:</span></span>
1. <span data-ttu-id="a9092-116">Selecione o ícone de engrenagem de configurações à direita dos detalhes da conta do usuário e selecione **Selecionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="a9092-116">Select the settings gear icon to the right of the user account details, and then select **Select permissions**.</span></span>
   
   <span data-ttu-id="a9092-117">![Selecionar as permissões do Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   </span><span class="sxs-lookup"><span data-stu-id="a9092-117">![Select the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. <span data-ttu-id="a9092-118">Role a lista de permissões para essas permissões:</span><span class="sxs-lookup"><span data-stu-id="a9092-118">Scroll through the list of permissions to these permissions:</span></span>
   + <span data-ttu-id="a9092-119">AccessReviews (3), expanda e selecione **AccessReviews.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="a9092-119">AccessReviews (3), expand and then select **AccessReviews.ReadWrite.All**.</span></span>
   + <span data-ttu-id="a9092-120">Grupo (2), expanda e selecione **Group.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="a9092-120">Group (2), expand and then select **Group.ReadWrite.All**.</span></span>
  
    <span data-ttu-id="a9092-121">Selecione **Consentimento** e, na janela pop, escolha **Consentir** em  nome da sua organização e selecione Aceitar para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="a9092-121">Select **Consent**, and in the pop window, choose to **Consent on behalf of your organization** and then select **Accept** to accept the consent of the permissions.</span></span>
   
   <span data-ttu-id="a9092-122">![Consentir com as permissões Graph Microsoft](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
   </span><span class="sxs-lookup"><span data-stu-id="a9092-122">![Consent to the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-test-users-in-your-tenant"></a><span data-ttu-id="a9092-123">Etapa 1: Criar usuários de teste em seu locatário</span><span class="sxs-lookup"><span data-stu-id="a9092-123">Step 1: Create test users in your tenant</span></span>

<span data-ttu-id="a9092-124">Crie três novos usuários de teste executando a solicitação abaixo de três vezes, alterando as propriedades **displayName,** **mailNickname** e **userPrincipalName** sempre.</span><span class="sxs-lookup"><span data-stu-id="a9092-124">Create three new test users by running the request below three times, changing the **displayName**, **mailNickname**, and **userPrincipalName** properties each time.</span></span> <span data-ttu-id="a9092-125">Grave suas **IDs.**</span><span class="sxs-lookup"><span data-stu-id="a9092-125">Record their **id** s.</span></span>

### <a name="request"></a><span data-ttu-id="a9092-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-126">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-createUser"
}-->
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

### <a name="response"></a><span data-ttu-id="a9092-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-127">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a><span data-ttu-id="a9092-128">Etapa 2: criar um grupo de segurança, atribuir proprietários e adicionar membros</span><span class="sxs-lookup"><span data-stu-id="a9092-128">Step 2: Create a security group, assign owners, and add members</span></span>

<span data-ttu-id="a9092-129">Crie um grupo de segurança chamado **Criando** um grupo de segurança que é o destino das análises de acesso neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="a9092-129">Create a security group named **Building security group** that is the target of the access reviews in this tutorial.</span></span> <span data-ttu-id="a9092-130">Atribua a esse grupo dois proprietários de grupo e dois membros.</span><span class="sxs-lookup"><span data-stu-id="a9092-130">Assign to this group two group owners and two members.</span></span> <span data-ttu-id="a9092-131">Esses membros serão objeto de revisão pelos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-131">These members will be the subject of review by the group owners.</span></span>

### <a name="request"></a><span data-ttu-id="a9092-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-132">Request</span></span>

<span data-ttu-id="a9092-133">Nesta chamada, substitua:</span><span class="sxs-lookup"><span data-stu-id="a9092-133">In this call, replace:</span></span>
+ <span data-ttu-id="a9092-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` e `b828cc0e-4240-46ed-bb25-888744487e2d` com **a id** s de seus dois proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` and `b828cc0e-4240-46ed-bb25-888744487e2d` with the **id** s of your two group owners.</span></span>
  + <span data-ttu-id="a9092-135">Um dos **IDs** pertence a um dos usuários que você criou na Etapa 1.</span><span class="sxs-lookup"><span data-stu-id="a9092-135">One of the **id** s belongs to one of the users you created in Step 1.</span></span>
  + <span data-ttu-id="a9092-136">A outra é sua **id.** Para recuperar sua **id,** execute `GET` em `https://graph.microsoft.com/beta/me` .</span><span class="sxs-lookup"><span data-stu-id="a9092-136">The other is your **id**. To retrieve your **id**, run `GET` on `https://graph.microsoft.com/beta/me`.</span></span>
+ <span data-ttu-id="a9092-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab` e `859924d0-7115-422a-9ee8-ea8c0c014707` com **as IDs** de vocês dois membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab` and `859924d0-7115-422a-9ee8-ea8c0c014707` with the **id** s of you two group members.</span></span> <span data-ttu-id="a9092-138">Esses são os outros dois membros criados na Etapa 1.</span><span class="sxs-lookup"><span data-stu-id="a9092-138">These are the other two members you created in Step 1.</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-creategroup"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Building security group",
    "displayName": "Building security group",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/010b2de0-0ed4-4ece-bfa2-22fff71d0497",
        "https://graph.microsoft.com/beta/users/b828cc0e-4240-46ed-bb25-888744487e2d"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab",
        "https://graph.microsoft.com/beta/users/859924d0-7115-422a-9ee8-ea8c0c014707"
    ]
}
```

### <a name="response"></a><span data-ttu-id="a9092-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "825f1b5e-6fb2-4d9a-b393-d491101acc0c",
    "displayName": "Building security group",
    "groupTypes": []
}
```
<span data-ttu-id="a9092-140">Na resposta, grave a **id** do novo grupo para usá-lo posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="a9092-140">From the response, record the **id** of the new group to use it later in this tutorial.</span></span>

## <a name="step-3-create-an-access-review-for-the-security-group"></a><span data-ttu-id="a9092-141">Etapa 3: Criar uma revisão de acesso para o grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="a9092-141">Step 3: Create an access review for the security group</span></span>

<span data-ttu-id="a9092-142">Crie uma revisão de acesso para membros do grupo de segurança, usando as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="a9092-142">Create an access review for members of the security group, using the following settings:</span></span>
+ <span data-ttu-id="a9092-143">É uma revisão de acesso de autoavaliação.</span><span class="sxs-lookup"><span data-stu-id="a9092-143">It is a self-reviewing access review.</span></span> <span data-ttu-id="a9092-144">Nesse caso, os usuários sob revisão autotestam a necessidade de acesso ao grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-144">In this case, users under review will self-attest to their need for access to the group.</span></span>
+ <span data-ttu-id="a9092-145">Esta é uma revisão de acesso único.</span><span class="sxs-lookup"><span data-stu-id="a9092-145">This is a one-time access review.</span></span> <span data-ttu-id="a9092-146">Nesse caso, depois que o acesso for concedido, o usuário não precisará fazer o autoteste novamente dentro do período de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-146">In this case, once access is granted, the user does not need to self-attest again within the access review period.</span></span>
+ <span data-ttu-id="a9092-147">O escopo de revisão é limitado a membros do **grupo de segurança de criação.**</span><span class="sxs-lookup"><span data-stu-id="a9092-147">The review scope is limited to members of **Building security group**.</span></span>

### <a name="request"></a><span data-ttu-id="a9092-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-148">Request</span></span>

<span data-ttu-id="a9092-149">Nesta chamada, substitua o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a9092-149">In this call, replace the following:</span></span>
+ <span data-ttu-id="a9092-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c` com a **id de** **Criar grupo de segurança**.</span><span class="sxs-lookup"><span data-stu-id="a9092-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>
+ <span data-ttu-id="a9092-151">O escopo especifica que a revisão é aplicada a todos os membros do grupo de segurança do **Building.**</span><span class="sxs-lookup"><span data-stu-id="a9092-151">The scope specifies that the review is applied to all group members of the the **Building security group**.</span></span> <span data-ttu-id="a9092-152">Para obter mais opções para configurar o escopo, consulte a [seção Consulte também.](#see-also)</span><span class="sxs-lookup"><span data-stu-id="a9092-152">For more options for configuring the scope, see the [See also](#see-also) section.</span></span>
+ <span data-ttu-id="a9092-153">Valor de **startDate** com a data de hoje e o valor de **endDate** com uma data de um ano a partir da data de início.</span><span class="sxs-lookup"><span data-stu-id="a9092-153">Value of **startDate** with today's date and value of **endDate** with a date one year from the start date.</span></span>

<span data-ttu-id="a9092-154">Ao não especificar o valor da propriedade **reviewers,** essa revisão de acesso é configurada como auto-revisão com os membros como revistores.</span><span class="sxs-lookup"><span data-stu-id="a9092-154">By failing to specify the value of the **reviewers** property, this access review is configured as self-reviewing with the members as the reviewers.</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security group",
    "descriptionForAdmins": "One-time self-review for members of Building security group",
    "descriptionForReviewers": "One-time self-review for members of Building security group",
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
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

### <a name="response"></a><span data-ttu-id="a9092-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-155">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "d7286a17-3a01-406a-b872-986b6b40317c",
    "displayName": "One-time self-review for members of Building security group",
    "status": "NotStarted",
    "createdBy": {
        "id": "b828cc0e-4240-46ed-bb25-888744487e2d",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "backupReviewers": [],
    "settings": {
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
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

## <a name="step-4-list-instances-of-the-access-review"></a><span data-ttu-id="a9092-156">Etapa 4: Listar instâncias da revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="a9092-156">Step 4: List instances of the access review</span></span>

<span data-ttu-id="a9092-157">A consulta a seguir lista todas as instâncias da definição de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-157">The following query lists all instances of the access review definition.</span></span> <span data-ttu-id="a9092-158">Como você criou uma revisão de acesso único na Etapa 3, a solicitação retorna apenas uma instância cuja **id** é a mesma que a id da definição de **acesso.**</span><span class="sxs-lookup"><span data-stu-id="a9092-158">Because you created a one-time access review in Step 3, the request returns only one instance whose **id** is the same as the access definition’s **id**.</span></span>

### <a name="request"></a><span data-ttu-id="a9092-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-159">Request</span></span>

<span data-ttu-id="a9092-160">Nesta chamada, substitua pela id da definição de revisão de `d7286a17-3a01-406a-b872-986b6b40317c` acesso retornada na Etapa 3. </span><span class="sxs-lookup"><span data-stu-id="a9092-160">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances
```

### <a name="response"></a><span data-ttu-id="a9092-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-161">Response</span></span>

<span data-ttu-id="a9092-162">Nesta resposta, o **status** da instância de revisão de acesso é porque `InProgress` **startDateTime** é passado e **endDateTime** está no futuro.</span><span class="sxs-lookup"><span data-stu-id="a9092-162">In this response, the **status** of the access review instance is `InProgress` because **startDateTime** is past and **endDateTime** is in the future.</span></span> <span data-ttu-id="a9092-163">Se **startDateTime** estiver no futuro, o status será `NotStarted` .</span><span class="sxs-lookup"><span data-stu-id="a9092-163">If **startDateTime** is in the future, the status will be `NotStarted`.</span></span> <span data-ttu-id="a9092-164">Por outro lado, se **endDateTime** estiver no passado, o status será `Completed` .</span><span class="sxs-lookup"><span data-stu-id="a9092-164">On the other hand, if **endDateTime** is in the past, the status will be `Completed`.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances",
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="step-5-get-decisions"></a><span data-ttu-id="a9092-165">Etapa 5: Obter decisões</span><span class="sxs-lookup"><span data-stu-id="a9092-165">Step 5: Get decisions</span></span>

<span data-ttu-id="a9092-166">Você está interessado nas decisões tomadas para a instância da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-166">You are interested in the decisions taken for the instance of the access review.</span></span>

### <a name="request"></a><span data-ttu-id="a9092-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-167">Request</span></span>

<span data-ttu-id="a9092-168">Nesta chamada, substitua pela id da definição de revisão de `d7286a17-3a01-406a-b872-986b6b40317c` acesso retornada na Etapa 3. </span><span class="sxs-lookup"><span data-stu-id="a9092-168">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances/d7286a17-3a01-406a-b872-986b6b40317c/decisions
```

### <a name="response"></a><span data-ttu-id="a9092-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-169">Response</span></span>

<span data-ttu-id="a9092-170">A resposta a seguir mostra a decisão tomada para a instância da revisão.</span><span class="sxs-lookup"><span data-stu-id="a9092-170">The following response shows the decision taken for the instance of the review.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances('d7286a17-3a01-406a-b872-986b6b40317c')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "1c74f500-9082-4dfe-80ac-784a6edb71d7",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        },
        {
            "id": "7744be81-7d17-40c9-8fd3-c9072b1ccace",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "userDisplayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "displayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            }
        }
    ]
}
```

<span data-ttu-id="a9092-171">Na chamada, a **propriedade decision** tem o valor de `NotReviewed` .</span><span class="sxs-lookup"><span data-stu-id="a9092-171">From the call, the **decision** property has the value of `NotReviewed`.</span></span> <span data-ttu-id="a9092-172">Isso porque nenhum dos dois membros concluiu seu autoteste.</span><span class="sxs-lookup"><span data-stu-id="a9092-172">This is because none of the two members has completed their self-attestation.</span></span> <span data-ttu-id="a9092-173">Siga a etapa 6 para saber como cada membro pode autotestar sua necessidade de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-173">Follow step 6 to learn how each member can self-attest to their need for access review.</span></span>

## <a name="step-6-self-review-your-pending-access"></a><span data-ttu-id="a9092-174">Etapa 6: revisar seu acesso pendente</span><span class="sxs-lookup"><span data-stu-id="a9092-174">Step 6: Self-review your pending access</span></span>

<span data-ttu-id="a9092-175">Na Etapa 3, você configurou a revisão de acesso como uma autoavaliação.</span><span class="sxs-lookup"><span data-stu-id="a9092-175">In Step 3, you configured the access review as a self-reviewing.</span></span> <span data-ttu-id="a9092-176">Isso significa que ambos os membros do **Grupo de** Segurança de Criação devem autotestar a necessidade de manter o acesso ao grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-176">This means that both members of **Building security group** must self-attest to their need to maintain access to the group.</span></span> <span data-ttu-id="a9092-177">Você concluirá esta etapa como um dos dois membros do grupo de segurança do Building.</span><span class="sxs-lookup"><span data-stu-id="a9092-177">You will complete this step as one of the two members of Building security group.</span></span>

<span data-ttu-id="a9092-178">In this step, you will:</span><span class="sxs-lookup"><span data-stu-id="a9092-178">In this step, you will:</span></span>
1. <span data-ttu-id="a9092-179">Listar suas instâncias de revisão de acesso pendentes.</span><span class="sxs-lookup"><span data-stu-id="a9092-179">List your pending access review instances.</span></span>
2. <span data-ttu-id="a9092-180">Conclua o processo de autoteste de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-180">Complete the access review self-attestation process.</span></span>

<span data-ttu-id="a9092-181">Inicie uma nova sessão de navegador no modo de navegação **incógnito** ou **InPrivate** ou por meio de um navegador anônimo e faça logon como um dos dois membros do grupo de segurança **de Criação.**</span><span class="sxs-lookup"><span data-stu-id="a9092-181">Start a new browser session in **incognito** or **InPrivate browsing** mode, or via an anonymous browser, and log in as one of the two members of **Building security group**.</span></span> <span data-ttu-id="a9092-182">Ao fazer isso, você não interromperá sua sessão atual como usuário na função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="a9092-182">By doing so, you will not interrupt your current session as a user in the global administrator role.</span></span> <span data-ttu-id="a9092-183">Como alternativa, você pode interromper sua sessão atual fazendo logon no Graph Explorer e fazendo logon de volta como um dos dois membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9092-183">Alternatively, you can interrupt your current session by logging out of Graph Explorer and logging back in as one of the two group members.</span></span>

### <a name="list-your-pending-access-review-instances"></a><span data-ttu-id="a9092-184">Listar suas instâncias de revisão de acesso pendentes</span><span class="sxs-lookup"><span data-stu-id="a9092-184">List your pending access review instances</span></span>

<span data-ttu-id="a9092-185">Na sessão de navegador incógnito e no Graph Explorer, execute a seguinte consulta para listar suas instâncias de revisão de acesso pendentes:</span><span class="sxs-lookup"><span data-stu-id="a9092-185">In the incognito browser session and in Graph Explorer, run the following query to list your pending access review instances:</span></span>

#### <a name="request"></a><span data-ttu-id="a9092-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-186">Request</span></span>

```http
GET /me/pendingAccessReviewInstances
```

#### <a name="response"></a><span data-ttu-id="a9092-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-187">Response</span></span>
<span data-ttu-id="a9092-188">Na resposta abaixo, o usuário Alex Wilber da **id** tem 1 revisão de acesso pendente para `43b12b0c-ee2c-4257-96fe-505d823e06ab` autoteste.</span><span class="sxs-lookup"><span data-stu-id="a9092-188">From the response below, user Alex Wilber of **id** `43b12b0c-ee2c-4257-96fe-505d823e06ab` has 1 pending access review to self-attest to.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('43b12b0c-ee2c-4257-96fe-505d823e06ab')/pendingAccessReviewInstances",
    "@odata.count": 1,
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
<span data-ttu-id="a9092-189">O uso da `/me/pendingAccessReviewInstances` chamada em um contexto de usuário tem várias vantagens:</span><span class="sxs-lookup"><span data-stu-id="a9092-189">Using the call `/me/pendingAccessReviewInstances` in a user context has a number of advantages:</span></span>
+ <span data-ttu-id="a9092-190">Nenhuma entidade de serviço é necessária.</span><span class="sxs-lookup"><span data-stu-id="a9092-190">No service principal is required.</span></span> <span data-ttu-id="a9092-191">Um usuário pode chamar e ler suas ações pendentes de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-191">A user can call and read their pending access review actions.</span></span>
+ <span data-ttu-id="a9092-192">Pode ser usado por widgets ou plug-ins em uma página da Intranet, ou um bot ou daemon que são executados como um serviço em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="a9092-192">Can be used by widgets or plugins on an Intranet page, or a bot or daemon that run as a background service.</span></span> <span data-ttu-id="a9092-193">Eles podem notificá-lo sobre novas avaliações de acesso ou de atualizações para acessar avaliações.</span><span class="sxs-lookup"><span data-stu-id="a9092-193">These can notify you of new access reviews or of updates to access reviews.</span></span> 

### <a name="complete-the-access-review-self-attestation"></a><span data-ttu-id="a9092-194">Concluir o autoteste de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="a9092-194">Complete the access review self-attestation</span></span>

<span data-ttu-id="a9092-195">Na mesma sessão de navegador incógnito, faça logon para https://myaccess.microsoft.com/ concluir o autoteste.</span><span class="sxs-lookup"><span data-stu-id="a9092-195">In the same incognito browser session, log in to https://myaccess.microsoft.com/ to complete the self-attestation.</span></span> <span data-ttu-id="a9092-196">Na barra de navegação direita, selecione **críticas de acesso e** escolha sua revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-196">From the right navigation bar, select **access reviews** and choose your access review.</span></span> <span data-ttu-id="a9092-197">Selecione **Sim**, que você ainda precisa acessar a Criação de grupo **de segurança**, insira um motivo e clique em **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="a9092-197">Select **Yes**, that you still need access to **Building security group**, enter a reason, then click **Submit**.</span></span>

   <span data-ttu-id="a9092-198">![Autoteste para acessar revisão](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span><span class="sxs-lookup"><span data-stu-id="a9092-198">![Self-attest to access review](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Self-attest to access review":::-->

<span data-ttu-id="a9092-199">Agora você pode fazer logout e sair da sessão do navegador anônimo.</span><span class="sxs-lookup"><span data-stu-id="a9092-199">You can now logout and exit the incognito browser session.</span></span>

<span data-ttu-id="a9092-200">De volta à sessão principal do navegador onde você ainda está conectado como o  usuário de administrador global, repita a Etapa 4 para ver se a propriedade de decisão do membro que concluiu a etapa 5 agora é `Approve` .</span><span class="sxs-lookup"><span data-stu-id="a9092-200">Back in the main browser session where you are still logged in as the global administrator user, repeat Step 4 to see that the **decision** property for the member who completed step 5 is now `Approve`.</span></span>

<span data-ttu-id="a9092-201">Parabéns!</span><span class="sxs-lookup"><span data-stu-id="a9092-201">Congratulations!</span></span> <span data-ttu-id="a9092-202">Você criou uma revisão de acesso e autotestou a necessidade de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-202">You have created an access review and self-attested to the need for access.</span></span> <span data-ttu-id="a9092-203">Você só faz isso uma vez e mantém o acesso até quando a definição de revisão de acesso expirar.</span><span class="sxs-lookup"><span data-stu-id="a9092-203">You only do this once, and maintain access until when the access review definition expires.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="a9092-204">Etapa 7: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="a9092-204">Step 7: Clean up resources</span></span>

<span data-ttu-id="a9092-205">Exclua os recursos criados para este tutorial: Criar grupo **de segurança,** a definição do agendamento de revisão de acesso e os três usuários de teste..</span><span class="sxs-lookup"><span data-stu-id="a9092-205">Delete the resources that you created for this tutorial—**Building security group**, the access review schedule definition, and the three test users..</span></span>

### <a name="delete-the-security-group"></a><span data-ttu-id="a9092-206">Excluir o grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="a9092-206">Delete the security group</span></span>

#### <a name="request"></a><span data-ttu-id="a9092-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-207">Request</span></span>

<span data-ttu-id="a9092-208">Nesta chamada, substitua `825f1b5e-6fb2-4d9a-b393-d491101acc0c` pela **id** do grupo de segurança **de criação.**</span><span class="sxs-lookup"><span data-stu-id="a9092-208">In this call, replace `825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c
```

#### <a name="response"></a><span data-ttu-id="a9092-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-209">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a><span data-ttu-id="a9092-210">Excluir a definição de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="a9092-210">Delete the access review definition</span></span>

<span data-ttu-id="a9092-211">Nesta chamada, substitua pela id da `d7286a17-3a01-406a-b872-986b6b40317c` **sua definição** de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-211">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition.</span></span> <span data-ttu-id="a9092-212">Como a definição de agenda de revisão de acesso é o modelo para a revisão de acesso, excluir a definição removerá as configurações, instâncias e decisões associadas à revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9092-212">Since the access review schedule definition is the blueprint for the access review, deleting the definition will remove the settings, instances, and decisions associated with the access review.</span></span>

#### <a name="request"></a><span data-ttu-id="a9092-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-213">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c
```

#### <a name="response"></a><span data-ttu-id="a9092-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-214">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-three-test-users"></a><span data-ttu-id="a9092-215">Excluir os três usuários de teste</span><span class="sxs-lookup"><span data-stu-id="a9092-215">Delete the three test users</span></span>
<span data-ttu-id="a9092-216">Nesta chamada, substitua `43b12b0c-ee2c-4257-96fe-505d823e06ab` pela **id do** usuário de teste.</span><span class="sxs-lookup"><span data-stu-id="a9092-216">In this call, replace `43b12b0c-ee2c-4257-96fe-505d823e06ab` with the **id** of your test user.</span></span> <span data-ttu-id="a9092-217">Repita isso duas vezes **com a id** s dos outros dois usuários para excluí-los.</span><span class="sxs-lookup"><span data-stu-id="a9092-217">Repeat this twice with the **id** s of the other two users to delete them.</span></span>

#### <a name="request"></a><span data-ttu-id="a9092-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9092-218">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab
```

#### <a name="response"></a><span data-ttu-id="a9092-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9092-219">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```


## <a name="see-also"></a><span data-ttu-id="a9092-220">Confira também</span><span class="sxs-lookup"><span data-stu-id="a9092-220">See also</span></span>

+ [<span data-ttu-id="a9092-221">Referência da API de avaliações do Access</span><span class="sxs-lookup"><span data-stu-id="a9092-221">Access reviews API Reference</span></span>](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="a9092-222">Configurar o escopo de sua definição de revisão de acesso usando a API Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="a9092-222">Configure the scope of your access review definition using the Microsoft Graph API</span></span>](/graph/accessreviews-scope-concept)
+ [<span data-ttu-id="a9092-223">Visão geral de avaliações do Access e requisitos de licença</span><span class="sxs-lookup"><span data-stu-id="a9092-223">Access reviews overview and license requirements</span></span>](/azure/active-directory/governance/access-reviews-overview)
+ [<span data-ttu-id="a9092-224">Criar uma revisão de acesso de grupos & aplicativos</span><span class="sxs-lookup"><span data-stu-id="a9092-224">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)

