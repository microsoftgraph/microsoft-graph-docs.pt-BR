---
title: Recursos compartilhados no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que dão suporte a vários fluxos de trabalho para uma organização de locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 80528f0ad7ab587e6945543e03225d112d958604
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271930"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="5bc6a-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5bc6a-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="5bc6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bc6a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bc6a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bc6a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bc6a-108">Esses pontos de extremidade são usados em vários fluxos de trabalho do Microsoft Graph API para o Intune.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="5bc6a-109">A intenção, finalidade e permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="5bc6a-110">Além disso, determinados métodos, propriedades e ações têm suporte apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="5bc6a-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="5bc6a-111">Os seguintes recursos de gráfico são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="5bc6a-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="5bc6a-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="5bc6a-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="5bc6a-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="5bc6a-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="5bc6a-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="5bc6a-115">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="5bc6a-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="5bc6a-116">Configurações de atribuição de aplicativo repositório gerenciado do Android</span><span class="sxs-lookup"><span data-stu-id="5bc6a-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-117">Armazenamento de destino de certificados</span><span class="sxs-lookup"><span data-stu-id="5bc6a-117">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="5bc6a-118">Repositório de certificados</span><span class="sxs-lookup"><span data-stu-id="5bc6a-118">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="5bc6a-119">Escala de período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="5bc6a-119">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="5bc6a-120">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="5bc6a-120">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="5bc6a-121">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="5bc6a-121">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="5bc6a-122">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="5bc6a-122">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="5bc6a-123">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-123">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="5bc6a-124">Origem da atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-124">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="5bc6a-125">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-125">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="5bc6a-126">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-126">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="5bc6a-127">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-127">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="5bc6a-128">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-128">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="5bc6a-129">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-129">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="5bc6a-130">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-130">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="5bc6a-131">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-131">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="5bc6a-132">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-132">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="5bc6a-133">Configurações de credenciais derivadas de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-133">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="5bc6a-134">Relatórios de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5bc6a-134">Device management reports</span></span>](intune-shared-devicemanagementreports.md)
- [<span data-ttu-id="5bc6a-135">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-135">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="5bc6a-136">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-136">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="5bc6a-137">Tipo de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-137">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="5bc6a-138">Habilitação</span><span class="sxs-lookup"><span data-stu-id="5bc6a-138">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="5bc6a-139">Opções de disponibilidade do registro</span><span class="sxs-lookup"><span data-stu-id="5bc6a-139">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="5bc6a-140">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="5bc6a-140">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="5bc6a-141">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="5bc6a-141">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="5bc6a-142">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="5bc6a-142">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="5bc6a-143">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="5bc6a-143">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="5bc6a-144">Algoritmos hash</span><span class="sxs-lookup"><span data-stu-id="5bc6a-144">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="5bc6a-145">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="5bc6a-145">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="5bc6a-146">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-146">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-147">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-147">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="5bc6a-148">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-148">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="5bc6a-149">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-149">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-150">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-150">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-151">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="5bc6a-151">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="5bc6a-152">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="5bc6a-152">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="5bc6a-153">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="5bc6a-153">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="5bc6a-154">Tamanho da chave</span><span class="sxs-lookup"><span data-stu-id="5bc6a-154">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="5bc6a-155">Opção de provedor de armazenamento de chaves</span><span class="sxs-lookup"><span data-stu-id="5bc6a-155">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="5bc6a-156">Usos de chave</span><span class="sxs-lookup"><span data-stu-id="5bc6a-156">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="5bc6a-157">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="5bc6a-157">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="5bc6a-158">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="5bc6a-158">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-159">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc6a-159">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="5bc6a-160">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="5bc6a-160">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="5bc6a-161">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="5bc6a-161">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="5bc6a-162">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="5bc6a-162">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-163">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="5bc6a-163">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="5bc6a-164">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5bc6a-164">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="5bc6a-165">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5bc6a-165">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-166">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5bc6a-166">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="5bc6a-167">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5bc6a-167">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="5bc6a-168">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="5bc6a-168">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="5bc6a-169">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="5bc6a-169">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="5bc6a-170">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="5bc6a-170">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="5bc6a-171">Report</span><span class="sxs-lookup"><span data-stu-id="5bc6a-171">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="5bc6a-172">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="5bc6a-172">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="5bc6a-173">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="5bc6a-173">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="5bc6a-174">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="5bc6a-174">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="5bc6a-175">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="5bc6a-175">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="5bc6a-176">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="5bc6a-176">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="5bc6a-177">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="5bc6a-177">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="5bc6a-178">Tipo de fonte de configuração</span><span class="sxs-lookup"><span data-stu-id="5bc6a-178">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="5bc6a-179">Tipo de nome alternativo da entidade</span><span class="sxs-lookup"><span data-stu-id="5bc6a-179">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="5bc6a-180">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc6a-180">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="5bc6a-181">URI</span><span class="sxs-lookup"><span data-stu-id="5bc6a-181">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="5bc6a-182">Usuário</span><span class="sxs-lookup"><span data-stu-id="5bc6a-182">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="5bc6a-183">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="5bc6a-183">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="5bc6a-184">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="5bc6a-184">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="5bc6a-185">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5bc6a-185">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-186">Prioridade de otimização de entrega do aplicativo LOB Win32</span><span class="sxs-lookup"><span data-stu-id="5bc6a-186">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="5bc6a-187">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5bc6a-187">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="5bc6a-188">Configurações de reinicialização de aplicativos LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5bc6a-188">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="5bc6a-189">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="5bc6a-189">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-190">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="5bc6a-190">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="5bc6a-191">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="5bc6a-191">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="5bc6a-192">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="5bc6a-192">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="5bc6a-193">Estado do Windows Update</span><span class="sxs-lookup"><span data-stu-id="5bc6a-193">Windows update state</span></span>](intune-shared-windowsupdatestate.md)