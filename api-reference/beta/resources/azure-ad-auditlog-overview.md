---
title: Visão geral sobre o API do log de auditoria AD Azure
description: Azure Active Directory (AD Azure) rastreia métricas de atividade e a entrada do usuário e auditoria de cria relatórios de log que ajudarão-lo a entender como os usuários acessam e aproveitem os serviços do Azure AD. Use a API do Microsoft Graph para Azure AD para analisar os dados base esses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.
localization_priority: Priority
ms.openlocfilehash: 07d285ce4e7fbf736900c1d6d4acdf159b451424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826219"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="563cc-104">Visão geral sobre o API do log de auditoria AD Azure</span><span class="sxs-lookup"><span data-stu-id="563cc-104">Azure AD audit log API overview</span></span>

> <span data-ttu-id="563cc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="563cc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="563cc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="563cc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="563cc-107">Azure Active Directory (AD Azure) rastreia métricas de atividade e a entrada do usuário e auditoria de cria relatórios de log que ajudarão-lo a entender como os usuários acessam e aproveitem os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="563cc-107">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="563cc-108">Use a API do Microsoft Graph para Azure AD para analisar os dados base esses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="563cc-108">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="563cc-109">Cite atividade do Azure AD logs?</span><span class="sxs-lookup"><span data-stu-id="563cc-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="563cc-110">Azure AD fornece dois tipos de logs de atividade:</span><span class="sxs-lookup"><span data-stu-id="563cc-110">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="563cc-111">logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="563cc-111">audit logs</span></span> 
- <span data-ttu-id="563cc-112">logs de entrar</span><span class="sxs-lookup"><span data-stu-id="563cc-112">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="563cc-113">Logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="563cc-113">Audit logs</span></span>

<span data-ttu-id="563cc-114">O relatório de atividade de logs de auditoria oferece acesso ao histórico de cada tarefa seja executada no seu locatário.</span><span class="sxs-lookup"><span data-stu-id="563cc-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="563cc-115">O relatório de logs de auditoria fornece registros de atividades do sistema para fins de conformidade.</span><span class="sxs-lookup"><span data-stu-id="563cc-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="563cc-116">Entre outros, os dados fornecidos permite abordar cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="563cc-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="563cc-117">Quem concedida acesso de administração de grupo a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="563cc-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="563cc-118">Quais usuários estão entrando para um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="563cc-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="563cc-119">Redefine as senhas quantos foram feitos dentro do diretório?</span><span class="sxs-lookup"><span data-stu-id="563cc-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="563cc-120">Inscreva-se nos logs</span><span class="sxs-lookup"><span data-stu-id="563cc-120">Sign in logs</span></span>

<span data-ttu-id="563cc-121">O relatório de atividade de logons ajuda a determinar quem executou as tarefas relatadas pelo relatórios do log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="563cc-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="563cc-122">O relatório de atividade de logons ajuda você a responder perguntas como:</span><span class="sxs-lookup"><span data-stu-id="563cc-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="563cc-123">O que é o padrão de um usuário entrar?</span><span class="sxs-lookup"><span data-stu-id="563cc-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="563cc-124">Quantos usuários tem entrado durante a última semana?</span><span class="sxs-lookup"><span data-stu-id="563cc-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="563cc-125">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="563cc-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="563cc-126">O que pode fazer com que o log de auditoria APIs no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="563cc-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="563cc-127">Aqui estão as solicitações de populares para trabalhar com dados de log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="563cc-127">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="563cc-128">Operação</span><span class="sxs-lookup"><span data-stu-id="563cc-128">Operation</span></span> | <span data-ttu-id="563cc-129">URL</span><span class="sxs-lookup"><span data-stu-id="563cc-129">URL</span></span>
:----------|:----
<span data-ttu-id="563cc-130">Obtenha as atividades do usuário de Inquilino</span><span class="sxs-lookup"><span data-stu-id="563cc-130">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="563cc-131">OBTER locatário entradas do usuário</span><span class="sxs-lookup"><span data-stu-id="563cc-131">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="563cc-132">Quais licenças são necessárias?</span><span class="sxs-lookup"><span data-stu-id="563cc-132">What licenses do I need?</span></span>

<span data-ttu-id="563cc-133">Relatórios do log de auditoria estão disponíveis para os recursos que você licenciou.</span><span class="sxs-lookup"><span data-stu-id="563cc-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="563cc-134">Se você tiver uma licença para um recurso específico, você também tem acesso aos seus logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="563cc-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="563cc-135">Por exemplo, você precisa de uma licença do Windows Azure AD Premium P1 para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="563cc-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="563cc-136">Para saber mais, consulte [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="563cc-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="563cc-137">Relatórios de entrar exigem uma licença do Windows Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="563cc-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="563cc-138">Para saber mais, consulte [preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="563cc-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="563cc-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="563cc-139">Next Steps</span></span>

- <span data-ttu-id="563cc-140">[Registrar seu aplicativo](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender a pré-requisitos de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="563cc-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="563cc-141">Saiba do [log de auditoria](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) e [exemplos de entrada](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="563cc-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="563cc-142">Revise o recurso [directoryAudit](directoryaudit.md) e ações.</span><span class="sxs-lookup"><span data-stu-id="563cc-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="563cc-143">Revise o recurso de [logon](signin.md) e ações.</span><span class="sxs-lookup"><span data-stu-id="563cc-143">Review [signIn](signin.md) resource and actions.</span></span> 
