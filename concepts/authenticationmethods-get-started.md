---
title: Introdução à API dos métodos de autenticação do Microsoft Graph
description: A API de métodos de autenticação no Microsoft Graph oferece às organizações a capacidade de gerenciar programaticamente os métodos de autenticação de seus usuários, obtendo aos usuários registrados para fazer a autenticação multifator (MFA) e redefinição de senha de autoatendimento (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272805"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="2f232-103">Introdução à API dos métodos de autenticação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2f232-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="2f232-104">Os [métodos de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) são as maneiras como os usuários são autenticados no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2f232-104">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="2f232-105">Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que podem ser gerenciados no Microsoft Graph hoje, entre muitas outras, como chaves de segurança do FIDO2 e o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="2f232-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="2f232-106">Os métodos de autenticação são usados na autenticação principal, de segundo fator e de etapa e também no processo de redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="2f232-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="2f232-107">Você pode usar as APIs do método de autenticação para gerenciar os métodos de autenticação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2f232-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="2f232-108">Por exemplo, você pode:</span><span class="sxs-lookup"><span data-stu-id="2f232-108">For example, you can:</span></span>

* <span data-ttu-id="2f232-109">Adicionar um número de telefone para um usuário, que pode usar esse número para autenticação de SMS e de chamada de voz, se estiverem habilitados para usá-lo por política</span><span class="sxs-lookup"><span data-stu-id="2f232-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="2f232-110">Atualizar ou excluir o número de telefone atribuído a um usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="2f232-111">Habilitar ou desabilitar o número para entrada do SMS</span><span class="sxs-lookup"><span data-stu-id="2f232-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="2f232-112">Redefinir a senha de um usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-112">Reset a user's password</span></span>

<span data-ttu-id="2f232-113">As APIs são uma ferramenta principal para gerenciar os métodos de autenticação dos seus usuários.</span><span class="sxs-lookup"><span data-stu-id="2f232-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="2f232-114">Neste tutorial, você aprenderá a:</span><span class="sxs-lookup"><span data-stu-id="2f232-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="2f232-115">Autenticar no Azure AD com as funções e permissões corretas</span><span class="sxs-lookup"><span data-stu-id="2f232-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="2f232-116">Verificar os métodos de autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="2f232-117">Adicionar novos números de telefone para o usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="2f232-118">Remover um número de telefone do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="2f232-119">Redefinir a senha do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="2f232-120">Etapa 1: autenticar no Azure AD com as funções e permissões corretas</span><span class="sxs-lookup"><span data-stu-id="2f232-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="2f232-121">Usando sua [ferramenta favorita para interagir com o Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), entre usando uma conta com uma destas funções:</span><span class="sxs-lookup"><span data-stu-id="2f232-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="2f232-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2f232-122">Global administrator</span></span>
* <span data-ttu-id="2f232-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="2f232-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="2f232-124">Administrador de Autenticação</span><span class="sxs-lookup"><span data-stu-id="2f232-124">Authentication administrator</span></span>

<span data-ttu-id="2f232-125">Em seguida, modifique suas permissões.</span><span class="sxs-lookup"><span data-stu-id="2f232-125">Next, modify your permissions.</span></span> <span data-ttu-id="2f232-126">Usaremos [UserAuthenticationMethod. ReadWrite. All](permissions-reference.md#user-authentication-method-permissions-preview) para este tutorial, portanto, certifique-se de que ele esteja habilitado no explorador do Graph ou em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f232-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="2f232-127">Depois que o escopo for atribuído e conenviado, você poderá começar a usar a API.</span><span class="sxs-lookup"><span data-stu-id="2f232-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="2f232-128">Os exemplos aqui usam um usuário padrão chamado Avery Howard.</span><span class="sxs-lookup"><span data-stu-id="2f232-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="2f232-129">Você deve usar uma conta de teste preexistente ou criar uma nova, seguindo [estas instruções](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span><span class="sxs-lookup"><span data-stu-id="2f232-129">You should use a preexisting test account or create a new one following [these instructions](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="2f232-130">Essas APIs estão ativas, portanto, não as testem em usuários reais.</span><span class="sxs-lookup"><span data-stu-id="2f232-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="2f232-131">Etapa 2: verificar os métodos de autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="2f232-132">Faça uma chamada para ver os métodos de autenticação do usuário.</span><span class="sxs-lookup"><span data-stu-id="2f232-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="2f232-133">Pegue a URL para ver o perfil de um usuário e adicionar `/authentication/methods` :</span><span class="sxs-lookup"><span data-stu-id="2f232-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="2f232-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="2f232-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-135">Response</span></span>

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="2f232-136">Etapa 3: adicionar novos números de telefone para o usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="2f232-137">Na etapa anterior, um novo usuário (Avery) tem apenas uma senha registrada.</span><span class="sxs-lookup"><span data-stu-id="2f232-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="2f232-138">Para atribuir um novo número de telefone para uso da Avery, faça uma `POST` solicitação com o tipo de telefone e o número no corpo.</span><span class="sxs-lookup"><span data-stu-id="2f232-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="2f232-139">Para informar ao sistema que um número de telefone está sendo adicionado, você também precisará alterar o final da URL de `methods` para `phoneMethods` .</span><span class="sxs-lookup"><span data-stu-id="2f232-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="2f232-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-140">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="2f232-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="2f232-142">Para adicionar o número de escritório da Avery, você irá `POST` novamente para a mesma URL, mas atualizará o tipo e o número de telefone:</span><span class="sxs-lookup"><span data-stu-id="2f232-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="2f232-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="2f232-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="2f232-145">Faça mais uma `GET` a URL dos métodos de telefone para ver todos os números de telefone da Avery:</span><span class="sxs-lookup"><span data-stu-id="2f232-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="2f232-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="2f232-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-147">Response</span></span>

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

<span data-ttu-id="2f232-148">Confirme que você pode ver os dois números conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="2f232-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="2f232-149">Etapa 4: remover um número de telefone do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="2f232-150">Neste cenário, a Avery agora está trabalhando em casa, você precisa remover o número do escritório de sua conta.</span><span class="sxs-lookup"><span data-stu-id="2f232-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="2f232-151">Você precisará chamar `DELETE` a URL do telefone do Office, que você pode criar acrescentando a ID do telefone do escritório à URL dos métodos de telefone.</span><span class="sxs-lookup"><span data-stu-id="2f232-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="2f232-152">Examine a lista de telefones da Avery acima: a ID do telefone do escritório começa com "e37f".</span><span class="sxs-lookup"><span data-stu-id="2f232-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="2f232-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="2f232-154">Não há dados na resposta porque não há mais telefone comercial conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="2f232-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="2f232-155">Você pode confirmar se ele está examinando todos os métodos da Avery, que é o mesmo `GET` que foi feito anteriormente:</span><span class="sxs-lookup"><span data-stu-id="2f232-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="2f232-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="2f232-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-157">Response</span></span>

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

<span data-ttu-id="2f232-158">Como esperado, o usuário agora volta para ter apenas um telefone celular e uma senha.</span><span class="sxs-lookup"><span data-stu-id="2f232-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="2f232-159">Etapa 5: redefinir a senha do usuário</span><span class="sxs-lookup"><span data-stu-id="2f232-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="2f232-160">Neste cenário, a Avery esqueceu a senha e você precisa redefini-la para elas.</span><span class="sxs-lookup"><span data-stu-id="2f232-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="2f232-161">Para redefinir, você irá criar a `POST` URL de sua senha (consulte a ID que começa com "28c1" acima na lista de métodos de autenticação da Avery), especificando a ação "resetPassword".</span><span class="sxs-lookup"><span data-stu-id="2f232-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="2f232-162">Forneça a nova senha no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f232-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="2f232-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="2f232-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-164">Response</span></span>

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="2f232-165">Como isso está sincronizando a senha para o Active Directory na infraestrutura local do locatário, pode levar alguns minutos, para que você tenha um endereço onde você pode verificar se está completo.</span><span class="sxs-lookup"><span data-stu-id="2f232-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="2f232-166">Esse endereço está no cabeçalho de local da resposta e para ver o status da `GET` URL.</span><span class="sxs-lookup"><span data-stu-id="2f232-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="2f232-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f232-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="2f232-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f232-168">Response</span></span>

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

<span data-ttu-id="2f232-169">E sucesso!</span><span class="sxs-lookup"><span data-stu-id="2f232-169">And success!</span></span> <span data-ttu-id="2f232-170">Você viu ver o perfil de um usuário, seus métodos de autenticação, adicionar e remover números de telefone e redefinir sua senha.</span><span class="sxs-lookup"><span data-stu-id="2f232-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="2f232-171">Agora você está pronto para gerenciar os métodos de seus próprios usuários.</span><span class="sxs-lookup"><span data-stu-id="2f232-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="2f232-172">Referência da API</span><span class="sxs-lookup"><span data-stu-id="2f232-172">API reference</span></span>

<span data-ttu-id="2f232-173">Procurando a referência de API para métodos de autenticação?</span><span class="sxs-lookup"><span data-stu-id="2f232-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="2f232-174">Consulte [visão geral da API de métodos de autenticação do Azure ad](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="2f232-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="2f232-175">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2f232-175">Next steps</span></span>

* <span data-ttu-id="2f232-176">Descubra como [usar as APIs REST do método de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="2f232-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="2f232-177">Use o Azure AD para se [autenticar](/graph/auth) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2f232-177">Use Azure AD to [authenticate](/graph/auth) to Microsoft Graph.</span></span>
* <span data-ttu-id="2f232-178">Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.</span><span class="sxs-lookup"><span data-stu-id="2f232-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="2f232-179">Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2f232-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="2f232-180">Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2f232-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
