---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 28d09cfe7dcb78480e02e5a2a23893495eb6655f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546207"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="5e91e-103">Visão geral da API de relatórios de atividades</span><span class="sxs-lookup"><span data-stu-id="5e91e-103">Activity reports API overview</span></span>

<span data-ttu-id="5e91e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e91e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e91e-105">O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5e91e-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="5e91e-106">Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="5e91e-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="5e91e-107">A disponibilidade desses relatórios de atividades é regida pelas políticas de retenção de dados do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5e91e-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="5e91e-108">Para saber mais, confira [políticas de retenção de dados](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span><span class="sxs-lookup"><span data-stu-id="5e91e-108">For more information, see [data retention policies](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="5e91e-109">O que são logs de atividade do Azure Active Directory?</span><span class="sxs-lookup"><span data-stu-id="5e91e-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="5e91e-110">O Microsoft Azure Active Directory fornece os seguintes tipos de relatórios de atividades:</span><span class="sxs-lookup"><span data-stu-id="5e91e-110">Azure AD provides the following types of activity reports:</span></span>

- <span data-ttu-id="5e91e-111">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="5e91e-111">Directory audits</span></span>
- <span data-ttu-id="5e91e-112">Entradas</span><span class="sxs-lookup"><span data-stu-id="5e91e-112">Sign-ins</span></span>

### <a name="directory-audits"></a><span data-ttu-id="5e91e-113">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="5e91e-113">Directory audits</span></span>

<span data-ttu-id="5e91e-114">O relatório de auditoria de diretório fornece acesso ao histórico de todas as tarefas executadas em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="5e91e-114">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="5e91e-115">O relatório de auditoria de diretório fornece registros de atividades do sistema para conformidade.</span><span class="sxs-lookup"><span data-stu-id="5e91e-115">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="5e91e-116">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="5e91e-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="5e91e-117">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="5e91e-117">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="5e91e-118">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="5e91e-118">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="5e91e-119">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="5e91e-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="5e91e-120">Entradas</span><span class="sxs-lookup"><span data-stu-id="5e91e-120">Sign-ins</span></span>

<span data-ttu-id="5e91e-121">O relatório de entradas ajuda a determinar quem executou as tarefas relatadas pelas auditorias de diretório.</span><span class="sxs-lookup"><span data-stu-id="5e91e-121">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="5e91e-122">O relatório de entrada ajuda você a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="5e91e-122">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="5e91e-123">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="5e91e-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="5e91e-124">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="5e91e-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="5e91e-125">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="5e91e-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="5e91e-126">O que posso fazer com as APIs de log de auditoria no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="5e91e-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="5e91e-127">As seguintes solicitações são populares para trabalhar com dados de log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="5e91e-127">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="5e91e-128">Operation</span><span class="sxs-lookup"><span data-stu-id="5e91e-128">Operation</span></span> | <span data-ttu-id="5e91e-129">URL</span><span class="sxs-lookup"><span data-stu-id="5e91e-129">URL</span></span>
:----------|:----
<span data-ttu-id="5e91e-130">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="5e91e-130">GET tenant user activities</span></span> | [<span data-ttu-id="5e91e-131">OBTER https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="5e91e-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="5e91e-132">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="5e91e-132">GET tenant user sign-ins</span></span> | [<span data-ttu-id="5e91e-133">OBTER https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="5e91e-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="5e91e-134">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="5e91e-134">What licenses do I need?</span></span>

<span data-ttu-id="5e91e-135">Os relatórios de atividades estão disponíveis para os recursos que você licenciou.</span><span class="sxs-lookup"><span data-stu-id="5e91e-135">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="5e91e-136">Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.</span><span class="sxs-lookup"><span data-stu-id="5e91e-136">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="5e91e-137">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="5e91e-137">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="5e91e-138">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="5e91e-138">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="5e91e-139">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="5e91e-139">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="5e91e-140">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="5e91e-140">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e91e-141">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5e91e-141">Next Steps</span></span>

- <span data-ttu-id="5e91e-142">[Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório.</span><span class="sxs-lookup"><span data-stu-id="5e91e-142">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="5e91e-143">Aprenda com [amostras do log de auditoria](/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="5e91e-143">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="5e91e-144">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="5e91e-144">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="5e91e-145">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="5e91e-145">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
