---
title: Visão geral da API de log de auditoria do Azure AD
description: O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e utilizam os serviços do Azure AD. Use a API do Microsoft Graph para o Azure AD para analisar os dados desses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.
localization_priority: Priority
ms.openlocfilehash: 89be0007ae6c13fb48ba165ca991f5dfa9d9b9cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543853"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="3c83e-104">Visão geral da API de log de auditoria do Azure AD</span><span class="sxs-lookup"><span data-stu-id="3c83e-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c83e-105">O Azure AD (Azure Active Directory) controla métricas de atividade e de entrada de usuário e cria logs de auditoria que ajudam você a entender como os usuários acessam e utilizam os serviços do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c83e-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="3c83e-106">Use a API do Microsoft Graph para o Azure AD para analisar os dados desses relatórios e criar soluções personalizadas adequadas às necessidades específicas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="3c83e-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="3c83e-107">O que são logs de atividade do Azure AD?</span><span class="sxs-lookup"><span data-stu-id="3c83e-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="3c83e-108">O Azure AD oferece dois tipos de logs de atividade:</span><span class="sxs-lookup"><span data-stu-id="3c83e-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="3c83e-109">Logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="3c83e-109">audit logs</span></span> 
- <span data-ttu-id="3c83e-110">Logs de entrada</span><span class="sxs-lookup"><span data-stu-id="3c83e-110">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="3c83e-111">Logs de auditoria</span><span class="sxs-lookup"><span data-stu-id="3c83e-111">Audit logs</span></span>

<span data-ttu-id="3c83e-112">O relatório de atividades de logs de auditoria fornece acesso ao histórico de todas as tarefas executada em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="3c83e-112">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="3c83e-113">O relatório de logs de auditoria fornece registros de atividades do sistema de conformidade.</span><span class="sxs-lookup"><span data-stu-id="3c83e-113">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="3c83e-114">Entre outros benefícios, os dados fornecidos permitem que você aborde cenários comuns, como:</span><span class="sxs-lookup"><span data-stu-id="3c83e-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="3c83e-115">Quem concedeu acesso ao grupo de administradores a um usuário de diretório?</span><span class="sxs-lookup"><span data-stu-id="3c83e-115">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="3c83e-116">Quais usuários estão se conectando a um aplicativo adquirido recentemente?</span><span class="sxs-lookup"><span data-stu-id="3c83e-116">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="3c83e-117">Quantas redefinições de senhas foram feitas no diretório?</span><span class="sxs-lookup"><span data-stu-id="3c83e-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="3c83e-118">Logs de entrada</span><span class="sxs-lookup"><span data-stu-id="3c83e-118">Sign in logs</span></span>

<span data-ttu-id="3c83e-119">O relatório de atividade de entrada ajuda a determinar quem realizou as tarefas relatadas pelos relatórios de log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3c83e-119">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="3c83e-120">O relatório de atividades de entrada ajuda a responder perguntas como:</span><span class="sxs-lookup"><span data-stu-id="3c83e-120">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="3c83e-121">O que é o padrão de entrada de um usuário?</span><span class="sxs-lookup"><span data-stu-id="3c83e-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="3c83e-122">Quantos usuários entraram durante a semana passada?</span><span class="sxs-lookup"><span data-stu-id="3c83e-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="3c83e-123">Qual é o status dessas entradas?</span><span class="sxs-lookup"><span data-stu-id="3c83e-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="3c83e-124">O que posso fazer com as APIs de log de auditoria no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="3c83e-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="3c83e-125">Estas são solicitações populares para trabalhar com dados de log de auditoria:</span><span class="sxs-lookup"><span data-stu-id="3c83e-125">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="3c83e-126">Operação</span><span class="sxs-lookup"><span data-stu-id="3c83e-126">Operation</span></span> | <span data-ttu-id="3c83e-127">URL</span><span class="sxs-lookup"><span data-stu-id="3c83e-127">URL</span></span>
:----------|:----
<span data-ttu-id="3c83e-128">OBTER atividades de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="3c83e-128">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="3c83e-129">OBTER entradas de usuário do locatário</span><span class="sxs-lookup"><span data-stu-id="3c83e-129">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="3c83e-130">De quais licenças eu preciso?</span><span class="sxs-lookup"><span data-stu-id="3c83e-130">What licenses do I need?</span></span>

<span data-ttu-id="3c83e-131">Os relatórios de log de auditoria estão disponíveis para os recursos que você tiver licenciado.</span><span class="sxs-lookup"><span data-stu-id="3c83e-131">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="3c83e-132">Se você tiver uma licença para um recurso específico, também terá acesso a seus logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3c83e-132">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="3c83e-133">Por exemplo, você precisa de uma licença P1 do Azure AD Premium para acessar os relatórios de auditoria de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="3c83e-133">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="3c83e-134">Para saber mais, confira [Licenciamento do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="3c83e-134">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="3c83e-135">Relatórios de entrada requerem uma licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="3c83e-135">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="3c83e-136">Para saber mais, consulte [Preços do Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="3c83e-136">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="3c83e-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3c83e-137">Next Steps</span></span>

- <span data-ttu-id="3c83e-138">[Registre seu aplicativo](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para satisfazer aos pré-requisitos do log de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3c83e-138">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="3c83e-139">Aprenda com [amostras do log de auditoria](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) e de [entrada](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="3c83e-139">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="3c83e-140">Analisar recurso e ações do [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="3c83e-140">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="3c83e-141">Analisar recurso e ações do [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="3c83e-141">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
