---
title: Visão geral para acessar as comunicações e a integridade do serviço através do Microsoft Graph
description: Use a API de comunicações do serviço no Microsoft Graph para acessar o status de integridade e as postagens do centro de mensagens sobre os serviços em nuvem da Microsoft.
author: payiAzure
localization_priority: Priority
ms.prod: service-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: f10aabbdbdb7028af3f16058a6137bd9da8615d6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108947"
---
# <a name="overview-for-accessing-service-health-and-communications-in-microsoft-graph"></a><span data-ttu-id="45881-103">Visão geral para acessar as comunicações e a integridade do serviço no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="45881-103">Overview for accessing service health and communications in Microsoft Graph</span></span>
<span data-ttu-id="45881-104">Você pode usar a API de comunicações de serviço no Microsoft Graph para acessar o status de integridade e as postagens do centro de mensagens sobre os serviços em nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="45881-104">You can use the service communications API in Microsoft Graph to access the health status and message center posts about Microsoft cloud services.</span></span> <span data-ttu-id="45881-105">O status de integridade real e as postagens correspondem aos serviços do Microsoft 365 e Dynamics 365 que são suportados pela API e assinados pelo locatário.</span><span class="sxs-lookup"><span data-stu-id="45881-105">The actual health status and posts correspond to the Microsoft 365 and Dynamics 365 services that are supported by the API and subscribed by the tenant.</span></span>

## <a name="why-integrate-with-service-health-and-communications-data"></a><span data-ttu-id="45881-106">Por que integrar com dados de comunicações e integridade do serviço?</span><span class="sxs-lookup"><span data-stu-id="45881-106">Why integrate with service health and communications data?</span></span>

### <a name="get-service-health-and-message-center-posts-for-a-tenant"></a><span data-ttu-id="45881-107">Obter postagens sobre a integridade do serviço e do centro de mensagens para um locatário</span><span class="sxs-lookup"><span data-stu-id="45881-107">Get service health and message center posts for a tenant</span></span>
<span data-ttu-id="45881-108">Os clientes podem obter os dados de integridade atuais ou históricos dos serviços Microsoft com suporte.</span><span class="sxs-lookup"><span data-stu-id="45881-108">Customers can get current or historical health data of supported Microsoft services.</span></span> <span data-ttu-id="45881-109">Ao enfrentar problemas com um serviço da Microsoft, eles podem verificar seu status de integridade para verificar se um problema foi identificado com uma solução em andamento, antes de ligar para o suporte ou gastar tempo solucionando o problema.</span><span class="sxs-lookup"><span data-stu-id="45881-109">When experiencing problems with a Microsoft service, they can check its health status to verify if an issue has been identified with a resolution in progress, before calling for support or spending time troubleshooting.</span></span> 

<span data-ttu-id="45881-110">Os clientes podem revisar regularmente as postagens do centro de mensagens para acompanhar os futuros novos recursos e atualizações, e outros anúncios importantes.</span><span class="sxs-lookup"><span data-stu-id="45881-110">Customers can regularly review message center posts to keep track of upcoming new features and updates, and other important announcements.</span></span> <span data-ttu-id="45881-111">Eles podem então prever como essas mudanças podem afetar os usuários e planejar de acordo.</span><span class="sxs-lookup"><span data-stu-id="45881-111">They can then anticipate how these changes may affect users and plan accordingly.</span></span>

### <a name="integrate-service-communications-data-into-custom-workflows"></a><span data-ttu-id="45881-112">Integre os dados de comunicações de serviço em fluxos de trabalho personalizados</span><span class="sxs-lookup"><span data-stu-id="45881-112">Integrate service communications data into custom workflows</span></span>
<span data-ttu-id="45881-113">Os desenvolvedores de aplicativos podem integrar problemas de integridade do serviço ativo diretamente em aplicativos personalizados, permitindo que os administradores façam a triagem e compartilhem informações de status com o público afetado.</span><span class="sxs-lookup"><span data-stu-id="45881-113">App developers can integrate active service health issues directly into custom applications, allowing administrators to triage and share status information with impacted audiences.</span></span>

<span data-ttu-id="45881-114">Os aplicativos podem permitir fluxos de trabalho personalizados para que os administradores analisem, atribuam e façam a triagem das comunicações de mudança do centro de mensagens.</span><span class="sxs-lookup"><span data-stu-id="45881-114">Apps can enable custom workflows for administrators to review, assign, and triage change communications from the message center.</span></span>

### <a name="build-customer-facing-dashboards"></a><span data-ttu-id="45881-115">Crie painéis voltados para o cliente</span><span class="sxs-lookup"><span data-stu-id="45881-115">Build customer-facing dashboards</span></span>

<span data-ttu-id="45881-116">Crie aplicativos com painéis voltados para o cliente para mostrar a integridade dos serviços Microsoft e permitir que os clientes acompanhem as futuras alterações e outros anúncios importantes sobre os serviços.</span><span class="sxs-lookup"><span data-stu-id="45881-116">Create applications with customer-facing dashboards to show the health of Microsoft services, and let customers keep track of upcoming changes and other important announcements about the services.</span></span>


## <a name="dashboards-examples-in-microsoft-365-admin-center"></a><span data-ttu-id="45881-117">Exemplos de painéis no Centro de administração do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="45881-117">Dashboards examples in Microsoft 365 admin center</span></span>
<span data-ttu-id="45881-118">Esta seção mostra exemplos no [Centro de administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) que usa a API de comunicações do serviço para construir os respectivos painéis de integridade.</span><span class="sxs-lookup"><span data-stu-id="45881-118">This section shows examples in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) that uses the service communications API to build respective health dashboards.</span></span> <span data-ttu-id="45881-119">Entre no centro de administração com uma conta de administrador e clique em **Integridade** para ver os seguintes painéis:</span><span class="sxs-lookup"><span data-stu-id="45881-119">Sign in to the admin center with an admin account, then click **Health** to see the following dashboards:</span></span>
- [<span data-ttu-id="45881-120">Integridade do Serviço</span><span class="sxs-lookup"><span data-stu-id="45881-120">Service health</span></span>](#service-health-dashboard)
- [<span data-ttu-id="45881-121">Integridade da versão do Windows</span><span class="sxs-lookup"><span data-stu-id="45881-121">Windows release health</span></span>](#windows-release-health-dashboard)
- [<span data-ttu-id="45881-122">Centro de mensagens</span><span class="sxs-lookup"><span data-stu-id="45881-122">Message center</span></span>](#message-center-dashboard)

### <a name="service-health-dashboard"></a><span data-ttu-id="45881-123">Painel de integridade do serviço</span><span class="sxs-lookup"><span data-stu-id="45881-123">Service health dashboard</span></span>

<span data-ttu-id="45881-124">No painel **Integridade do serviço**, você pode visualizar a integridade dos serviços Microsoft assinados, que podem incluir Office na web, Yammer, Microsoft Dynamics CRM e serviços de gerenciamento de dispositivos móveis de nuvem.</span><span class="sxs-lookup"><span data-stu-id="45881-124">From the **Service health** dashboad, you can view the health of your subscribed Microsoft services, which can include Office on the web, Yammer, Microsoft Dynamics CRM, and mobile device management cloud services.</span></span> <span data-ttu-id="45881-125">Veja os exemplos demarcados na figura 1.</span><span class="sxs-lookup"><span data-stu-id="45881-125">See examples as demarcated in figure 1.</span></span>

<span data-ttu-id="45881-126">**Figura 1. Painel de integridade do serviço no Centro de administração do Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="45881-126">**Figure 1. Service health dashboard in Microsoft 365 admin center**</span></span>

![Captura de tela do painel de integridade do serviço do Centro de administração do Microsoft 365 para um usuário](images/service-communications-concept-overview-admin-center-serviceHealth2.png)

### <a name="windows-release-health-dashboard"></a><span data-ttu-id="45881-128">Painel de integridade da versão do Windows</span><span class="sxs-lookup"><span data-stu-id="45881-128">Windows release health dashboard</span></span>

<span data-ttu-id="45881-129">No painel de **integridade da versão do Windows**, você pode exibir informações essenciais sobre a qualidade mensal e atualizações de recursos, além dos recursos e aprimoramentos mais recentes do Windows.</span><span class="sxs-lookup"><span data-stu-id="45881-129">From the **Windows release health** dashboad, you can view essential information about monthly quality and feature updates, and the latest features and enhancements for Windows.</span></span> <span data-ttu-id="45881-130">Veja um exemplo conforme demarcado na figura 2.</span><span class="sxs-lookup"><span data-stu-id="45881-130">See an example as demarcated in figure 2.</span></span>

<span data-ttu-id="45881-131">**Figura 2. Painel de integridade da versão do Windows no Centro de administração do Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="45881-131">**Figure 2. Windows release health dashboard in Microsoft 365 admin center**</span></span>

![Captura de tela do painel de integridade da versão Windows do Centro de administração do Microsoft 365 para um usuário](images/service-communications-concept-overview-admin-center-windowshealth2.png)


### <a name="message-center-dashboard"></a><span data-ttu-id="45881-133">Painel do centro de mensagens</span><span class="sxs-lookup"><span data-stu-id="45881-133">Message center dashboard</span></span>
<span data-ttu-id="45881-134">No painel do **Centro de mensagens**, você pode exibir as alterações futuras, incluindo recursos novos e alterados, manutenção planejada e outros anúncios importantes.</span><span class="sxs-lookup"><span data-stu-id="45881-134">From the **Message center** dashboad, you can view upcoming changes, including new and changed features, planned maintenance, and other important announcements.</span></span> <span data-ttu-id="45881-135">Veja os exemplos demarcados na figura 3.</span><span class="sxs-lookup"><span data-stu-id="45881-135">See examples as demarcated in figure 3.</span></span>

<span data-ttu-id="45881-136">**Figura 3. Painel do centro de mensagens no Centro de administração do Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="45881-136">**Figure 3. Message center dashboard in Microsoft 365 admin center**</span></span>

![Captura de tela do painel do centro de mensagens do Centro de administração do Microsoft 365 para um usuário](images/service-communications-concept-overview-admin-center-messagecenter2.png)



## <a name="next-steps"></a><span data-ttu-id="45881-138">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="45881-138">Next steps</span></span>

- <span data-ttu-id="45881-139">Experimente consultas de exemplos de comunicações de serviço no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta).</span><span class="sxs-lookup"><span data-stu-id="45881-139">Try service communications sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta).</span></span>

- <span data-ttu-id="45881-140">Saiba mais sobre a [API de comunicações do serviço](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="45881-140">Learn more about the [service communications API](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>