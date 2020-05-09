---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 2d138f4c92999477054e8fe154c426fd18181037
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178091"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="c70f2-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c70f2-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="c70f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c70f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c70f2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c70f2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c70f2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c70f2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c70f2-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c70f2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c70f2-108">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="c70f2-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="c70f2-109">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="c70f2-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="c70f2-110">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="c70f2-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="c70f2-111">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="c70f2-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="c70f2-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="c70f2-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="c70f2-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="c70f2-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="c70f2-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="c70f2-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="c70f2-115">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="c70f2-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="c70f2-116">Configurações de atribuição de aplicativo repositório gerenciado do Android</span><span class="sxs-lookup"><span data-stu-id="c70f2-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="c70f2-117">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="c70f2-117">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="c70f2-118">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="c70f2-118">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="c70f2-119">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="c70f2-119">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="c70f2-120">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="c70f2-120">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="c70f2-121">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-121">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="c70f2-122">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-122">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="c70f2-123">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-123">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="c70f2-124">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-124">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="c70f2-125">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-125">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="c70f2-126">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-126">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="c70f2-127">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-127">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="c70f2-128">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c70f2-128">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="c70f2-129">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c70f2-129">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="c70f2-130">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-130">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="c70f2-131">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-131">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="c70f2-132">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c70f2-132">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="c70f2-133">Habilitação</span><span class="sxs-lookup"><span data-stu-id="c70f2-133">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="c70f2-134">Opções de disponibilidade do registro</span><span class="sxs-lookup"><span data-stu-id="c70f2-134">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="c70f2-135">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="c70f2-135">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="c70f2-136">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="c70f2-136">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="c70f2-137">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="c70f2-137">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="c70f2-138">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="c70f2-138">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="c70f2-139">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-139">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="c70f2-140">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-140">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="c70f2-141">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-141">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="c70f2-142">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-142">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="c70f2-143">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-143">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="c70f2-144">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="c70f2-144">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="c70f2-145">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="c70f2-145">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="c70f2-146">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="c70f2-146">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="c70f2-147">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="c70f2-147">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="c70f2-148">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="c70f2-148">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="c70f2-149">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="c70f2-149">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="c70f2-150">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="c70f2-150">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="c70f2-151">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="c70f2-151">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="c70f2-152">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="c70f2-152">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="c70f2-153">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="c70f2-153">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="c70f2-154">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c70f2-154">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="c70f2-155">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c70f2-155">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="c70f2-156">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c70f2-156">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="c70f2-157">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c70f2-157">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="c70f2-158">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="c70f2-158">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="c70f2-159">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="c70f2-159">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="c70f2-160">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="c70f2-160">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="c70f2-161">Report</span><span class="sxs-lookup"><span data-stu-id="c70f2-161">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="c70f2-162">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="c70f2-162">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="c70f2-163">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="c70f2-163">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="c70f2-164">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="c70f2-164">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="c70f2-165">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="c70f2-165">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="c70f2-166">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="c70f2-166">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="c70f2-167">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="c70f2-167">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="c70f2-168">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="c70f2-168">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="c70f2-169">URI</span><span class="sxs-lookup"><span data-stu-id="c70f2-169">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="c70f2-170">Usuário</span><span class="sxs-lookup"><span data-stu-id="c70f2-170">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="c70f2-171">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="c70f2-171">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="c70f2-172">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="c70f2-172">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="c70f2-173">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c70f2-173">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="c70f2-174">Prioridade de otimização de entrega do aplicativo LOB Win32</span><span class="sxs-lookup"><span data-stu-id="c70f2-174">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="c70f2-175">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c70f2-175">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="c70f2-176">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c70f2-176">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="c70f2-177">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="c70f2-177">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="c70f2-178">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c70f2-178">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="c70f2-179">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="c70f2-179">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="c70f2-180">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="c70f2-180">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="c70f2-181">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="c70f2-181">Windows update state</span></span>](intune-shared-windowsupdatestate.md)