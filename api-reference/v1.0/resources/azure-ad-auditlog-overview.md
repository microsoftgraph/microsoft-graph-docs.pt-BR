---
title: Visão geral da API de relatórios de atividades
description: Use a API de relatórios de atividades no Microsoft Graph para acessar os relatórios que o Azure Active Directory cria para ajudar a rastrear a atividade do usuário em um locatário.
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: eba6b2af8dd6437d8996ab0bc2304c99eb7b4ac1
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129443"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="e9f4d-103">Visão geral da API de relatórios de atividades</span><span class="sxs-lookup"><span data-stu-id="e9f4d-103">Activity reports API overview</span></span>

<span data-ttu-id="e9f4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9f4d-105">O Azure Active Directory (Azure AD) rastreia a atividade do usuário e cria relatórios que ajudam a entender como seus usuários acessam e usam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="e9f4d-106">Use a API do Microsoft Graph para Azure AD para analisar os dados nesses relatórios e criar soluções personalizadas adaptadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="e9f4d-107">A disponibilidade desses relatórios de atividades é regida pelas políticas de retenção de dados do Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="e9f4d-108">Para saber mais, confira [políticas de retenção de dados](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-108">For more information, see [data retention policies](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="e9f4d-109">O que são logs de atividade do Azure Active Directory?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="e9f4d-110">O Microsoft Azure Active Directory fornece os seguintes tipos de relatórios de atividades:</span><span class="sxs-lookup"><span data-stu-id="e9f4d-110">Azure AD provides the following types of activity reports:</span></span>

- <span data-ttu-id="e9f4d-111">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="e9f4d-111">Directory audits</span></span>
- <span data-ttu-id="e9f4d-112">Entradas</span><span class="sxs-lookup"><span data-stu-id="e9f4d-112">Sign-ins</span></span>

### <a name="directory-audits"></a><span data-ttu-id="e9f4d-113">Auditorias de diretório</span><span class="sxs-lookup"><span data-stu-id="e9f4d-113">Directory audits</span></span>

<span data-ttu-id="e9f4d-114">O relatório de auditoria de diretório fornece acesso ao histórico de todas as tarefas executadas em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-114">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="e9f4d-115">O relatório de auditoria de diretório fornece registros de atividades do sistema para conformidade.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-115">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="e9f4d-116">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="e9f4d-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="e9f4d-117">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-117">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="e9f4d-118">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-118">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="e9f4d-119">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="e9f4d-120">Entradas</span><span class="sxs-lookup"><span data-stu-id="e9f4d-120">Sign-ins</span></span>

<span data-ttu-id="e9f4d-121">O relatório de entradas ajuda a determinar quem executou as tarefas relatadas pelas auditorias de diretório.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-121">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="e9f4d-122">O relatório de entrada ajuda você a responder a perguntas como:</span><span class="sxs-lookup"><span data-stu-id="e9f4d-122">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="e9f4d-123">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="e9f4d-124">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="e9f4d-125">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="e9f4d-126">O que posso fazer com as APIs de log de auditoria no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="e9f4d-127">As seguintes solicitações são populares para trabalhar com dados de log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="e9f4d-127">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="e9f4d-128">Operation</span><span class="sxs-lookup"><span data-stu-id="e9f4d-128">Operation</span></span> | <span data-ttu-id="e9f4d-129">URL</span><span class="sxs-lookup"><span data-stu-id="e9f4d-129">URL</span></span>
:----------|:----
<span data-ttu-id="e9f4d-130">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="e9f4d-130">GET tenant user activities</span></span> | [<span data-ttu-id="e9f4d-131">OBTER https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="e9f4d-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="e9f4d-132">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="e9f4d-132">GET tenant user sign-ins</span></span> | [<span data-ttu-id="e9f4d-133">OBTER https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="e9f4d-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="e9f4d-134">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="e9f4d-134">What licenses do I need?</span></span>

<span data-ttu-id="e9f4d-135">Os relatórios de atividades estão disponíveis para os recursos que você licenciou.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-135">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="e9f4d-136">Se você possui uma licença para um recurso específico, também tem acesso aos relatórios.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-136">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="e9f4d-137">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-137">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="e9f4d-138">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-138">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="e9f4d-139">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-139">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="e9f4d-140">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-140">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="e9f4d-141">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e9f4d-141">Next Steps</span></span>

- <span data-ttu-id="e9f4d-142">[Registre seu aplicativo](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para atender aos pré-requisitos do relatório.</span><span class="sxs-lookup"><span data-stu-id="e9f4d-142">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="e9f4d-143">Para saber como recuperar os logs de auditoria enquanto são autenticados usando certificados, consulte o [Tutorial: Obter dados usando a API de relatórios do Azure Active Directory com certificados](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-143">To learn how to retrieve audit logs while authenticated using certificates, see [Tutorial: Get data using the Azure Active Directory reporting API with certificates](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).</span></span>   
- <span data-ttu-id="e9f4d-144">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-144">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="e9f4d-145">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="e9f4d-145">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
