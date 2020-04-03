---
title: Visão geral da API de log de auditoria do Azure AD
description: O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e usam os serviços do Azure AD. Use a API do Microsoft Graph para o Azure AD para analisar os dados desses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: kholtz
ms.openlocfilehash: 7bd0a0d0f5c32f36d887880c148fcd29caeeb7be
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124466"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="8274f-104">Visão geral da API de log de auditoria do Azure AD</span><span class="sxs-lookup"><span data-stu-id="8274f-104">Azure AD audit log API overview</span></span>

<span data-ttu-id="8274f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8274f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8274f-106">O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e usam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8274f-106">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="8274f-107">Use a API do Microsoft Graph para o Azure AD para analisar os dados desses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8274f-107">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="8274f-108">O que são logs de atividade do Azure AD?</span><span class="sxs-lookup"><span data-stu-id="8274f-108">What are Azure AD activity logs?</span></span>

<span data-ttu-id="8274f-109">O Azure AD oferece dois tipos de logs de atividade:</span><span class="sxs-lookup"><span data-stu-id="8274f-109">Azure AD provides three types of activity logs:</span></span>

- <span data-ttu-id="8274f-110">Logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="8274f-110">Audit logs</span></span> 
- <span data-ttu-id="8274f-111">Logs de entrada</span><span class="sxs-lookup"><span data-stu-id="8274f-111">Sign-in logs</span></span>
- <span data-ttu-id="8274f-112">Modo de Provisionamento</span><span class="sxs-lookup"><span data-stu-id="8274f-112">Provisioning logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="8274f-113">Logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="8274f-113">Audit logs</span></span>

<span data-ttu-id="8274f-114">O relatório de atividades de logs de auditoria fornece acesso ao histórico de todas as tarefas executada em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="8274f-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="8274f-115">O relatório de logs de auditoria fornece registros de atividades do sistema de conformidade.</span><span class="sxs-lookup"><span data-stu-id="8274f-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="8274f-116">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="8274f-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="8274f-117">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="8274f-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="8274f-118">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="8274f-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="8274f-119">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="8274f-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="8274f-120">Logs de entrada</span><span class="sxs-lookup"><span data-stu-id="8274f-120">Sign-in logs</span></span>

<span data-ttu-id="8274f-121">O relatório de atividade de entrada ajuda a determinar quem realizou as tarefas relatadas pelos relatórios de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8274f-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="8274f-122">O relatório de atividades de entrada ajuda a responder perguntas como:</span><span class="sxs-lookup"><span data-stu-id="8274f-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="8274f-123">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="8274f-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="8274f-124">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="8274f-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="8274f-125">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="8274f-125">What's the status of these sign-ins?</span></span>

### <a name="provisioning-logs"></a><span data-ttu-id="8274f-126">Modo de Provisionamento</span><span class="sxs-lookup"><span data-stu-id="8274f-126">Provisioning logs</span></span>
<span data-ttu-id="8274f-127">Os logs de provisionamento ajudam a ver todas as ações executadas pelo serviço de provisionamento do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8274f-127">The provisioning logs help you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="8274f-128">Os logs de provisionamento ajudam você a responder perguntas como:</span><span class="sxs-lookup"><span data-stu-id="8274f-128">The provisioning logs help you answer questions like:</span></span>

- <span data-ttu-id="8274f-129">Quais grupos foram criados com sucesso no ServiceNow?</span><span class="sxs-lookup"><span data-stu-id="8274f-129">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="8274f-130">Quais funções foram importadas dos serviços Web da Amazon?</span><span class="sxs-lookup"><span data-stu-id="8274f-130">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="8274f-131">Quais usuários foram criados sem sucesso a partir da workday?</span><span class="sxs-lookup"><span data-stu-id="8274f-131">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="8274f-132">O que posso fazer com as APIs de log de auditoria no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="8274f-132">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="8274f-133">Estas são solicitações populares para trabalhar com dados de log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="8274f-133">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="8274f-134">Operação</span><span class="sxs-lookup"><span data-stu-id="8274f-134">Operation</span></span> | <span data-ttu-id="8274f-135">URL</span><span class="sxs-lookup"><span data-stu-id="8274f-135">URL</span></span>
:----------|:----
<span data-ttu-id="8274f-136">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="8274f-136">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="8274f-137">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="8274f-137">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="8274f-138">OBTER logs de provisionamento</span><span class="sxs-lookup"><span data-stu-id="8274f-138">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryProvisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryProvisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="8274f-139">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="8274f-139">What licenses do I need?</span></span>

<span data-ttu-id="8274f-140">Os relatórios de log de auditoria estão disponíveis para os recursos que você tiver licenciado.</span><span class="sxs-lookup"><span data-stu-id="8274f-140">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="8274f-141">Se você tiver uma licença para um recurso específico, também terá acesso a seus logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8274f-141">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="8274f-142">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="8274f-142">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="8274f-143">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="8274f-143">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="8274f-144">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="8274f-144">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="8274f-145">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="8274f-145">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8274f-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8274f-146">Next steps</span></span>

- <span data-ttu-id="8274f-147">[Registre seu aplicativo](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para satisfazer aos pré-requisitos do log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8274f-147">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="8274f-148">Aprenda com [amostras do log de auditoria](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="8274f-148">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="8274f-149">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="8274f-149">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="8274f-150">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="8274f-150">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="8274f-151">Analisar o recurso[provisioningObjectSummary](provisioningobjectsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8274f-151">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
