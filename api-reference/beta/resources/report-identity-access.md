---
title: Visão geral da API de relatórios de identidade e acesso
description: Acesse a identidade e os relatórios de acesso para obter informações sobre como as pessoas da sua empresa estão usando os aplicativos no locatário do Azure Active Directory.
localization_priority: Priority
ms.prod: identity-and-access-reports
author: besiler
doc_type: conceptualPageType
ms.openlocfilehash: 567bfdfd848c2a7f1df19b8aad76a68774a6bf0e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129363"
---
# <a name="identity-and-access-reports-api-overview"></a><span data-ttu-id="5c07f-103">Visão geral da API de relatórios de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="5c07f-103">Identity and access reports API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c07f-104">Com o Microsoft Graph, você pode usar a identidade de acesso e os relatórios de acesso para obter informações sobre como as pessoas da sua empresa estão usando aplicativos no locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5c07f-104">With Microsoft Graph, you can use access identity and access reports to get information about how people in your business are using applications in your Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="authorization"></a><span data-ttu-id="5c07f-105">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c07f-105">Authorization</span></span>

<span data-ttu-id="5c07f-106">O Microsoft Graph controla o acesso aos recursos utilizando permissões.</span><span class="sxs-lookup"><span data-stu-id="5c07f-106">Microsoft Graph controls access to resources using permissions.</span></span> <span data-ttu-id="5c07f-107">Você deve especificar as permissões necessárias para acessar os recursos dos relatórios.</span><span class="sxs-lookup"><span data-stu-id="5c07f-107">You must specify the permissions you need in order to access reports resources.</span></span> <span data-ttu-id="5c07f-108">Para saber mais, veja [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e[Permissões de relatórios](/graph/permissions-reference#reports-permissions).</span><span class="sxs-lookup"><span data-stu-id="5c07f-108">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="what-are-identity-and-access-reports"></a><span data-ttu-id="5c07f-109">O que são relatórios de identidade e acesso?</span><span class="sxs-lookup"><span data-stu-id="5c07f-109">What are identity and access reports?</span></span>

<span data-ttu-id="5c07f-110">Os seguintes relatórios de identidade e acesso estão disponíveis para ajudá-lo a entender a atividade do aplicativo no seu locatário:</span><span class="sxs-lookup"><span data-stu-id="5c07f-110">The following identity and access reports are available to help you understand application activity in your tenant:</span></span>

- <span data-ttu-id="5c07f-111">Atividade de aplicativo no AD FS</span><span class="sxs-lookup"><span data-stu-id="5c07f-111">AD FS application activity</span></span>
- <span data-ttu-id="5c07f-112">Entrar no aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c07f-112">Application sign-in</span></span>
- <span data-ttu-id="5c07f-113">Registro e utilização</span><span class="sxs-lookup"><span data-stu-id="5c07f-113">Registration and usage</span></span>

### <a name="ad-fs-application-activity"></a><span data-ttu-id="5c07f-114">Atividade de aplicativo no AD FS</span><span class="sxs-lookup"><span data-stu-id="5c07f-114">AD FS application activity</span></span>

<span data-ttu-id="5c07f-115">O relatório de atividades do aplicativo AD FS fornece informações sobre como uma terceira parte confiável é configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração da terceira parte confiável pode ser migrada para o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5c07f-115">The AD FS application activity report provides information about how a relying party is configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span> <span data-ttu-id="5c07f-116">Para obter mais informações, consulte o recurso [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5c07f-116">For more information, see the [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="application-sign-in"></a><span data-ttu-id="5c07f-117">Entrar no aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c07f-117">Application sign-in</span></span>

<span data-ttu-id="5c07f-118">Avalie o uso de logins de aplicativos no seu locatário utilizando um relatório de resumo ou um relatório que forneça detalhes de entradas, como o número de entradas e se ocorreu algum erro durante a entrada.</span><span class="sxs-lookup"><span data-stu-id="5c07f-118">Evaluate the usage of application sign-ins in your tenant using either a summary report or a report that provides details of sign-ins, such as the number of sign-ins and whether any errors occured during sign-in.</span></span> <span data-ttu-id="5c07f-119">Para mais informações, consulte o recurso [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5c07f-119">For more information, see the [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="registration-and-usage"></a><span data-ttu-id="5c07f-120">Registro e utilização</span><span class="sxs-lookup"><span data-stu-id="5c07f-120">Registration and usage</span></span>

<span data-ttu-id="5c07f-121">Entenda melhor como os usuários da sua organização utilizam os recursos do Microsoft Azure Active Directory, como o autoatendimento para redefinição de senha e autenticação multifatorial (MFA).</span><span class="sxs-lookup"><span data-stu-id="5c07f-121">Get a better understanding of how users in your organization use Azure AD capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span> <span data-ttu-id="5c07f-122">Você pode determinar quais métodos de autenticação são mais bem-sucedidos para sua organização, quais tipos de erros os usuários finais estão enfrentando e qual campanha você precisa executar para ajudar seus usuários finais a adotar o uso do autoatendimento para redefinição de senha e MFA.</span><span class="sxs-lookup"><span data-stu-id="5c07f-122">You can determine which authentication methods are more successful for your organization, what types of errors end users are running into, and what campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span> <span data-ttu-id="5c07f-123">Para obter mais informações, consulte a [API de relatório de uso de métodos de autenticação](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5c07f-123">For more information, see the [authentication methods usage report API](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span></span>

## <a name="next-steps"></a><span data-ttu-id="5c07f-124">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5c07f-124">Next steps</span></span>

<span data-ttu-id="5c07f-125">APIs e recursos de relatório podem criar novas maneiras para você relacionar-se com os usuários e gerenciar as experiências deles com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5c07f-125">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="5c07f-126">Para saber mais:</span><span class="sxs-lookup"><span data-stu-id="5c07f-126">To learn more:</span></span>

- <span data-ttu-id="5c07f-127">Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.</span><span class="sxs-lookup"><span data-stu-id="5c07f-127">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="5c07f-128">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="5c07f-128">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


