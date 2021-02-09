---
title: Recursos compartilhados no Microsoft Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para pontos de extremidade do Intune (REST) que suportam vários fluxos de trabalho para uma organização locatária.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 07f408cfc4157dd4ad415a71b19367ce0ce6ddfa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156732"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="446ed-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="446ed-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="446ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="446ed-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="446ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="446ed-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="446ed-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="446ed-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="446ed-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="446ed-108">Esses pontos de extremidade são usados em várias APIs do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="446ed-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="446ed-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso variam de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="446ed-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="446ed-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="446ed-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="446ed-111">Os seguintes recursos do Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="446ed-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="446ed-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="446ed-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="446ed-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="446ed-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="446ed-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="446ed-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="446ed-115">Tipo de pacote VPN always on enterprise do Android</span><span class="sxs-lookup"><span data-stu-id="446ed-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="446ed-116">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="446ed-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="446ed-117">Configurações de atribuição de aplicativo do armazenamento gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="446ed-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="446ed-118">Armazenamento de destino de certificados</span><span class="sxs-lookup"><span data-stu-id="446ed-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="446ed-119">Repositório de certificados</span><span class="sxs-lookup"><span data-stu-id="446ed-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="446ed-120">Escala de período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="446ed-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="446ed-121">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="446ed-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="446ed-122">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="446ed-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="446ed-123">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="446ed-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="446ed-124">Destino de atribuição de coleção do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="446ed-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="446ed-125">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="446ed-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="446ed-126">Fonte de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="446ed-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="446ed-127">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="446ed-128">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="446ed-129">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="446ed-130">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="446ed-131">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="446ed-132">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="446ed-133">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="446ed-134">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="446ed-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="446ed-135">Configurações de credencial derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="446ed-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="446ed-136">Relatórios de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="446ed-136">Device management reports</span></span>](intune-shared-devicemanagementreports.md)
- [<span data-ttu-id="446ed-137">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-137">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="446ed-138">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-138">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="446ed-139">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="446ed-139">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="446ed-140">Habilitação</span><span class="sxs-lookup"><span data-stu-id="446ed-140">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="446ed-141">Opções de disponibilidade de registro</span><span class="sxs-lookup"><span data-stu-id="446ed-141">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="446ed-142">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="446ed-142">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="446ed-143">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="446ed-143">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="446ed-144">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="446ed-144">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="446ed-145">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="446ed-145">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="446ed-146">Algoritmos hash</span><span class="sxs-lookup"><span data-stu-id="446ed-146">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="446ed-147">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="446ed-147">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="446ed-148">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="446ed-148">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="446ed-149">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="446ed-149">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="446ed-150">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="446ed-150">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="446ed-151">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="446ed-151">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="446ed-152">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="446ed-152">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="446ed-153">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="446ed-153">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="446ed-154">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="446ed-154">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="446ed-155">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="446ed-155">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="446ed-156">Tamanho da chave</span><span class="sxs-lookup"><span data-stu-id="446ed-156">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="446ed-157">Opção de provedor de armazenamento de chaves</span><span class="sxs-lookup"><span data-stu-id="446ed-157">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="446ed-158">Usos de chave</span><span class="sxs-lookup"><span data-stu-id="446ed-158">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="446ed-159">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="446ed-159">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="446ed-160">Configurações de atribuição do aplicativo LOB do macOS</span><span class="sxs-lookup"><span data-stu-id="446ed-160">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="446ed-161">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="446ed-161">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="446ed-162">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="446ed-162">Managed device</span></span>](intune-shared-manageddevice.md)
- [<span data-ttu-id="446ed-163">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="446ed-163">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="446ed-164">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="446ed-164">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="446ed-165">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="446ed-165">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="446ed-166">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="446ed-166">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="446ed-167">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="446ed-167">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="446ed-168">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="446ed-168">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="446ed-169">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="446ed-169">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="446ed-170">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="446ed-170">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="446ed-171">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="446ed-171">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="446ed-172">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="446ed-172">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="446ed-173">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="446ed-173">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="446ed-174">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="446ed-174">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="446ed-175">Report</span><span class="sxs-lookup"><span data-stu-id="446ed-175">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="446ed-176">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="446ed-176">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="446ed-177">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="446ed-177">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="446ed-178">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="446ed-178">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="446ed-179">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="446ed-179">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="446ed-180">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="446ed-180">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="446ed-181">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="446ed-181">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="446ed-182">Configurando o tipo de fonte</span><span class="sxs-lookup"><span data-stu-id="446ed-182">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="446ed-183">Tipo de nome alternativo da entidade</span><span class="sxs-lookup"><span data-stu-id="446ed-183">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="446ed-184">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="446ed-184">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="446ed-185">URI</span><span class="sxs-lookup"><span data-stu-id="446ed-185">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="446ed-186">Usuário</span><span class="sxs-lookup"><span data-stu-id="446ed-186">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="446ed-187">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="446ed-187">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="446ed-188">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="446ed-188">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="446ed-189">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="446ed-189">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="446ed-190">Prioridade de otimização de entrega de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="446ed-190">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="446ed-191">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="446ed-191">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="446ed-192">Configurações de reinicialização do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="446ed-192">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="446ed-193">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="446ed-193">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="446ed-194">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="446ed-194">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="446ed-195">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="446ed-195">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="446ed-196">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="446ed-196">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="446ed-197">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="446ed-197">Windows update state</span></span>](intune-shared-windowsupdatestate.md)