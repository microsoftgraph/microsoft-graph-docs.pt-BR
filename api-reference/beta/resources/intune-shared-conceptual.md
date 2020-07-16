---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 06be7eefad204f0cef73d8c0d16d70159f9142db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793756"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="7dd89-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7dd89-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="7dd89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dd89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dd89-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7dd89-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dd89-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7dd89-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dd89-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dd89-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dd89-108">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="7dd89-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="7dd89-109">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="7dd89-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="7dd89-110">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="7dd89-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="7dd89-111">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="7dd89-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="7dd89-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="7dd89-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="7dd89-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="7dd89-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="7dd89-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="7dd89-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="7dd89-115">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="7dd89-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="7dd89-116">Configurações de atribuição de aplicativo repositório gerenciado do Android</span><span class="sxs-lookup"><span data-stu-id="7dd89-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="7dd89-117">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="7dd89-117">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="7dd89-118">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="7dd89-118">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="7dd89-119">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="7dd89-119">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="7dd89-120">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="7dd89-120">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="7dd89-121">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="7dd89-121">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="7dd89-122">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-122">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="7dd89-123">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-123">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="7dd89-124">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-124">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="7dd89-125">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-125">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="7dd89-126">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-126">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="7dd89-127">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-127">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="7dd89-128">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-128">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="7dd89-129">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7dd89-129">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="7dd89-130">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7dd89-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="7dd89-131">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="7dd89-132">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="7dd89-133">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7dd89-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="7dd89-134">Habilitação</span><span class="sxs-lookup"><span data-stu-id="7dd89-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="7dd89-135">Opções de disponibilidade do registro</span><span class="sxs-lookup"><span data-stu-id="7dd89-135">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="7dd89-136">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="7dd89-136">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="7dd89-137">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="7dd89-137">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="7dd89-138">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="7dd89-138">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="7dd89-139">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="7dd89-139">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="7dd89-140">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-140">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="7dd89-141">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-141">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="7dd89-142">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-142">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="7dd89-143">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-143">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="7dd89-144">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-144">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="7dd89-145">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="7dd89-145">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="7dd89-146">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="7dd89-146">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="7dd89-147">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="7dd89-147">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="7dd89-148">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="7dd89-148">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="7dd89-149">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="7dd89-149">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="7dd89-150">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="7dd89-150">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="7dd89-151">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="7dd89-151">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="7dd89-152">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="7dd89-152">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="7dd89-153">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="7dd89-153">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="7dd89-154">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="7dd89-154">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="7dd89-155">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="7dd89-155">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="7dd89-156">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="7dd89-156">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="7dd89-157">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="7dd89-157">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="7dd89-158">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="7dd89-158">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="7dd89-159">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="7dd89-159">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="7dd89-160">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="7dd89-160">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="7dd89-161">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="7dd89-161">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="7dd89-162">Report</span><span class="sxs-lookup"><span data-stu-id="7dd89-162">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="7dd89-163">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="7dd89-163">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="7dd89-164">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="7dd89-164">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="7dd89-165">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="7dd89-165">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="7dd89-166">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="7dd89-166">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="7dd89-167">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="7dd89-167">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="7dd89-168">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="7dd89-168">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="7dd89-169">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="7dd89-169">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="7dd89-170">URI</span><span class="sxs-lookup"><span data-stu-id="7dd89-170">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="7dd89-171">Usuário</span><span class="sxs-lookup"><span data-stu-id="7dd89-171">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="7dd89-172">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="7dd89-172">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="7dd89-173">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="7dd89-173">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="7dd89-174">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="7dd89-174">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="7dd89-175">Prioridade de otimização de entrega do aplicativo LOB Win32</span><span class="sxs-lookup"><span data-stu-id="7dd89-175">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="7dd89-176">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="7dd89-176">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="7dd89-177">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="7dd89-177">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="7dd89-178">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="7dd89-178">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="7dd89-179">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="7dd89-179">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="7dd89-180">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="7dd89-180">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="7dd89-181">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="7dd89-181">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="7dd89-182">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="7dd89-182">Windows update state</span></span>](intune-shared-windowsupdatestate.md)