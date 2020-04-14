---
title: Trabalhar com a API de relatório de uso dos métodos de autenticação
description: O relatório de uso dos métodos de autenticação ajuda uma organização a entender como os usuários finais estão usando recursos do Azure Active Directory, como redefinição de senha de autoatendimento e autenticação multifator (MFA).
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: d7f7a8e6cddf308c5681f74ca6546a9467704cc6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472197"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="a25dc-103">Trabalhar com a API de relatório de uso dos métodos de autenticação</span><span class="sxs-lookup"><span data-stu-id="a25dc-103">Working with the authentication methods usage report API</span></span>

<span data-ttu-id="a25dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a25dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a25dc-105">Os relatórios de uso dos métodos de autenticação ajudam você a compreender como os usuários da sua organização usam os recursos do Azure Active Directory (Azure AD), como a senha de autoatendimento e a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="a25dc-105">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="a25dc-106">Esses relatórios fornecem informações como:</span><span class="sxs-lookup"><span data-stu-id="a25dc-106">These reports provide information such as:</span></span>

- <span data-ttu-id="a25dc-107">Quais métodos de autenticação são mais bem sucedidos para sua organização.</span><span class="sxs-lookup"><span data-stu-id="a25dc-107">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="a25dc-108">Quais tipos de erros os usuários finais estão executando.</span><span class="sxs-lookup"><span data-stu-id="a25dc-108">What types of errors end users are running into.</span></span>
- <span data-ttu-id="a25dc-109">Qual campanha você precisa executar para ajudar os usuários finais a adotar o uso da senha de autoatendimento REST e da MFA.</span><span class="sxs-lookup"><span data-stu-id="a25dc-109">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="a25dc-110">Solicitações comuns</span><span class="sxs-lookup"><span data-stu-id="a25dc-110">Common requests</span></span>

<span data-ttu-id="a25dc-111">A tabela a seguir lista algumas solicitações comuns que você pode usar com essa API.</span><span class="sxs-lookup"><span data-stu-id="a25dc-111">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="a25dc-112">Operation</span><span class="sxs-lookup"><span data-stu-id="a25dc-112">Operation</span></span> | <span data-ttu-id="a25dc-113">Experimente o Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="a25dc-113">Try in Graph Explorer</span></span> | <span data-ttu-id="a25dc-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a25dc-114">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="a25dc-115">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="a25dc-115">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | <span data-ttu-id="a25dc-116">[OBTER/credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="a25dc-116">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="a25dc-117">Obtenha o número de usuários registrados para redefinição e MFA de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="a25dc-117">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="a25dc-118">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="a25dc-118">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [<span data-ttu-id="a25dc-119">OBTER/credentialusagesummary</span><span class="sxs-lookup"><span data-stu-id="a25dc-119">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="a25dc-120">Obtenha o número de usuários usando a redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="a25dc-120">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="a25dc-121">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="a25dc-121">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [<span data-ttu-id="a25dc-122">OBTER/credentialuserregistrationdetails</span><span class="sxs-lookup"><span data-stu-id="a25dc-122">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="a25dc-123">Obtenha os detalhes do usuário para as atividades de redefinição de senha de autoatendimento e de registro de MFA.</span><span class="sxs-lookup"><span data-stu-id="a25dc-123">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="a25dc-124">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="a25dc-124">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [<span data-ttu-id="a25dc-125">OBTER/usercredentialusagedetails</span><span class="sxs-lookup"><span data-stu-id="a25dc-125">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="a25dc-126">Obtenha detalhes do usuário para todas as atividades de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="a25dc-126">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="a25dc-127">Licenças</span><span class="sxs-lookup"><span data-stu-id="a25dc-127">Licenses</span></span>

<span data-ttu-id="a25dc-128">Relatórios de uso estão disponíveis para recursos licenciados que aproveitam a redefinição de senha de autoatendimento e a MFA em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a25dc-128">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a25dc-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a25dc-129">Next steps</span></span>

- <span data-ttu-id="a25dc-130">Saiba como [implantar a redefinição de senha de autoatendimento do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span><span class="sxs-lookup"><span data-stu-id="a25dc-130">Learn how to [deploy Azure Active Directory self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="a25dc-131">Saiba como implantar o [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span><span class="sxs-lookup"><span data-stu-id="a25dc-131">Learn how to deploy [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="a25dc-132">Saiba como habilitar o [registro de informações de segurança combinado](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span><span class="sxs-lookup"><span data-stu-id="a25dc-132">Learn how to enable [combined security info registration](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>



