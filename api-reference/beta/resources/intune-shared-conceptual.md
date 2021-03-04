---
title: Recursos compartilhados no Microsoft Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para pontos de extremidade do Intune (REST) que suportam vários fluxos de trabalho para uma organização de locatários.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 6c0b11847ff5ec0f4431a20e4ffa197ddd21dbcf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440175"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="5c595-103">Recursos compartilhados no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5c595-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="5c595-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c595-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c595-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c595-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c595-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c595-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c595-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c595-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c595-108">Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="5c595-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="5c595-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="5c595-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="5c595-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="5c595-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="5c595-111">Os seguintes recursos do Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="5c595-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="5c595-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="5c595-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="5c595-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="5c595-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="5c595-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="5c595-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="5c595-115">Android enterprise sempre no tipo de pacote VPN</span><span class="sxs-lookup"><span data-stu-id="5c595-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="5c595-116">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="5c595-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="5c595-117">Configurações de atribuição de aplicativo de loja gerenciada do Android</span><span class="sxs-lookup"><span data-stu-id="5c595-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="5c595-118">Armazenamento de destino de certificados</span><span class="sxs-lookup"><span data-stu-id="5c595-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="5c595-119">Repositório de certificados</span><span class="sxs-lookup"><span data-stu-id="5c595-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="5c595-120">Escala de período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="5c595-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="5c595-121">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="5c595-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="5c595-122">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="5c595-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="5c595-123">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="5c595-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="5c595-124">Destino da atribuição da coleção configuration manager</span><span class="sxs-lookup"><span data-stu-id="5c595-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="5c595-125">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="5c595-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="5c595-126">Fonte de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="5c595-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="5c595-127">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="5c595-128">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="5c595-129">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="5c595-130">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="5c595-131">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="5c595-132">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="5c595-133">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="5c595-134">Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5c595-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="5c595-135">Configurações de credenciais derivadas do gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5c595-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="5c595-136">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-136">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="5c595-137">Tipo de plataforma do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c595-137">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="5c595-138">Habilitação</span><span class="sxs-lookup"><span data-stu-id="5c595-138">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="5c595-139">Opções de disponibilidade de registro</span><span class="sxs-lookup"><span data-stu-id="5c595-139">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="5c595-140">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="5c595-140">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="5c595-141">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="5c595-141">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="5c595-142">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="5c595-142">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="5c595-143">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="5c595-143">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="5c595-144">Algoritmos hash</span><span class="sxs-lookup"><span data-stu-id="5c595-144">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="5c595-145">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="5c595-145">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="5c595-146">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="5c595-146">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="5c595-147">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="5c595-147">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="5c595-148">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="5c595-148">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="5c595-149">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="5c595-149">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="5c595-150">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="5c595-150">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="5c595-151">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="5c595-151">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="5c595-152">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="5c595-152">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="5c595-153">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="5c595-153">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="5c595-154">Tamanho da chave</span><span class="sxs-lookup"><span data-stu-id="5c595-154">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="5c595-155">Opção de provedor de armazenamento de chaves</span><span class="sxs-lookup"><span data-stu-id="5c595-155">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="5c595-156">Usos de chave</span><span class="sxs-lookup"><span data-stu-id="5c595-156">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="5c595-157">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="5c595-157">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="5c595-158">Configurações de atribuição do aplicativo LOB do macOS</span><span class="sxs-lookup"><span data-stu-id="5c595-158">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="5c595-159">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="5c595-159">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="5c595-160">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5c595-160">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="5c595-161">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="5c595-161">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="5c595-162">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="5c595-162">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="5c595-163">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="5c595-163">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="5c595-164">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5c595-164">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="5c595-165">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5c595-165">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="5c595-166">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5c595-166">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="5c595-167">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="5c595-167">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="5c595-168">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="5c595-168">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="5c595-169">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="5c595-169">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="5c595-170">Report</span><span class="sxs-lookup"><span data-stu-id="5c595-170">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="5c595-171">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="5c595-171">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="5c595-172">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="5c595-172">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="5c595-173">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="5c595-173">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="5c595-174">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="5c595-174">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="5c595-175">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="5c595-175">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="5c595-176">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="5c595-176">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="5c595-177">Definindo o tipo de origem</span><span class="sxs-lookup"><span data-stu-id="5c595-177">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="5c595-178">Tipo de nome alternativo da entidade</span><span class="sxs-lookup"><span data-stu-id="5c595-178">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="5c595-179">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5c595-179">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="5c595-180">URI</span><span class="sxs-lookup"><span data-stu-id="5c595-180">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="5c595-181">Usuário</span><span class="sxs-lookup"><span data-stu-id="5c595-181">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="5c595-182">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="5c595-182">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="5c595-183">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="5c595-183">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="5c595-184">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5c595-184">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="5c595-185">Prioridade de otimização de entrega de aplicativos LOB win32</span><span class="sxs-lookup"><span data-stu-id="5c595-185">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="5c595-186">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5c595-186">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="5c595-187">Configurações de reinicialização do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="5c595-187">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="5c595-188">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="5c595-188">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="5c595-189">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="5c595-189">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="5c595-190">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="5c595-190">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="5c595-191">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="5c595-191">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="5c595-192">Estado de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="5c595-192">Windows update state</span></span>](intune-shared-windowsupdatestate.md)