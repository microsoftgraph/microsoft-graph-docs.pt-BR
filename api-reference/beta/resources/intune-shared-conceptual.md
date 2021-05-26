---
title: Recursos compartilhados em Microsoft Intune - API Graph Microsoft
description: Lista a API Graph microsoft para pontos de extremidade do Intune (REST) que suportam vários fluxos de trabalho para uma organização de locatários.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 77500484aaafd5d9101e66789966b4861b61e511
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664899"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="d09fc-103">Recursos compartilhados em Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d09fc-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="d09fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d09fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d09fc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d09fc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d09fc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d09fc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d09fc-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d09fc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d09fc-108">Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.</span><span class="sxs-lookup"><span data-stu-id="d09fc-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="d09fc-109">A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.</span><span class="sxs-lookup"><span data-stu-id="d09fc-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="d09fc-110">Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.</span><span class="sxs-lookup"><span data-stu-id="d09fc-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="d09fc-111">Os seguintes Graph são compartilhados entre fluxos de trabalho do Intune:</span><span class="sxs-lookup"><span data-stu-id="d09fc-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="d09fc-112">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="d09fc-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="d09fc-113">Destino de atribuição de todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="d09fc-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="d09fc-114">Destino de atribuição de todos os usuários licenciados</span><span class="sxs-lookup"><span data-stu-id="d09fc-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d09fc-115">Android enterprise sempre no tipo de pacote VPN</span><span class="sxs-lookup"><span data-stu-id="d09fc-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="d09fc-116">Proteção de aplicativo gerenciado Android</span><span class="sxs-lookup"><span data-stu-id="d09fc-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="d09fc-117">Configurações de atribuição de aplicativo de loja gerenciada do Android</span><span class="sxs-lookup"><span data-stu-id="d09fc-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="d09fc-118">Armazenamento de destino de certificados</span><span class="sxs-lookup"><span data-stu-id="d09fc-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="d09fc-119">Repositório de certificados</span><span class="sxs-lookup"><span data-stu-id="d09fc-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="d09fc-120">Escala de período de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="d09fc-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="d09fc-121">Ação do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="d09fc-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="d09fc-122">Ação bloqueada do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="d09fc-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="d09fc-123">Status de conformidade</span><span class="sxs-lookup"><span data-stu-id="d09fc-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="d09fc-124">Destino da atribuição da coleção configuration manager</span><span class="sxs-lookup"><span data-stu-id="d09fc-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="d09fc-125">Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="d09fc-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="d09fc-126">Fonte de atribuição de gerenciamento de dispositivos e aplicativos</span><span class="sxs-lookup"><span data-stu-id="d09fc-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="d09fc-127">Destino de atribuição de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d09fc-128">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="d09fc-129">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="d09fc-130">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="d09fc-131">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="d09fc-132">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="d09fc-133">Tipo de registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="d09fc-134">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="d09fc-135">Configurações de credenciais derivadas do gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d09fc-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="d09fc-136">Script de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d09fc-136">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="d09fc-137">Habilitação</span><span class="sxs-lookup"><span data-stu-id="d09fc-137">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="d09fc-138">Opções de disponibilidade de registro</span><span class="sxs-lookup"><span data-stu-id="d09fc-138">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="d09fc-139">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="d09fc-139">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="d09fc-140">Destino de atribuição de grupos de exclusão</span><span class="sxs-lookup"><span data-stu-id="d09fc-140">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d09fc-141">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="d09fc-141">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="d09fc-142">Destino de atribuição de grupo</span><span class="sxs-lookup"><span data-stu-id="d09fc-142">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="d09fc-143">Algoritmos hash</span><span class="sxs-lookup"><span data-stu-id="d09fc-143">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="d09fc-144">Intenção de instalação</span><span class="sxs-lookup"><span data-stu-id="d09fc-144">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="d09fc-145">Configurações de atribuição do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-145">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="d09fc-146">Configuração de provisionamento do aplicativo LOB do iOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-146">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="d09fc-147">Proteção de aplicativo gerenciado iOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-147">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="d09fc-148">Configurações de atribuição de aplicativo da loja iOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-148">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="d09fc-149">Configurações de atribuição do aplicativo VPP do iOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-149">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="d09fc-150">Intervalo de IP</span><span class="sxs-lookup"><span data-stu-id="d09fc-150">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="d09fc-151">Intervalo de IPv4</span><span class="sxs-lookup"><span data-stu-id="d09fc-151">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="d09fc-152">Intervalo de IPv6</span><span class="sxs-lookup"><span data-stu-id="d09fc-152">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="d09fc-153">Tamanho da chave</span><span class="sxs-lookup"><span data-stu-id="d09fc-153">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="d09fc-154">Opção de provedor de armazenamento de chaves</span><span class="sxs-lookup"><span data-stu-id="d09fc-154">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="d09fc-155">Usos de chave</span><span class="sxs-lookup"><span data-stu-id="d09fc-155">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="d09fc-156">Par chave/valor</span><span class="sxs-lookup"><span data-stu-id="d09fc-156">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="d09fc-157">Configurações de atribuição do aplicativo LOB do macOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-157">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="d09fc-158">Configurações de atribuição do aplicativo VPP do macOS</span><span class="sxs-lookup"><span data-stu-id="d09fc-158">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="d09fc-159">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="d09fc-159">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="d09fc-160">Política de proteção de informações do Windows MDM</span><span class="sxs-lookup"><span data-stu-id="d09fc-160">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="d09fc-161">Configurações de atribuição do aplicativo da Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="d09fc-161">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="d09fc-162">Conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="d09fc-162">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="d09fc-163">Aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="d09fc-163">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="d09fc-164">Configurações de atribuição de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="d09fc-164">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="d09fc-165">Configurações de tempo de instalação do aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="d09fc-165">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="d09fc-166">Evento de solução de problemas de aplicativo móvel</span><span class="sxs-lookup"><span data-stu-id="d09fc-166">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="d09fc-167">Tipo de proprietário</span><span class="sxs-lookup"><span data-stu-id="d09fc-167">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="d09fc-168">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="d09fc-168">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="d09fc-169">Relatório</span><span class="sxs-lookup"><span data-stu-id="d09fc-169">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="d09fc-170">Raiz de relatório</span><span class="sxs-lookup"><span data-stu-id="d09fc-170">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="d09fc-171">Estado do aplicativo resultante</span><span class="sxs-lookup"><span data-stu-id="d09fc-171">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="d09fc-172">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="d09fc-172">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="d09fc-173">Executar como tipo de conta</span><span class="sxs-lookup"><span data-stu-id="d09fc-173">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="d09fc-174">Estado da execução</span><span class="sxs-lookup"><span data-stu-id="d09fc-174">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="d09fc-175">Opções de geração do estado da interface do usuário salvas</span><span class="sxs-lookup"><span data-stu-id="d09fc-175">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="d09fc-176">Definindo o tipo de origem</span><span class="sxs-lookup"><span data-stu-id="d09fc-176">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="d09fc-177">Tipo de nome alternativo da entidade</span><span class="sxs-lookup"><span data-stu-id="d09fc-177">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="d09fc-178">Configuração direcionada de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="d09fc-178">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="d09fc-179">URI</span><span class="sxs-lookup"><span data-stu-id="d09fc-179">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="d09fc-180">Usuário</span><span class="sxs-lookup"><span data-stu-id="d09fc-180">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="d09fc-181">Tipo de conta do token VPP</span><span class="sxs-lookup"><span data-stu-id="d09fc-181">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="d09fc-182">Causa da falha da ação do token VPP</span><span class="sxs-lookup"><span data-stu-id="d09fc-182">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="d09fc-183">Configurações de atribuição do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="d09fc-183">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="d09fc-184">Prioridade de otimização de entrega de aplicativos LOB win32</span><span class="sxs-lookup"><span data-stu-id="d09fc-184">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="d09fc-185">Notificação de aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="d09fc-185">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="d09fc-186">Configurações de reinicialização do aplicativo LOB do Win32</span><span class="sxs-lookup"><span data-stu-id="d09fc-186">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="d09fc-187">Configurações de atribuição do aplicativo Windows AppX</span><span class="sxs-lookup"><span data-stu-id="d09fc-187">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="d09fc-188">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="d09fc-188">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="d09fc-189">Configuração de ingresso no domínio do Windows</span><span class="sxs-lookup"><span data-stu-id="d09fc-189">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="d09fc-190">Configurações de atribuição do aplicativo Windows universal AppX</span><span class="sxs-lookup"><span data-stu-id="d09fc-190">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="d09fc-191">Windows estado de atualização</span><span class="sxs-lookup"><span data-stu-id="d09fc-191">Windows update state</span></span>](intune-shared-windowsupdatestate.md)