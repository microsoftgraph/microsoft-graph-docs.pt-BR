---
title: Visão geral da API da política de métodos de autenticação do Azure AD
description: Métodos de autenticação as políticas definem quais métodos de autenticação podem ser usados por usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 730368b4e47c34353882e5e601644133dbb38225
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921568"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="08f5e-103">Visão geral da API de métodos de autenticação do Azure AD</span><span class="sxs-lookup"><span data-stu-id="08f5e-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="08f5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08f5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f5e-105">Métodos de autenticação as políticas definem [métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) e os usuários que têm permissão para usá-los para entrar e realizar a autenticação multifator (MFA) no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="08f5e-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="08f5e-106">Métodos de autenticação as políticas que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança FIDO2 e entrada de telefone sem senha com o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="08f5e-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="08f5e-107">As APIs de diretivas de método de autenticação são usadas para gerenciar as configurações de política.</span><span class="sxs-lookup"><span data-stu-id="08f5e-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="08f5e-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="08f5e-108">For example:</span></span>

* <span data-ttu-id="08f5e-109">Defina os tipos de chaves de segurança do FIDO2 que podem ser usados no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08f5e-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="08f5e-110">Definir os usuários ou grupos de usuários que têm permissão para usar chaves de segurança do FIDO2 ou entrada de telefone sem senha para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08f5e-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="08f5e-111">Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="08f5e-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="08f5e-112">Política de método de autenticação</span><span class="sxs-lookup"><span data-stu-id="08f5e-112">Authentication method policy</span></span>       | <span data-ttu-id="08f5e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="08f5e-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="08f5e-114">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="08f5e-114">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="08f5e-115">Definir restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08f5e-115">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="08f5e-116">passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="08f5e-116">passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration</span></span>](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="08f5e-117">Defina usuários que podem usar a entrada de telefone sem senha para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08f5e-117">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="08f5e-118">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="08f5e-118">Next steps</span></span>

* <span data-ttu-id="08f5e-119">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="08f5e-119">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
