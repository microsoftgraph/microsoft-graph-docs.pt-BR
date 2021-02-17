---
title: Visão geral da API da política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 593cbea196edcbe1c868a337b1dcfa8a1de2afc9
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271824"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="b1f37-103">Visão geral da API de políticas de métodos de autenticação do Azure AD</span><span class="sxs-lookup"><span data-stu-id="b1f37-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="b1f37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1f37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1f37-105">As políticas de métodos de autenticação [definem](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a MFA (autenticação multifatofa) no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b1f37-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b1f37-106">As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança FIDO2 e login por telefone sem senha com o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="b1f37-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="b1f37-107">As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política.</span><span class="sxs-lookup"><span data-stu-id="b1f37-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="b1f37-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b1f37-108">For example:</span></span>

* <span data-ttu-id="b1f37-109">Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="b1f37-110">Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou login por telefone sem senha para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="b1f37-111">Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="b1f37-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="b1f37-112">Política de método de autenticação</span><span class="sxs-lookup"><span data-stu-id="b1f37-112">Authentication method policy</span></span>       | <span data-ttu-id="b1f37-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f37-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="b1f37-114">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1f37-114">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="b1f37-115">Defina os usuários que podem usar a Mensagem de Texto no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-115">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="b1f37-116">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="b1f37-116">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="b1f37-117">Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-117">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="b1f37-118">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="b1f37-118">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="b1f37-119">Defina os usuários que podem usar o Microsoft Authenticator no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-119">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="b1f37-120">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="b1f37-120">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="b1f37-121">Defina os usuários que podem usar o OTP de email no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-121">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="b1f37-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="b1f37-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="b1f37-123">Defina os usuários que podem usar a Assinatura de Telefone Sem Senha para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-123">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="b1f37-124">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="b1f37-124">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="b1f37-125">Defina os usuários que podem usar o Acesso Temporário para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1f37-125">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="b1f37-126">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b1f37-126">Next steps</span></span>

* <span data-ttu-id="b1f37-127">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b1f37-127">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
