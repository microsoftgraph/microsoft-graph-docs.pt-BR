---
title: Introdução à API dos métodos de autenticação do Microsoft Graph
description: A API dos métodos de autenticação do Microsoft Graph oferece às organizações a capacidade de gerenciar programaticamente os métodos de autenticação dos usuários, registrando os usuários para autenticação multifator (MFA) e redefinição de senha de autoatendimento (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36385345141daa8dc782b64fa154ef97c46b3091
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761448"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="6d9db-103">Introdução à API dos métodos de autenticação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6d9db-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="6d9db-104">Os [métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são como os usuários se autenticam no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6d9db-104">[Authentication methods](/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6d9db-105">Os métodos de autenticação do Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que hoje são gerenciáveis no Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="6d9db-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="6d9db-106">Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="6d9db-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="6d9db-107">Também é possível usar as APIs do método de autenticação para gerenciar os métodos de autenticação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6d9db-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="6d9db-108">Por exemplo, você pode:</span><span class="sxs-lookup"><span data-stu-id="6d9db-108">For example, you can:</span></span>

* <span data-ttu-id="6d9db-109">Adicionar um número de telefone para um usuário, que pode usar esse número para SMS e autenticação de chamada de voz, se estiverem habilitados para o uso pela política</span><span class="sxs-lookup"><span data-stu-id="6d9db-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="6d9db-110">Atualizar ou excluir o número de telefone atribuído a um usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="6d9db-111">Habilitar ou desabilitar o número para entrada de SMS</span><span class="sxs-lookup"><span data-stu-id="6d9db-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="6d9db-112">Redefinir a senha de um usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-112">Reset a user's password</span></span>

<span data-ttu-id="6d9db-113">As APIs são uma ferramenta fundamental para gerenciar os métodos de autenticação dos usuários.</span><span class="sxs-lookup"><span data-stu-id="6d9db-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="6d9db-114">Neste tutorial, você aprenderá a:</span><span class="sxs-lookup"><span data-stu-id="6d9db-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="6d9db-115">Autenticar-se no Azure AD com as funções e permissões certas</span><span class="sxs-lookup"><span data-stu-id="6d9db-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="6d9db-116">Verificar os métodos de autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="6d9db-117">Adicionar novos números de telefone para o usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="6d9db-118">Remover um número de telefone do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="6d9db-119">Redefinir a senha do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="6d9db-120">Etapa 1: Autenticar-se no Azure AD com as funções e permissões certas</span><span class="sxs-lookup"><span data-stu-id="6d9db-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="6d9db-121">Usando sua [ferramenta favorita para interagir com o Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), entre usando uma conta com uma destas funções:</span><span class="sxs-lookup"><span data-stu-id="6d9db-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="6d9db-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6d9db-122">Global administrator</span></span>
* <span data-ttu-id="6d9db-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="6d9db-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="6d9db-124">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="6d9db-124">Authentication administrator</span></span>

<span data-ttu-id="6d9db-125">Em seguida, modifique suas permissões.</span><span class="sxs-lookup"><span data-stu-id="6d9db-125">Next, modify your permissions.</span></span> <span data-ttu-id="6d9db-126">Usaremos o [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) para este tutorial, portanto, verifique se ele está habilitado no Graph Explorer ou no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d9db-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="6d9db-127">Comece a usar a API após o escopo ser atribuído e aprovado.</span><span class="sxs-lookup"><span data-stu-id="6d9db-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="6d9db-128">Os exemplos aqui usam um usuário padrão chamado de Avery Howard.</span><span class="sxs-lookup"><span data-stu-id="6d9db-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="6d9db-129">Use uma conta de teste preexistente ou crie uma nova seguindo [estas instruções](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span><span class="sxs-lookup"><span data-stu-id="6d9db-129">You should use a preexisting test account or create a new one following [these instructions](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="6d9db-130">Essas APIs estão ativas, portanto não as testem em usuários reais.</span><span class="sxs-lookup"><span data-stu-id="6d9db-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="6d9db-131">Etapa 2: Verificar os métodos de autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="6d9db-132">Faça uma chamada para verificar os métodos de autenticação do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d9db-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="6d9db-133">Pegue a URL para ver o perfil de um usuário e adicione `/authentication/methods`:</span><span class="sxs-lookup"><span data-stu-id="6d9db-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="6d9db-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-135">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="6d9db-136">Etapa 3: Adicionar novos números de telefone para o usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="6d9db-137">Da etapa anterior, um novo usuário (Avery) tem apenas uma senha registrada.</span><span class="sxs-lookup"><span data-stu-id="6d9db-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="6d9db-138">Para atribuir um novo número de telefone para o Avery usar, faça uma solicitação de `POST` com o tipo de telefone e número no corpo.</span><span class="sxs-lookup"><span data-stu-id="6d9db-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="6d9db-139">Para informar ao sistema que um número de telefone está sendo adicionado, também será necessário alterar o final da URL de `methods` para `phoneMethods`.</span><span class="sxs-lookup"><span data-stu-id="6d9db-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-140">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a><span data-ttu-id="6d9db-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="6d9db-142">Para adicionar o número comercial do Avery, você vai `POST` novamente para a mesma URL, mas atualizará o número e o tipo de telefone:</span><span class="sxs-lookup"><span data-stu-id="6d9db-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-143">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a><span data-ttu-id="6d9db-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="6d9db-145">Faça mais um `GET` na URL de métodos de telefone para ver todos os números de telefone do Avery:</span><span class="sxs-lookup"><span data-stu-id="6d9db-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="6d9db-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-147">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

<span data-ttu-id="6d9db-148">Confirme se você consegue ver os dois números conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="6d9db-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="6d9db-149">Etapa 4: Remover um número de telefone do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="6d9db-150">Neste cenário, o Avery agora está trabalhando em casa e você precisa remover o número comercial da conta.</span><span class="sxs-lookup"><span data-stu-id="6d9db-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="6d9db-151">É necessário chamar `DELETE` na URL do telefone comercial, que pode ser criado anexando a ID do telefone comercial à URL de métodos de telefone.</span><span class="sxs-lookup"><span data-stu-id="6d9db-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="6d9db-152">Veja acima a lista de telefones do Avery: a ID do telefone comercial começa com "e37f".</span><span class="sxs-lookup"><span data-stu-id="6d9db-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="6d9db-154">Não há dados na resposta porque não há mais telefone comercial, conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="6d9db-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="6d9db-155">Confirme se ele desapareceu em todos os métodos do Avery, que é o mesmo `GET` feito anteriormente:</span><span class="sxs-lookup"><span data-stu-id="6d9db-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="6d9db-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-157">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

<span data-ttu-id="6d9db-158">Como esperado, o usuário agora voltou a ter apenas um telefone celular e uma senha.</span><span class="sxs-lookup"><span data-stu-id="6d9db-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="6d9db-159">Etapa 5: Redefinir senha do usuário</span><span class="sxs-lookup"><span data-stu-id="6d9db-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="6d9db-160">Neste cenário, o Avery esqueceu a senha e você precisa redefini-la.</span><span class="sxs-lookup"><span data-stu-id="6d9db-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="6d9db-161">Para redefinir, você fará uma `POST` na URL da senha (veja acima a ID começando com "28c1" na lista de métodos de autenticação do Avery), especificando a ação "resetPassword".</span><span class="sxs-lookup"><span data-stu-id="6d9db-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="6d9db-162">Forneça a nova senha no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d9db-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="6d9db-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-164">Response</span></span>

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="6d9db-165">Como isso está sincronizando a senha com o Active Directory na infraestrutura local do locatário, poderá levar alguns minutos, então você tem um endereço onde poderá verificar se está completo.</span><span class="sxs-lookup"><span data-stu-id="6d9db-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="6d9db-166">Esse endereço está no cabeçalho do local da resposta e, para ver o status, faça um `GET` na URL.</span><span class="sxs-lookup"><span data-stu-id="6d9db-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="6d9db-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d9db-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="6d9db-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d9db-168">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

<span data-ttu-id="6d9db-169">E sucesso!</span><span class="sxs-lookup"><span data-stu-id="6d9db-169">And success!</span></span> <span data-ttu-id="6d9db-170">Você viu o perfil de um usuário, seus métodos de autenticação, como adicionar e remover números de telefone, e como redefinir senha.</span><span class="sxs-lookup"><span data-stu-id="6d9db-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="6d9db-171">Agora, você está pronto para gerenciar os métodos dos seus usuários.</span><span class="sxs-lookup"><span data-stu-id="6d9db-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="6d9db-172">Referência da API</span><span class="sxs-lookup"><span data-stu-id="6d9db-172">API reference</span></span>

<span data-ttu-id="6d9db-173">Está procurando a referência de API para métodos de autenticação?</span><span class="sxs-lookup"><span data-stu-id="6d9db-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="6d9db-174">Confira [Visão geral da API dos métodos de autenticação do Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="6d9db-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d9db-175">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6d9db-175">Next steps</span></span>

* <span data-ttu-id="6d9db-176">Descubra como [usar as APIs REST do método de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6d9db-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="6d9db-177">Use o Azure AD para se [autenticar](./auth/index.yml) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6d9db-177">Use Azure AD to [authenticate](./auth/index.yml) to Microsoft Graph.</span></span>
* <span data-ttu-id="6d9db-178">Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.</span><span class="sxs-lookup"><span data-stu-id="6d9db-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="6d9db-179">Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6d9db-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="6d9db-180">Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6d9db-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>