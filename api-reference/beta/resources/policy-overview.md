---
title: Visão geral da API de política
description: O Azure Active Directory usa políticas para controlar comportamentos de recursos do Azure AD em sua organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 3829a4018c9b904b058329d52149e98337ebfae6
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234131"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="ff161-103">Visão geral da política do Azure AD</span><span class="sxs-lookup"><span data-stu-id="ff161-103">Azure AD policy overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff161-104">O Azure Active Directory (Azure AD) usa políticas para controlar comportamentos de recursos do Azure AD em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ff161-104">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="ff161-105">As políticas são regras personalizadas que podem ser impostas em aplicativos, entidades de serviço, grupos ou em toda a organização à qual foram atribuídos.</span><span class="sxs-lookup"><span data-stu-id="ff161-105">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="ff161-106">Quais políticas estão disponíveis?</span><span class="sxs-lookup"><span data-stu-id="ff161-106">What policies are available?</span></span>

| <span data-ttu-id="ff161-107">Tipo de política</span><span class="sxs-lookup"><span data-stu-id="ff161-107">Policy type</span></span>       | <span data-ttu-id="ff161-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff161-108">Description</span></span> | <span data-ttu-id="ff161-109">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff161-109">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="ff161-110">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="ff161-110">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="ff161-111">Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="ff161-111">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="ff161-112">Configure o portal do Azure para ter um tempo limite de inatividade de 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="ff161-112">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="ff161-113">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="ff161-113">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="ff161-114">Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="ff161-114">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="ff161-115">Crie e atribua uma política para omitir as declarações básicas de tokens emitidos para uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ff161-115">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="ff161-116">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="ff161-116">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="ff161-117">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="ff161-117">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="ff161-118">Configure todos os usuários para ignorar a descoberta de realm inicial e ser roteado diretamente para o ADFS para autenticação.</span><span class="sxs-lookup"><span data-stu-id="ff161-118">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="ff161-119">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="ff161-119">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="ff161-120">Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.</span><span class="sxs-lookup"><span data-stu-id="ff161-120">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="ff161-121">Configure um aplicativo especialmente confidencial com uma vida útil mais curta do que o token padrão.</span><span class="sxs-lookup"><span data-stu-id="ff161-121">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="ff161-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ff161-122">Next steps</span></span>

* <span data-ttu-id="ff161-123">Revise os diferentes tipos de recursos de política listados acima e seus vários métodos.</span><span class="sxs-lookup"><span data-stu-id="ff161-123">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="ff161-124">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="ff161-124">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
