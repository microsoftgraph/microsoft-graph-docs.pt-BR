---
title: Microsoft 365 Lighthouse Visão geral da API
description: Microsoft 365 Lighthouse é um portal de administração que ajuda os MSPs (Provedores de Serviços Gerenciados) a proteger e gerenciar dispositivos, dados e usuários em escala para clientes de pequenas e médias empresas (SMB) que estão usando o Microsoft 365 Business Premium.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 177a2f03fe5ee0e2e7d90ade038dcef1f7d6c3db
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401885"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a><span data-ttu-id="36f51-103">Visão geral do gerenciamento de vários locatários usando Microsoft 365 Lighthouse API</span><span class="sxs-lookup"><span data-stu-id="36f51-103">Overview for multi-tenant management using the Microsoft 365 Lighthouse API</span></span>

<span data-ttu-id="36f51-104">Microsoft 365 Lighthouse é um portal de administração que permite que os MSPs (Provedores de Serviços Gerenciados) gerenciem remotamente vários locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="36f51-104">Microsoft 365 Lighthouse is an admin portal that lets Managed Service Providers (MSPs) remotely manage multiple customer tenants.</span></span> <span data-ttu-id="36f51-105">Ele ajuda os MSPs a proteger e gerenciar dispositivos, dados e usuários em escala para clientes de pequenas e médias empresas (SMB) que estão usando Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="36f51-105">It helps MSPs secure and manage devices, data, and users at scale for small- and medium-sized business (SMB) customers who are using Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="36f51-106">Microsoft 365 Lighthouse ajuda os MSPs a simplificar a integração de Microsoft 365 Business Premium locatários do cliente.</span><span class="sxs-lookup"><span data-stu-id="36f51-106">Microsoft 365 Lighthouse helps MSPs simplify onboarding of Microsoft 365 Business Premium customer tenants.</span></span> <span data-ttu-id="36f51-107">Ele oferece a um MSP a conveniência de exibições de vários locatários em todos os ambientes de locatários do cliente.</span><span class="sxs-lookup"><span data-stu-id="36f51-107">It offers an MSP the convenience of multi-tenant views across all its customer tenant environments.</span></span> <span data-ttu-id="36f51-108">Ele pode recomendar linhas de base de configuração de segurança personalizadas para os clientes SMB do MSP.</span><span class="sxs-lookup"><span data-stu-id="36f51-108">It can recommend security configuration baselines tailored to the MSP's SMB customers.</span></span> <span data-ttu-id="36f51-109">Com Microsoft 365 Lighthouse, os MSPs podem dimensionar o gerenciamento de seus locatários de clientes, se concentrar no que é mais importante, encontrar e investigar riscos rapidamente e tomar medidas para ajudar a obter seus locatários de clientes para um estado íntegre e seguro.</span><span class="sxs-lookup"><span data-stu-id="36f51-109">With Microsoft 365 Lighthouse, MSPs can scale the management of their customer tenants, focus on what's most important, quickly find and investigate risks, and take action to help get their customer tenants to a healthy and secure state.</span></span>

> [!NOTE]  
> <span data-ttu-id="36f51-110">Esta documentação trata da API Microsoft 365 Lighthouse disponível no _Microsoft Graph_.</span><span class="sxs-lookup"><span data-stu-id="36f51-110">This documentation is about the Microsoft 365 Lighthouse API available on _Microsoft Graph_.</span></span> <span data-ttu-id="36f51-111">Uma oferta semelhante, o Azure Lighthouse, ajuda os provedores de serviços a fornecer serviços gerenciados para serviços do Azure usando ferramentas de gerenciamento abrangentes e robustas integradas à plataforma _do Azure._</span><span class="sxs-lookup"><span data-stu-id="36f51-111">A similar offering, Azure Lighthouse, helps service providers deliver managed services for Azure services by using comprehensive and robust management tooling built into the _Azure_ platform.</span></span> <span data-ttu-id="36f51-112">Para saber mais, confira [O que é o Farol do Azure.](/azure/lighthouse/overview)</span><span class="sxs-lookup"><span data-stu-id="36f51-112">To learn more, see [What is Azure Lighthouse](/azure/lighthouse/overview).</span></span>

## <a name="why-integrate-with-microsoft-365-lighthouse"></a><span data-ttu-id="36f51-113">Por que se integrar Microsoft 365 Lighthouse?</span><span class="sxs-lookup"><span data-stu-id="36f51-113">Why integrate with Microsoft 365 Lighthouse?</span></span>

<span data-ttu-id="36f51-114">Como um MSP, você pode usar a API Microsoft 365 Lighthouse no Microsoft Graph para obter informações sobre riscos identificados e tomar medidas para ajudar a obter seus clientes em um estado saudável e seguro.</span><span class="sxs-lookup"><span data-stu-id="36f51-114">As an MSP, you can use the Microsoft 365 Lighthouse API in Microsoft Graph to gain insights into identified risks and take action to help get your customers into a healthy and secure state.</span></span>

### <a name="devices"></a><span data-ttu-id="36f51-115">Dispositivos</span><span class="sxs-lookup"><span data-stu-id="36f51-115">Devices</span></span>

<span data-ttu-id="36f51-116">Você pode usar a API do Farol para executar as seguintes tarefas de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="36f51-116">You can use the Lighthouse API to perform the following device tasks:</span></span>

- <span data-ttu-id="36f51-117">Analise [as tendências de conformidade](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) do dispositivo para entender melhor como a conformidade do dispositivo está evoluindo ao longo do tempo para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="36f51-117">Analyze [device compliance trends](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) to better understand how device compliance is evolving over time for your customers.</span></span>
- <span data-ttu-id="36f51-118">Entenda quais [políticas de conformidade de](/graph/api/resources/managedtenants-manageddevicecompliance) dispositivo foram criadas em seus clientes e o status das políticas.</span><span class="sxs-lookup"><span data-stu-id="36f51-118">Understand what [device compliance policies](/graph/api/resources/managedtenants-manageddevicecompliance) have been created across your customers and the status of the policies.</span></span>

### <a name="threat-management"></a><span data-ttu-id="36f51-119">Gerenciamento de ameaças</span><span class="sxs-lookup"><span data-stu-id="36f51-119">Threat management</span></span>

<span data-ttu-id="36f51-120">Você pode usar a API do Farol para executar as seguintes tarefas de gerenciamento de ameaças:</span><span class="sxs-lookup"><span data-stu-id="36f51-120">You can use the Lighthouse API to perform the following threat management tasks:</span></span>

- <span data-ttu-id="36f51-121">Obtenha informações sobre o estado de [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) presente nos dispositivos Windows registrados para gerenciamento em seus clientes.</span><span class="sxs-lookup"><span data-stu-id="36f51-121">Gain insight to the state of [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) that is present on the Windows devices registered for management across your customers.</span></span>
- <span data-ttu-id="36f51-122">Exibir o [estado de proteção](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) para dispositivos Windows registrados para gerenciamento em seus clientes para garantir que os usuários Windows Defender estão em um estado saudável.</span><span class="sxs-lookup"><span data-stu-id="36f51-122">View the [protection state](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) for Windows devices registered for management across your customers to ensure those using Windows Defender are in a healthy state.</span></span>

### <a name="users"></a><span data-ttu-id="36f51-123">Usuários</span><span class="sxs-lookup"><span data-stu-id="36f51-123">Users</span></span>

<span data-ttu-id="36f51-124">Você pode usar a API do Farol para executar as seguintes tarefas de usuário:</span><span class="sxs-lookup"><span data-stu-id="36f51-124">You can use the Lighthouse API to perform the following user tasks:</span></span>

- <span data-ttu-id="36f51-125">Descubra [usuários arriscados](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) em seus clientes.</span><span class="sxs-lookup"><span data-stu-id="36f51-125">Discover [risky users](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) across your customers.</span></span>
- <span data-ttu-id="36f51-126">Exibir resumo do registro do usuário [de credencial](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) para entender o que os usuários em seus clientes registraram para autenticação multifaionária e redefinição de senha de autoatendados.</span><span class="sxs-lookup"><span data-stu-id="36f51-126">View [credential user registration summary](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) to understand what users across your customers have registered for multi-factor authentication and self-service password reset.</span></span>

## <a name="api-reference"></a><span data-ttu-id="36f51-127">Referência da API</span><span class="sxs-lookup"><span data-stu-id="36f51-127">API reference</span></span>

<span data-ttu-id="36f51-128">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="36f51-128">Looking for the API reference for this service?</span></span>

<span data-ttu-id="36f51-129">Consulte [Microsoft 365 Lighthouse API no Microsoft Graph (visualização)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="36f51-129">See [Microsoft 365 Lighthouse API in Microsoft Graph (preview)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).</span></span>

> [!NOTE]
> <span data-ttu-id="36f51-130">A Microsoft 365 Lighthouse api é definida no subnamespace OData, `microsoft.graph.managedTenants` .</span><span class="sxs-lookup"><span data-stu-id="36f51-130">The Microsoft 365 Lighthouse API is defined in the OData subnamespace, `microsoft.graph.managedTenants`.</span></span>


## <a name="next-steps"></a><span data-ttu-id="36f51-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="36f51-131">Next steps</span></span>

- <span data-ttu-id="36f51-132">Saiba mais sobre o [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.</span><span class="sxs-lookup"><span data-stu-id="36f51-132">Learn more about the [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.</span></span>
- <span data-ttu-id="36f51-133">Saiba mais sobre os [novos recursos e atualizações mais recentes para](/graph/whats-new-overview) a API do Farol.</span><span class="sxs-lookup"><span data-stu-id="36f51-133">Find out about the [latest new features and updates](/graph/whats-new-overview) for the Lighthouse API.</span></span>
- <span data-ttu-id="36f51-134">Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="36f51-134">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
