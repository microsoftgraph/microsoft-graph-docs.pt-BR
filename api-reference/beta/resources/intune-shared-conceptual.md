---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: db7746504a7bd31df99941ffc7bc85065eb5d56a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527474"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="32d9f-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32d9f-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="32d9f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32d9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32d9f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32d9f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32d9f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32d9f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32d9f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32d9f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32d9f-108">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="32d9f-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="32d9f-109">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="32d9f-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="32d9f-110">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="32d9f-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="32d9f-111">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="32d9f-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="32d9f-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="32d9f-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="32d9f-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="32d9f-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="32d9f-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="32d9f-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="32d9f-115">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="32d9f-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="32d9f-116">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="32d9f-116">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="32d9f-117">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="32d9f-117">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="32d9f-118">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="32d9f-118">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="32d9f-119">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="32d9f-119">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="32d9f-120">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-120">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="32d9f-121">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-121">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="32d9f-122">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-122">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="32d9f-123">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-123">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="32d9f-124">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-124">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="32d9f-125">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-125">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="32d9f-126">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-126">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="32d9f-127">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="32d9f-127">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="32d9f-128">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="32d9f-128">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="32d9f-129">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-129">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="32d9f-130">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-130">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="32d9f-131">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="32d9f-131">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="32d9f-132">Habilitação</span><span class="sxs-lookup"><span data-stu-id="32d9f-132">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="32d9f-133">Opções de disponibilidade do registro</span><span class="sxs-lookup"><span data-stu-id="32d9f-133">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="32d9f-134">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="32d9f-134">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="32d9f-135">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="32d9f-135">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="32d9f-136">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="32d9f-136">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="32d9f-137">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="32d9f-137">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="32d9f-138">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-138">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="32d9f-139">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-139">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="32d9f-140">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-140">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="32d9f-141">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-141">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="32d9f-142">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-142">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="32d9f-143">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="32d9f-143">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="32d9f-144">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="32d9f-144">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="32d9f-145">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="32d9f-145">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="32d9f-146">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="32d9f-146">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="32d9f-147">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="32d9f-147">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="32d9f-148">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="32d9f-148">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="32d9f-149">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="32d9f-149">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="32d9f-150">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="32d9f-150">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="32d9f-151">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="32d9f-151">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="32d9f-152">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="32d9f-152">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="32d9f-153">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="32d9f-153">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="32d9f-154">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="32d9f-154">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="32d9f-155">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="32d9f-155">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="32d9f-156">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="32d9f-156">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="32d9f-157">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="32d9f-157">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="32d9f-158">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="32d9f-158">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="32d9f-159">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="32d9f-159">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="32d9f-160">Report</span><span class="sxs-lookup"><span data-stu-id="32d9f-160">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="32d9f-161">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="32d9f-161">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="32d9f-162">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="32d9f-162">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="32d9f-163">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="32d9f-163">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="32d9f-164">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="32d9f-164">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="32d9f-165">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="32d9f-165">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="32d9f-166">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="32d9f-166">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="32d9f-167">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="32d9f-167">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="32d9f-168">URI</span><span class="sxs-lookup"><span data-stu-id="32d9f-168">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="32d9f-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="32d9f-169">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="32d9f-170">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="32d9f-170">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="32d9f-171">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="32d9f-171">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="32d9f-172">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="32d9f-172">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="32d9f-173">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="32d9f-173">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="32d9f-174">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="32d9f-174">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="32d9f-175">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="32d9f-175">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="32d9f-176">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="32d9f-176">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="32d9f-177">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="32d9f-177">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="32d9f-178">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="32d9f-178">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="32d9f-179">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="32d9f-179">Windows update state</span></span>](intune-shared-windowsupdatestate.md)

