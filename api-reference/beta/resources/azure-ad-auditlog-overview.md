---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: besiler
ms.openlocfilehash: 5e49061d4212b2b81482d57b0a7048d52c242572
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523634"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="7c0c6-103">Visão geral da API de relatórios de atividades</span><span class="sxs-lookup"><span data-stu-id="7c0c6-103">Activity reports API overview</span></span>

<span data-ttu-id="7c0c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c0c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c0c6-105">O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="7c0c6-106">Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-activity-reports"></a><span data-ttu-id="7c0c6-107">O que são relatórios de atividades?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-107">What are activity reports?</span></span>

<span data-ttu-id="7c0c6-108">O Azure AD fornece três tipos de relatórios de atividades:</span><span class="sxs-lookup"><span data-stu-id="7c0c6-108">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="7c0c6-109">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="7c0c6-109">Directory audits</span></span> 
- <span data-ttu-id="7c0c6-110">Entradas</span><span class="sxs-lookup"><span data-stu-id="7c0c6-110">Sign-ins</span></span>
- <span data-ttu-id="7c0c6-111">Provisionamento</span><span class="sxs-lookup"><span data-stu-id="7c0c6-111">Provisioning</span></span>

### <a name="directory-audits"></a><span data-ttu-id="7c0c6-112">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="7c0c6-112">Directory audits</span></span>

<span data-ttu-id="7c0c6-113">O relatório de auditoria de diretório fornece acesso ao histórico de todas as tarefas executadas em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-113">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="7c0c6-114">O relatório de auditoria de diretório fornece registros de atividades do sistema para conformidade.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-114">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="7c0c6-115">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="7c0c6-115">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="7c0c6-116">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-116">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="7c0c6-117">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-117">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="7c0c6-118">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-118">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="7c0c6-119">Entradas</span><span class="sxs-lookup"><span data-stu-id="7c0c6-119">Sign-ins</span></span>

<span data-ttu-id="7c0c6-120">O relatório de entradas ajuda a determinar quem executou as tarefas relatadas pelas auditorias de diretório.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-120">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="7c0c6-121">O relatório de entrada ajuda você a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="7c0c6-121">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="7c0c6-122">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-122">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="7c0c6-123">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-123">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="7c0c6-124">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-124">What's the status of these sign-ins?</span></span>

### <a name="provisioning"></a><span data-ttu-id="7c0c6-125">Provisionamento</span><span class="sxs-lookup"><span data-stu-id="7c0c6-125">Provisioning</span></span>

<span data-ttu-id="7c0c6-126">O relatório de aprovisionamento ajuda a ver todas as ações executadas pelo serviço de provisionamento do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-126">The provisioning report helps you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="7c0c6-127">O relatório de aprovisionamento ajuda a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="7c0c6-127">The provisioning report helps you answer questions like:</span></span>

- <span data-ttu-id="7c0c6-128">Quais grupos foram criados com sucesso no ServiceNow?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-128">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="7c0c6-129">Quais funções foram importadas dos serviços Web da Amazon?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-129">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="7c0c6-130">Quais usuários foram criados sem sucesso a partir da workday?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-130">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a><span data-ttu-id="7c0c6-131">O que posso fazer com os relatórios de atividades do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-131">What can I do with activity reports in Microsoft Graph?</span></span>

<span data-ttu-id="7c0c6-132">Aqui estão solicitações populares para trabalhar com dados de relatório:</span><span class="sxs-lookup"><span data-stu-id="7c0c6-132">Here are popular requests for working with report data:</span></span>

<span data-ttu-id="7c0c6-133">Operation</span><span class="sxs-lookup"><span data-stu-id="7c0c6-133">Operation</span></span> | <span data-ttu-id="7c0c6-134">URL</span><span class="sxs-lookup"><span data-stu-id="7c0c6-134">URL</span></span>
:----------|:----
<span data-ttu-id="7c0c6-135">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="7c0c6-135">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="7c0c6-136">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="7c0c6-136">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="7c0c6-137">OBTER logs de provisionamento</span><span class="sxs-lookup"><span data-stu-id="7c0c6-137">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="7c0c6-138">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="7c0c6-138">What licenses do I need?</span></span>

<span data-ttu-id="7c0c6-139">Os relatórios de atividades estão disponíveis para os recursos que você licenciou.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-139">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="7c0c6-140">Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-140">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="7c0c6-141">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-141">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="7c0c6-142">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-142">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="7c0c6-143">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-143">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="7c0c6-144">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-144">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7c0c6-145">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7c0c6-145">Next steps</span></span>

- <span data-ttu-id="7c0c6-146">[Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório.</span><span class="sxs-lookup"><span data-stu-id="7c0c6-146">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="7c0c6-147">Aprenda com [amostras do log de auditoria](/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-147">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="7c0c6-148">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-148">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="7c0c6-149">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-149">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="7c0c6-150">Analisar o recurso[provisioningObjectSummary](provisioningobjectsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7c0c6-150">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>