---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: e1b613dc9140e597dc9eb0c74448f227cf940ba5
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636823"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="84af2-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="84af2-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="84af2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84af2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84af2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84af2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84af2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84af2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84af2-107">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="84af2-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="84af2-108">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="84af2-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="84af2-109">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="84af2-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="84af2-110">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="84af2-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="84af2-111">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="84af2-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="84af2-112">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="84af2-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="84af2-113">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="84af2-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="84af2-114">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="84af2-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="84af2-115">Tipo de rotação da senha de recuperação do BitLocker</span><span class="sxs-lookup"><span data-stu-id="84af2-115">BitLocker recovery password rotation type</span></span>](intune-shared-bitlockerrecoverypasswordrotationtype.md)
- [<span data-ttu-id="84af2-116">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="84af2-116">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="84af2-117">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="84af2-117">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="84af2-118">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="84af2-118">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="84af2-119">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="84af2-119">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="84af2-120">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-120">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="84af2-121">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-121">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="84af2-122">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-122">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="84af2-123">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-123">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="84af2-124">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-124">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="84af2-125">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-125">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="84af2-126">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-126">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="84af2-127">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="84af2-127">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="84af2-128">Emissor de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="84af2-128">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="84af2-129">Tipo de notificação de credencial derivada de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-129">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="84af2-130">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="84af2-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="84af2-131">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="84af2-132">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="84af2-133">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="84af2-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="84af2-134">Habilitação</span><span class="sxs-lookup"><span data-stu-id="84af2-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="84af2-135">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="84af2-135">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="84af2-136">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="84af2-136">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="84af2-137">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="84af2-137">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="84af2-138">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="84af2-138">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="84af2-139">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="84af2-139">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="84af2-140">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="84af2-140">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="84af2-141">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="84af2-141">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="84af2-142">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="84af2-142">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="84af2-143">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="84af2-143">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="84af2-144">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="84af2-144">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="84af2-145">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="84af2-145">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="84af2-146">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="84af2-146">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="84af2-147">Par de valores booleanos principais</span><span class="sxs-lookup"><span data-stu-id="84af2-147">Key boolean value pair</span></span>](intune-shared-keybooleanvaluepair.md)
- [<span data-ttu-id="84af2-148">Par principal de valor inteiro</span><span class="sxs-lookup"><span data-stu-id="84af2-148">Key integer value pair</span></span>](intune-shared-keyintegervaluepair.md)
- [<span data-ttu-id="84af2-149">Par chave real de valor</span><span class="sxs-lookup"><span data-stu-id="84af2-149">Key real value pair</span></span>](intune-shared-keyrealvaluepair.md)
- [<span data-ttu-id="84af2-150">Par de valores de cadeia de caracteres de chave</span><span class="sxs-lookup"><span data-stu-id="84af2-150">Key string value pair</span></span>](intune-shared-keystringvaluepair.md)
- [<span data-ttu-id="84af2-151">Par de valores digitados por chave</span><span class="sxs-lookup"><span data-stu-id="84af2-151">Key typed value pair</span></span>](intune-shared-keytypedvaluepair.md)
- [<span data-ttu-id="84af2-152">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="84af2-152">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="84af2-153">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="84af2-153">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="84af2-154">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="84af2-154">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="84af2-155">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="84af2-155">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="84af2-156">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="84af2-156">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="84af2-157">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="84af2-157">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="84af2-158">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="84af2-158">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="84af2-159">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="84af2-159">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="84af2-160">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="84af2-160">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="84af2-161">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="84af2-161">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="84af2-162">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="84af2-162">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="84af2-163">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="84af2-163">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="84af2-164">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="84af2-164">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="84af2-165">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="84af2-165">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="84af2-166">Report</span><span class="sxs-lookup"><span data-stu-id="84af2-166">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="84af2-167">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="84af2-167">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="84af2-168">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="84af2-168">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="84af2-169">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="84af2-169">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="84af2-170">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="84af2-170">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="84af2-171">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="84af2-171">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="84af2-172">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="84af2-172">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="84af2-173">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="84af2-173">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="84af2-174">URI</span><span class="sxs-lookup"><span data-stu-id="84af2-174">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="84af2-175">Usuário</span><span class="sxs-lookup"><span data-stu-id="84af2-175">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="84af2-176">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="84af2-176">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="84af2-177">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="84af2-177">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="84af2-178">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="84af2-178">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="84af2-179">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="84af2-179">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="84af2-180">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="84af2-180">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="84af2-181">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="84af2-181">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="84af2-182">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="84af2-182">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="84af2-183">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="84af2-183">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="84af2-184">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="84af2-184">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="84af2-185">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="84af2-185">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="84af2-186">Status do Windows Update</span><span class="sxs-lookup"><span data-stu-id="84af2-186">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

