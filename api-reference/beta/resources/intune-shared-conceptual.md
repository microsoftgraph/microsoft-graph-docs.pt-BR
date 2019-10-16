---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 1420f751866224905f1636205de173e3bd117451
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539166"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ee535-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ee535-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="ee535-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee535-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee535-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee535-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee535-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee535-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee535-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="ee535-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ee535-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="ee535-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ee535-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="ee535-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ee535-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="ee535-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="ee535-111">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="ee535-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="ee535-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="ee535-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ee535-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="ee535-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ee535-114">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="ee535-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="ee535-115">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="ee535-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ee535-116">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="ee535-116">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="ee535-117">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ee535-118">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ee535-119">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ee535-120">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-120">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="ee535-121">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-121">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="ee535-122">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-122">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="ee535-123">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-123">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="ee535-124">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ee535-124">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ee535-125">Emissor de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ee535-125">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="ee535-126">Tipo de notificação de credencial derivada de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-126">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="ee535-127">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ee535-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="ee535-128">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="ee535-129">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="ee535-130">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee535-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="ee535-131">Habilitação</span><span class="sxs-lookup"><span data-stu-id="ee535-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="ee535-132">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="ee535-132">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="ee535-133">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="ee535-133">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ee535-134">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="ee535-134">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ee535-135">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="ee535-135">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ee535-136">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="ee535-136">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="ee535-137">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="ee535-137">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="ee535-138">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="ee535-138">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="ee535-139">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="ee535-139">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="ee535-140">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="ee535-140">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="ee535-141">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="ee535-141">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="ee535-142">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="ee535-142">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="ee535-143">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="ee535-143">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="ee535-144">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="ee535-144">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="ee535-145">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="ee535-145">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="ee535-146">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="ee535-146">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="ee535-147">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="ee535-147">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ee535-148">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="ee535-148">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="ee535-149">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="ee535-149">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ee535-150">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="ee535-150">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="ee535-151">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="ee535-151">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="ee535-152">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="ee535-152">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="ee535-153">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="ee535-153">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="ee535-154">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="ee535-154">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="ee535-155">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="ee535-155">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="ee535-156">Report</span><span class="sxs-lookup"><span data-stu-id="ee535-156">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ee535-157">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="ee535-157">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ee535-158">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="ee535-158">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="ee535-159">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="ee535-159">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="ee535-160">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="ee535-160">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="ee535-161">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="ee535-161">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="ee535-162">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="ee535-162">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ee535-163">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="ee535-163">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="ee535-164">URI</span><span class="sxs-lookup"><span data-stu-id="ee535-164">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ee535-165">Usuário</span><span class="sxs-lookup"><span data-stu-id="ee535-165">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ee535-166">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="ee535-166">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="ee535-167">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="ee535-167">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="ee535-168">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="ee535-168">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="ee535-169">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="ee535-169">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="ee535-170">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="ee535-170">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="ee535-171">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ee535-171">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="ee535-172">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ee535-172">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ee535-173">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="ee535-173">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="ee535-174">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="ee535-174">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="ee535-175">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="ee535-175">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="ee535-176">Status do Windows Update</span><span class="sxs-lookup"><span data-stu-id="ee535-176">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

