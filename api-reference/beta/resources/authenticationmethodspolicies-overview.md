---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 35d3beecb26a5ae4455502ed0535c959cf7f502e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682128"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="d76f8-103">Visão geral das políticas de políticas de autenticação do Azure AD</span><span class="sxs-lookup"><span data-stu-id="d76f8-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="d76f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d76f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d76f8-105">As políticas de [](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d76f8-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d76f8-106">As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança fido2 e Telefone de acesso sem senha com Microsoft Authenticator aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d76f8-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="d76f8-107">As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política.</span><span class="sxs-lookup"><span data-stu-id="d76f8-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="d76f8-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="d76f8-108">For example:</span></span>

* <span data-ttu-id="d76f8-109">Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="d76f8-110">Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou senhas Telefone entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>
* <span data-ttu-id="d76f8-111">Defina os usuários ou grupos de usuários que devem ser lembrados para configurar o Microsoft Authenticator para MFA usando notificações por push.</span><span class="sxs-lookup"><span data-stu-id="d76f8-111">Define the users or groups of users who should be reminded to set up the Microsoft Authenticator for MFA using push notifications.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="d76f8-112">Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="d76f8-112">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="d76f8-113">Política de método de autenticação</span><span class="sxs-lookup"><span data-stu-id="d76f8-113">Authentication method policy</span></span>       | <span data-ttu-id="d76f8-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d76f8-114">Description</span></span> |
|:---------------------------|:------------|
|[<span data-ttu-id="d76f8-115">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d76f8-115">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="d76f8-116">Definir usuários que podem usar Mensagem de Texto no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-116">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="d76f8-117">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d76f8-117">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="d76f8-118">Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-118">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="d76f8-119">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d76f8-119">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="d76f8-120">Definir usuários que podem usar Microsoft Authenticator no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-120">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="d76f8-121">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d76f8-121">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="d76f8-122">Definir usuários que podem usar o OTP de email no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-122">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="d76f8-123">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="d76f8-123">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="d76f8-124">Defina os usuários que podem usar a senha Telefone entrar para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-124">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="d76f8-125">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d76f8-125">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="d76f8-126">Defina os usuários que podem usar o Passe de Acesso Temporário para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d76f8-126">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a><span data-ttu-id="d76f8-127">Políticas disponíveis para pressionar os usuários a configurar métodos de autenticação:</span><span class="sxs-lookup"><span data-stu-id="d76f8-127">Policies available to push users to set up authentication methods:</span></span>
|<span data-ttu-id="d76f8-128">Política</span><span class="sxs-lookup"><span data-stu-id="d76f8-128">Policy</span></span>       | <span data-ttu-id="d76f8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d76f8-129">Description</span></span> |
|:---------------------------|:------------|
|[<span data-ttu-id="d76f8-130">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="d76f8-130">authenticationMethodsRegistrationCampaign</span></span>](authenticationmethodsregistrationcampaign.md)| <span data-ttu-id="d76f8-131">Defina os usuários que devem ser lembrados para configurar um método de autenticação (somente com suporte para o Microsoft Authenticator).</span><span class="sxs-lookup"><span data-stu-id="d76f8-131">Define users who should be reminded to set up an authentication method (only supported for the Microsoft Authenticator).</span></span>|

## <a name="next-steps"></a><span data-ttu-id="d76f8-132">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d76f8-132">Next steps</span></span>

* <span data-ttu-id="d76f8-133">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="d76f8-133">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
