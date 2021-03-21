---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 5aed8ead61bb9f2dde102dc085e5509945d492f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964628"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="eef1a-103">Visão geral das políticas de políticas de autenticação do Azure AD</span><span class="sxs-lookup"><span data-stu-id="eef1a-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="eef1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eef1a-105">As políticas de [](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifatofa (MFA) no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="eef1a-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="eef1a-106">As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem Chaves de Segurança FIDO2 e Login de Telefone Sem Senha com o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="eef1a-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="eef1a-107">As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política.</span><span class="sxs-lookup"><span data-stu-id="eef1a-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="eef1a-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="eef1a-108">For example:</span></span>

* <span data-ttu-id="eef1a-109">Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eef1a-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="eef1a-110">Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança fido2 ou entrar sem senha para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eef1a-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="eef1a-111">Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="eef1a-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="eef1a-112">Política de método de autenticação</span><span class="sxs-lookup"><span data-stu-id="eef1a-112">Authentication method policy</span></span>       | <span data-ttu-id="eef1a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef1a-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="eef1a-114">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="eef1a-114">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="eef1a-115">Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eef1a-115">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="eef1a-116">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="eef1a-116">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="eef1a-117">Definir usuários que podem usar o Microsoft Authenticator no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eef1a-117">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="eef1a-118">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="eef1a-118">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="eef1a-119">Definir usuários que podem usar o OTP de email no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eef1a-119">Define users who can use email OTP on the Azure AD tenant.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="eef1a-120">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="eef1a-120">Next steps</span></span>

* <span data-ttu-id="eef1a-121">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="eef1a-121">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
