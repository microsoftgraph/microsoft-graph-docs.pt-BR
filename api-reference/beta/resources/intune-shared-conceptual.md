---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 9a5a6ee1a9111f85d041821e8e5917c0b007698d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160337"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="c9b95-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c9b95-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="c9b95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9b95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9b95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9b95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9b95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b95-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="c9b95-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="c9b95-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="c9b95-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="c9b95-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="c9b95-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="c9b95-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="c9b95-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="c9b95-111">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="c9b95-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="c9b95-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="c9b95-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="c9b95-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="c9b95-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="c9b95-114">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="c9b95-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="c9b95-115">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="c9b95-115">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="c9b95-116">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="c9b95-116">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="c9b95-117">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="c9b95-117">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="c9b95-118">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="c9b95-118">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="c9b95-119">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-119">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="c9b95-120">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-120">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="c9b95-121">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-121">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="c9b95-122">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-122">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="c9b95-123">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-123">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="c9b95-124">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-124">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="c9b95-125">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-125">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="c9b95-126">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c9b95-126">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="c9b95-127">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c9b95-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="c9b95-128">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="c9b95-129">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="c9b95-130">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9b95-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="c9b95-131">Habilitação</span><span class="sxs-lookup"><span data-stu-id="c9b95-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="c9b95-132">Opções de disponibilidade do registro</span><span class="sxs-lookup"><span data-stu-id="c9b95-132">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="c9b95-133">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="c9b95-133">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="c9b95-134">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="c9b95-134">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="c9b95-135">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="c9b95-135">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="c9b95-136">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="c9b95-136">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="c9b95-137">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-137">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="c9b95-138">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-138">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="c9b95-139">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-139">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="c9b95-140">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-140">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="c9b95-141">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-141">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="c9b95-142">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="c9b95-142">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="c9b95-143">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="c9b95-143">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="c9b95-144">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="c9b95-144">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="c9b95-145">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="c9b95-145">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="c9b95-146">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="c9b95-146">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="c9b95-147">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="c9b95-147">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="c9b95-148">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="c9b95-148">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="c9b95-149">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="c9b95-149">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="c9b95-150">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="c9b95-150">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="c9b95-151">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="c9b95-151">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="c9b95-152">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c9b95-152">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="c9b95-153">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c9b95-153">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="c9b95-154">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c9b95-154">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="c9b95-155">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="c9b95-155">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="c9b95-156">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="c9b95-156">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="c9b95-157">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="c9b95-157">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="c9b95-158">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="c9b95-158">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="c9b95-159">Report</span><span class="sxs-lookup"><span data-stu-id="c9b95-159">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="c9b95-160">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="c9b95-160">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="c9b95-161">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="c9b95-161">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="c9b95-162">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="c9b95-162">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="c9b95-163">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="c9b95-163">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="c9b95-164">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="c9b95-164">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="c9b95-165">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="c9b95-165">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="c9b95-166">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="c9b95-166">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="c9b95-167">URI</span><span class="sxs-lookup"><span data-stu-id="c9b95-167">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="c9b95-168">Usuário</span><span class="sxs-lookup"><span data-stu-id="c9b95-168">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="c9b95-169">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="c9b95-169">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="c9b95-170">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="c9b95-170">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="c9b95-171">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c9b95-171">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="c9b95-172">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c9b95-172">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="c9b95-173">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="c9b95-173">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="c9b95-174">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="c9b95-174">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="c9b95-175">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c9b95-175">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="c9b95-176">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="c9b95-176">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="c9b95-177">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="c9b95-177">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="c9b95-178">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="c9b95-178">Windows update state</span></span>](intune-shared-windowsupdatestate.md)

