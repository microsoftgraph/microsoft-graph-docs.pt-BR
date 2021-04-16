---
title: Recursos compartilhados no Microsoft Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para pontos de extremidade do Intune (REST) que suportam vários fluxos de trabalho para uma organização de locatários.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 4de0e8477d7d20894981c0d0e68956d806d926c4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866143"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="3357c-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3357c-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="3357c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3357c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3357c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3357c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3357c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3357c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3357c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3357c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3357c-108">Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="3357c-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="3357c-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="3357c-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="3357c-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="3357c-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="3357c-111">Os seguintes recursos do Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="3357c-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="3357c-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="3357c-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="3357c-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="3357c-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="3357c-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="3357c-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="3357c-115">Android enterprise sempre no tipo de pacote VPN</span><span class="sxs-lookup"><span data-stu-id="3357c-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="3357c-116">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="3357c-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="3357c-117">Configurações de atribuição de aplicativo de loja gerenciada do Android</span><span class="sxs-lookup"><span data-stu-id="3357c-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="3357c-118">Armazenamento de destino de certificados</span><span class="sxs-lookup"><span data-stu-id="3357c-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="3357c-119">Repositório de certificados</span><span class="sxs-lookup"><span data-stu-id="3357c-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="3357c-120">Escala de período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="3357c-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="3357c-121">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="3357c-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="3357c-122">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="3357c-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="3357c-123">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="3357c-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="3357c-124">Destino da atribuição da coleção configuration manager</span><span class="sxs-lookup"><span data-stu-id="3357c-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="3357c-125">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="3357c-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="3357c-126">Fonte de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="3357c-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="3357c-127">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="3357c-128">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="3357c-129">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="3357c-130">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="3357c-131">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="3357c-132">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="3357c-133">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="3357c-134">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="3357c-135">Configurações de credenciais derivadas do gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3357c-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="3357c-136">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-136">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="3357c-137">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3357c-137">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="3357c-138">Habilitação</span><span class="sxs-lookup"><span data-stu-id="3357c-138">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="3357c-139">Opções de disponibilidade de registro</span><span class="sxs-lookup"><span data-stu-id="3357c-139">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="3357c-140">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="3357c-140">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="3357c-141">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="3357c-141">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="3357c-142">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="3357c-142">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="3357c-143">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="3357c-143">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="3357c-144">Algoritmos hash</span><span class="sxs-lookup"><span data-stu-id="3357c-144">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="3357c-145">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="3357c-145">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="3357c-146">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="3357c-146">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="3357c-147">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="3357c-147">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="3357c-148">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="3357c-148">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="3357c-149">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="3357c-149">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="3357c-150">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="3357c-150">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="3357c-151">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="3357c-151">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="3357c-152">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="3357c-152">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="3357c-153">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="3357c-153">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="3357c-154">Tamanho da chave</span><span class="sxs-lookup"><span data-stu-id="3357c-154">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="3357c-155">Opção de provedor de armazenamento de chaves</span><span class="sxs-lookup"><span data-stu-id="3357c-155">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="3357c-156">Usos de chave</span><span class="sxs-lookup"><span data-stu-id="3357c-156">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="3357c-157">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="3357c-157">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="3357c-158">Configurações de atribuição do aplicativo LOB do macOS</span><span class="sxs-lookup"><span data-stu-id="3357c-158">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="3357c-159">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="3357c-159">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="3357c-160">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3357c-160">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="3357c-161">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="3357c-161">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="3357c-162">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="3357c-162">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="3357c-163">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="3357c-163">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="3357c-164">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="3357c-164">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="3357c-165">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="3357c-165">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="3357c-166">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="3357c-166">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="3357c-167">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="3357c-167">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="3357c-168">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="3357c-168">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="3357c-169">Tipo de plataforma da política</span><span class="sxs-lookup"><span data-stu-id="3357c-169">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="3357c-170">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="3357c-170">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="3357c-171">Report</span><span class="sxs-lookup"><span data-stu-id="3357c-171">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="3357c-172">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="3357c-172">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="3357c-173">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="3357c-173">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="3357c-174">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="3357c-174">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="3357c-175">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="3357c-175">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="3357c-176">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="3357c-176">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="3357c-177">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="3357c-177">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="3357c-178">Definindo o tipo de origem</span><span class="sxs-lookup"><span data-stu-id="3357c-178">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="3357c-179">Tipo de nome alternativo da entidade</span><span class="sxs-lookup"><span data-stu-id="3357c-179">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="3357c-180">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="3357c-180">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="3357c-181">URI</span><span class="sxs-lookup"><span data-stu-id="3357c-181">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="3357c-182">Usuário</span><span class="sxs-lookup"><span data-stu-id="3357c-182">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="3357c-183">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="3357c-183">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="3357c-184">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="3357c-184">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="3357c-185">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="3357c-185">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="3357c-186">Prioridade de otimização de entrega de aplicativos LOB win32</span><span class="sxs-lookup"><span data-stu-id="3357c-186">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="3357c-187">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="3357c-187">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="3357c-188">Configurações de reinicialização do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="3357c-188">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="3357c-189">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="3357c-189">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="3357c-190">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="3357c-190">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="3357c-191">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="3357c-191">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="3357c-192">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="3357c-192">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="3357c-193">Estado de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="3357c-193">Windows update state</span></span>](intune-shared-windowsupdatestate.md)