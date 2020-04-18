---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários são autenticados no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 73f4bb06d15c6b2e41226e872b71ba417de1076b
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557903"
---
# <a name="azure-ad-authentication-methods-api-overview"></a><span data-ttu-id="4f89a-103">Visão geral da API de métodos de autenticação do Azure AD</span><span class="sxs-lookup"><span data-stu-id="4f89a-103">Azure AD authentication methods API overview</span></span>

<span data-ttu-id="4f89a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f89a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f89a-105">Os [métodos de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) são as maneiras como os usuários são autenticados no Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="4f89a-105">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (AD).</span></span> <span data-ttu-id="4f89a-106">Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que podem ser gerenciados no Microsoft Graph hoje, entre muitas outras, como chaves de segurança do FIDO2 e o aplicativo Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="4f89a-106">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="4f89a-107">Os métodos de autenticação são usados na autenticação principal, de segundo fator e de etapa e também no processo de redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="4f89a-107">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="4f89a-108">As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-108">The authentication method APIs are used to manage a user's authentication methods.</span></span> <span data-ttu-id="4f89a-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="4f89a-109">For example:</span></span>

* <span data-ttu-id="4f89a-110">Você pode adicionar um número de telefone a um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-110">You can add a phone number to a user.</span></span> <span data-ttu-id="4f89a-111">Em seguida, o usuário pode usar esse número de telefone para autenticação de SMS e de chamada de voz se estiver habilitado para usá-lo por política.</span><span class="sxs-lookup"><span data-stu-id="4f89a-111">The user can then use that phone number for SMS and voice call authentication if they're enabled to use it by policy.</span></span> 
* <span data-ttu-id="4f89a-112">Você pode atualizar esse número ou excluí-lo do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-112">You can update that number, or delete it from the user.</span></span>
* <span data-ttu-id="4f89a-113">Você pode habilitar ou desabilitar o número para entrada do SMS.</span><span class="sxs-lookup"><span data-stu-id="4f89a-113">You can enable or disable the number for SMS sign-in.</span></span>
* <span data-ttu-id="4f89a-114">Você pode redefinir a senha de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-114">You can reset a user's password.</span></span>

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="4f89a-115">Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="4f89a-115">What authentication methods can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="4f89a-116">Método de autenticação</span><span class="sxs-lookup"><span data-stu-id="4f89a-116">Authentication method</span></span>       | <span data-ttu-id="4f89a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f89a-117">Description</span></span> |<span data-ttu-id="4f89a-118">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4f89a-118">Examples</span></span>     |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="4f89a-119">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f89a-119">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md)| <span data-ttu-id="4f89a-120">No momento, uma senha é o método de autenticação principal padrão no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4f89a-120">A password is currently the default primary authentication method in Azure AD.</span></span>|<span data-ttu-id="4f89a-121">Redefinir a senha de um usuário</span><span class="sxs-lookup"><span data-stu-id="4f89a-121">Reset a user's password</span></span>|
|[<span data-ttu-id="4f89a-122">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f89a-122">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md)|<span data-ttu-id="4f89a-123">Um telefone pode ser usado por um usuário para autenticar usando o [SMS ou chamadas de voz](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).</span><span class="sxs-lookup"><span data-stu-id="4f89a-123">A phone can be used by a user to authenticate using [SMS or voice calls](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (as allowed by policy).</span></span>|<span data-ttu-id="4f89a-124">Confira os números de telefone de autenticação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-124">See a user's authentication phone numbers.</span></span> <span data-ttu-id="4f89a-125">Adicionar, atualizar ou remover um número de telefone para um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f89a-125">Add, update, or remove a phone number to a user.</span></span> <span data-ttu-id="4f89a-126">Habilitar ou desabilitar um telefone celular principal para entrada do SMS.</span><span class="sxs-lookup"><span data-stu-id="4f89a-126">Enable or disable a primary mobile phone for SMS sign-in.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="4f89a-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4f89a-127">Next steps</span></span>

* <span data-ttu-id="4f89a-128">Revise os tipos de método de autenticação e seus vários métodos.</span><span class="sxs-lookup"><span data-stu-id="4f89a-128">Review the authentication method types and their various methods.</span></span>
* <span data-ttu-id="4f89a-129">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="4f89a-129">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
