---
title: Visão geral da API de política
description: O Azure Active Directory usa políticas para controlar comportamentos de recursos do Azure AD em sua organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: b64efc81caa10c249030e33cb893d90aec8a1afb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229441"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="a1e71-103">Visão geral da política do Azure AD</span><span class="sxs-lookup"><span data-stu-id="a1e71-103">Azure AD policy overview</span></span>

<span data-ttu-id="a1e71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1e71-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a1e71-105">O Azure Active Directory (Azure AD) usa políticas para controlar comportamentos de recursos do Azure AD em sua organização.</span><span class="sxs-lookup"><span data-stu-id="a1e71-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="a1e71-106">As políticas são regras personalizadas que podem ser impostas em aplicativos, entidades de serviço, grupos ou em toda a organização à qual foram atribuídos.</span><span class="sxs-lookup"><span data-stu-id="a1e71-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="a1e71-107">Quais políticas estão disponíveis?</span><span class="sxs-lookup"><span data-stu-id="a1e71-107">What policies are available?</span></span>

| <span data-ttu-id="a1e71-108">Tipo de política</span><span class="sxs-lookup"><span data-stu-id="a1e71-108">Policy type</span></span>       | <span data-ttu-id="a1e71-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e71-109">Description</span></span> | <span data-ttu-id="a1e71-110">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1e71-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="a1e71-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="a1e71-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="a1e71-112">Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="a1e71-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="a1e71-113">Configure o portal do Azure para ter um tempo limite de inatividade de 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="a1e71-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="a1e71-114">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="a1e71-114">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="a1e71-115">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="a1e71-115">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="a1e71-116">Configure todos os usuários para ignorar a descoberta de realm inicial e ser roteado diretamente para o ADFS para autenticação.</span><span class="sxs-lookup"><span data-stu-id="a1e71-116">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="a1e71-117">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="a1e71-117">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="a1e71-118">Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.</span><span class="sxs-lookup"><span data-stu-id="a1e71-118">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="a1e71-119">Configure um aplicativo especialmente confidencial com uma vida útil mais curta do que o token padrão.</span><span class="sxs-lookup"><span data-stu-id="a1e71-119">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="a1e71-120">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="a1e71-120">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="a1e71-121">Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a1e71-121">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="a1e71-122">Configure o algoritmo de assinatura ou a versão token SAML a ser usado para emitir o token SAML.</span><span class="sxs-lookup"><span data-stu-id="a1e71-122">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a1e71-123">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e71-123">Next steps</span></span>

* <span data-ttu-id="a1e71-124">Revise os diferentes tipos de recursos de política listados acima e seus vários métodos.</span><span class="sxs-lookup"><span data-stu-id="a1e71-124">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="a1e71-125">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="a1e71-125">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
