---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 56950c21527c4bf72dd57e71d27f0b1be2e47046
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196340"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="17ecd-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="17ecd-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="17ecd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17ecd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17ecd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17ecd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17ecd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17ecd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17ecd-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="17ecd-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="17ecd-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="17ecd-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="17ecd-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="17ecd-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="17ecd-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="17ecd-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="17ecd-111">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="17ecd-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="17ecd-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="17ecd-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="17ecd-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="17ecd-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="17ecd-114">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="17ecd-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="17ecd-115">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="17ecd-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="17ecd-116">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="17ecd-116">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="17ecd-117">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="17ecd-118">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="17ecd-119">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="17ecd-120">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-120">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="17ecd-121">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-121">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="17ecd-122">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-122">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="17ecd-123">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-123">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="17ecd-124">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="17ecd-124">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="17ecd-125">Emissor de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="17ecd-125">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="17ecd-126">Tipo de notificação de credencial derivada de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-126">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="17ecd-127">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="17ecd-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="17ecd-128">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="17ecd-129">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="17ecd-130">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="17ecd-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="17ecd-131">Habilitação</span><span class="sxs-lookup"><span data-stu-id="17ecd-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="17ecd-132">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="17ecd-132">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="17ecd-133">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="17ecd-133">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="17ecd-134">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="17ecd-134">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="17ecd-135">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="17ecd-135">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="17ecd-136">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-136">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="17ecd-137">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-137">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="17ecd-138">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-138">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="17ecd-139">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-139">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="17ecd-140">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-140">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="17ecd-141">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="17ecd-141">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="17ecd-142">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="17ecd-142">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="17ecd-143">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="17ecd-143">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="17ecd-144">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="17ecd-144">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="17ecd-145">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="17ecd-145">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="17ecd-146">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="17ecd-146">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="17ecd-147">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="17ecd-147">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="17ecd-148">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="17ecd-148">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="17ecd-149">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="17ecd-149">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="17ecd-150">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="17ecd-150">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="17ecd-151">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="17ecd-151">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="17ecd-152">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="17ecd-152">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="17ecd-153">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="17ecd-153">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="17ecd-154">Report</span><span class="sxs-lookup"><span data-stu-id="17ecd-154">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="17ecd-155">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="17ecd-155">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="17ecd-156">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="17ecd-156">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="17ecd-157">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="17ecd-157">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="17ecd-158">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="17ecd-158">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="17ecd-159">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="17ecd-159">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="17ecd-160">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="17ecd-160">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="17ecd-161">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="17ecd-161">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="17ecd-162">URI</span><span class="sxs-lookup"><span data-stu-id="17ecd-162">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="17ecd-163">Usuário</span><span class="sxs-lookup"><span data-stu-id="17ecd-163">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="17ecd-164">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="17ecd-164">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="17ecd-165">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="17ecd-165">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="17ecd-166">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="17ecd-166">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="17ecd-167">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="17ecd-167">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="17ecd-168">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="17ecd-168">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="17ecd-169">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="17ecd-169">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="17ecd-170">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="17ecd-170">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="17ecd-171">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="17ecd-171">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="17ecd-172">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="17ecd-172">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="17ecd-173">Status do Windows Update</span><span class="sxs-lookup"><span data-stu-id="17ecd-173">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

