---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b8b53037c70ff68523f51dd266da69518a1cc57a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133040"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="6ee9c-103">Visão geral da API de relatórios de atividades</span><span class="sxs-lookup"><span data-stu-id="6ee9c-103">Activity reports API overview</span></span>

<span data-ttu-id="6ee9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ee9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee9c-105">O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="6ee9c-106">Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="6ee9c-107">A disponibilidade desses relatórios de atividades é regida pelas políticas de retenção de dados do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="6ee9c-108">Para saber mais, confira [políticas de retenção de dados](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-108">For more information, see [data retention policies](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-activity-reports"></a><span data-ttu-id="6ee9c-109">O que são relatórios de atividades?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-109">What are activity reports?</span></span>

<span data-ttu-id="6ee9c-110">O Microsoft Azure Active Directory fornece três tipos de relatórios de atividades:</span><span class="sxs-lookup"><span data-stu-id="6ee9c-110">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="6ee9c-111">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="6ee9c-111">Directory audits</span></span> 
- <span data-ttu-id="6ee9c-112">Entradas</span><span class="sxs-lookup"><span data-stu-id="6ee9c-112">Sign-ins</span></span>
- <span data-ttu-id="6ee9c-113">Provisionamento</span><span class="sxs-lookup"><span data-stu-id="6ee9c-113">Provisioning</span></span>

### <a name="directory-audits"></a><span data-ttu-id="6ee9c-114">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="6ee9c-114">Directory audits</span></span>

<span data-ttu-id="6ee9c-115">O relatório de auditoria de diretório fornece acesso ao histórico de todas as tarefas executadas em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-115">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="6ee9c-116">O relatório de auditoria de diretório fornece registros de atividades do sistema para conformidade.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-116">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="6ee9c-117">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="6ee9c-117">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="6ee9c-118">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-118">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="6ee9c-119">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-119">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="6ee9c-120">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-120">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="6ee9c-121">Entradas</span><span class="sxs-lookup"><span data-stu-id="6ee9c-121">Sign-ins</span></span>

<span data-ttu-id="6ee9c-122">O relatório de entradas ajuda a determinar quem executou as tarefas relatadas pelas auditorias de diretório.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-122">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="6ee9c-123">O relatório de entrada ajuda você a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="6ee9c-123">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="6ee9c-124">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-124">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="6ee9c-125">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-125">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="6ee9c-126">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-126">What's the status of these sign-ins?</span></span>

### <a name="provisioning"></a><span data-ttu-id="6ee9c-127">Provisionamento</span><span class="sxs-lookup"><span data-stu-id="6ee9c-127">Provisioning</span></span>

<span data-ttu-id="6ee9c-128">O relatório de aprovisionamento ajuda a ver todas as ações executadas pelo serviço de provisionamento do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-128">The provisioning report helps you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="6ee9c-129">O relatório de aprovisionamento ajuda a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="6ee9c-129">The provisioning report helps you answer questions like:</span></span>

- <span data-ttu-id="6ee9c-130">Quais grupos foram criados com sucesso no ServiceNow?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-130">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="6ee9c-131">Quais funções foram importadas dos serviços Web da Amazon?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-131">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="6ee9c-132">Quais usuários foram criados sem sucesso a partir da workday?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-132">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a><span data-ttu-id="6ee9c-133">O que posso fazer com os relatórios de atividades do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-133">What can I do with activity reports in Microsoft Graph?</span></span>

<span data-ttu-id="6ee9c-134">Aqui estão solicitações populares para trabalhar com dados de relatório:</span><span class="sxs-lookup"><span data-stu-id="6ee9c-134">Here are popular requests for working with report data:</span></span>

<span data-ttu-id="6ee9c-135">Operation</span><span class="sxs-lookup"><span data-stu-id="6ee9c-135">Operation</span></span> | <span data-ttu-id="6ee9c-136">URL</span><span class="sxs-lookup"><span data-stu-id="6ee9c-136">URL</span></span>
:----------|:----
<span data-ttu-id="6ee9c-137">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="6ee9c-137">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="6ee9c-138">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="6ee9c-138">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="6ee9c-139">OBTER logs de provisionamento</span><span class="sxs-lookup"><span data-stu-id="6ee9c-139">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="6ee9c-140">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="6ee9c-140">What licenses do I need?</span></span>

<span data-ttu-id="6ee9c-141">Os relatórios de atividades estão disponíveis para os recursos que você licenciou.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-141">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="6ee9c-142">Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-142">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="6ee9c-143">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-143">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="6ee9c-144">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-144">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="6ee9c-145">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-145">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="6ee9c-146">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-146">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ee9c-147">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6ee9c-147">Next steps</span></span>

- <span data-ttu-id="6ee9c-148">[Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório.</span><span class="sxs-lookup"><span data-stu-id="6ee9c-148">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="6ee9c-149">Aprenda com [amostras do log de auditoria](/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-149">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="6ee9c-150">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-150">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="6ee9c-151">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-151">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="6ee9c-152">Analisar o recurso[provisioningObjectSummary](provisioningobjectsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6ee9c-152">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
