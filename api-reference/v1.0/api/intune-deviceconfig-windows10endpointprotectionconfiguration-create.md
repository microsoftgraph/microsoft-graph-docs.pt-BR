---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9d3cdd29a403ff5bf7b005ce8df0a89c282d57b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558220"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="25f20-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="25f20-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="25f20-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25f20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25f20-105">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f20-105">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25f20-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25f20-106">Prerequisites</span></span>
<span data-ttu-id="25f20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25f20-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25f20-109">Permission type</span></span>|<span data-ttu-id="25f20-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25f20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25f20-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25f20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25f20-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25f20-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25f20-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25f20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25f20-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f20-114">Not supported.</span></span>|
|<span data-ttu-id="25f20-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25f20-115">Application</span></span>|<span data-ttu-id="25f20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25f20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25f20-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25f20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="25f20-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25f20-118">Request headers</span></span>
|<span data-ttu-id="25f20-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25f20-119">Header</span></span>|<span data-ttu-id="25f20-120">Valor</span><span class="sxs-lookup"><span data-stu-id="25f20-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25f20-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25f20-121">Authorization</span></span>|<span data-ttu-id="25f20-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25f20-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25f20-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25f20-123">Accept</span></span>|<span data-ttu-id="25f20-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25f20-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25f20-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25f20-125">Request body</span></span>
<span data-ttu-id="25f20-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="25f20-126">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="25f20-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="25f20-127">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="25f20-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25f20-128">Property</span></span>|<span data-ttu-id="25f20-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="25f20-129">Type</span></span>|<span data-ttu-id="25f20-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="25f20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25f20-131">id</span><span class="sxs-lookup"><span data-stu-id="25f20-131">id</span></span>|<span data-ttu-id="25f20-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f20-132">String</span></span>|<span data-ttu-id="25f20-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25f20-133">Key of the entity.</span></span> <span data-ttu-id="25f20-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25f20-135">lastModifiedDateTime</span></span>|<span data-ttu-id="25f20-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25f20-136">DateTimeOffset</span></span>|<span data-ttu-id="25f20-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="25f20-137">DateTime the object was last modified.</span></span> <span data-ttu-id="25f20-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25f20-139">createdDateTime</span></span>|<span data-ttu-id="25f20-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25f20-140">DateTimeOffset</span></span>|<span data-ttu-id="25f20-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="25f20-141">DateTime the object was created.</span></span> <span data-ttu-id="25f20-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-143">description</span><span class="sxs-lookup"><span data-stu-id="25f20-143">description</span></span>|<span data-ttu-id="25f20-144">String</span><span class="sxs-lookup"><span data-stu-id="25f20-144">String</span></span>|<span data-ttu-id="25f20-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25f20-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25f20-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-147">displayName</span><span class="sxs-lookup"><span data-stu-id="25f20-147">displayName</span></span>|<span data-ttu-id="25f20-148">String</span><span class="sxs-lookup"><span data-stu-id="25f20-148">String</span></span>|<span data-ttu-id="25f20-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25f20-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25f20-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-151">versão</span><span class="sxs-lookup"><span data-stu-id="25f20-151">version</span></span>|<span data-ttu-id="25f20-152">Int32</span><span class="sxs-lookup"><span data-stu-id="25f20-152">Int32</span></span>|<span data-ttu-id="25f20-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25f20-153">Version of the device configuration.</span></span> <span data-ttu-id="25f20-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f20-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f20-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="25f20-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="25f20-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-156">Boolean</span></span>|<span data-ttu-id="25f20-157">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="25f20-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="25f20-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="25f20-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="25f20-159">Int32</span><span class="sxs-lookup"><span data-stu-id="25f20-159">Int32</span></span>|<span data-ttu-id="25f20-160">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="25f20-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="25f20-161">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="25f20-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="25f20-162">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="25f20-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="25f20-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="25f20-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="25f20-164">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="25f20-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="25f20-165">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="25f20-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="25f20-166">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="25f20-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="25f20-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="25f20-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="25f20-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-168">Boolean</span></span>|<span data-ttu-id="25f20-169">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="25f20-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="25f20-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="25f20-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="25f20-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-171">Boolean</span></span>|<span data-ttu-id="25f20-172">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="25f20-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="25f20-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="25f20-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="25f20-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-174">Boolean</span></span>|<span data-ttu-id="25f20-175">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="25f20-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="25f20-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="25f20-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="25f20-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-177">Boolean</span></span>|<span data-ttu-id="25f20-178">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="25f20-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="25f20-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="25f20-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="25f20-180">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="25f20-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="25f20-181">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="25f20-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="25f20-182">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="25f20-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="25f20-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="25f20-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="25f20-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-184">Boolean</span></span>|<span data-ttu-id="25f20-185">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="25f20-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="25f20-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="25f20-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="25f20-187">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="25f20-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="25f20-188">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="25f20-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="25f20-189">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="25f20-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="25f20-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="25f20-190">firewallProfileDomain</span></span>|[<span data-ttu-id="25f20-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="25f20-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="25f20-192">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="25f20-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="25f20-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="25f20-193">firewallProfilePublic</span></span>|[<span data-ttu-id="25f20-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="25f20-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="25f20-195">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="25f20-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="25f20-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="25f20-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="25f20-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="25f20-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="25f20-198">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="25f20-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="25f20-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="25f20-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="25f20-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f20-200">String collection</span></span>|<span data-ttu-id="25f20-201">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="25f20-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="25f20-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="25f20-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="25f20-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25f20-203">String collection</span></span>|<span data-ttu-id="25f20-204">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="25f20-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="25f20-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="25f20-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="25f20-206">String collection</span><span class="sxs-lookup"><span data-stu-id="25f20-206">String collection</span></span>|<span data-ttu-id="25f20-207">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="25f20-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="25f20-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="25f20-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="25f20-209">Binária</span><span class="sxs-lookup"><span data-stu-id="25f20-209">Binary</span></span>|<span data-ttu-id="25f20-210">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="25f20-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="25f20-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="25f20-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="25f20-212">String</span><span class="sxs-lookup"><span data-stu-id="25f20-212">String</span></span>|<span data-ttu-id="25f20-213">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="25f20-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="25f20-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="25f20-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="25f20-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-215">Boolean</span></span>|<span data-ttu-id="25f20-216">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="25f20-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="25f20-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="25f20-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="25f20-218">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="25f20-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="25f20-219">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="25f20-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="25f20-220">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="25f20-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="25f20-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="25f20-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="25f20-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-222">Boolean</span></span>|<span data-ttu-id="25f20-223">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="25f20-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="25f20-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="25f20-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="25f20-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="25f20-225">Boolean</span></span>|<span data-ttu-id="25f20-226">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="25f20-226">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="25f20-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="25f20-227">applicationGuardEnabled</span></span>|<span data-ttu-id="25f20-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-228">Boolean</span></span>|<span data-ttu-id="25f20-229">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="25f20-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="25f20-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="25f20-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="25f20-231">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="25f20-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="25f20-232">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="25f20-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="25f20-233">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="25f20-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="25f20-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="25f20-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="25f20-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-235">Boolean</span></span>|<span data-ttu-id="25f20-236">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="25f20-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="25f20-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="25f20-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="25f20-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-238">Boolean</span></span>|<span data-ttu-id="25f20-239">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="25f20-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="25f20-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="25f20-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="25f20-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-241">Boolean</span></span>|<span data-ttu-id="25f20-242">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="25f20-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="25f20-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="25f20-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="25f20-244">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="25f20-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="25f20-245">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="25f20-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="25f20-246">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="25f20-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="25f20-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="25f20-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="25f20-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-248">Boolean</span></span>|<span data-ttu-id="25f20-249">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="25f20-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="25f20-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="25f20-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="25f20-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-251">Boolean</span></span>|<span data-ttu-id="25f20-252">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="25f20-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="25f20-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="25f20-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="25f20-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-254">Boolean</span></span>|<span data-ttu-id="25f20-255">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="25f20-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="25f20-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="25f20-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="25f20-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-257">Boolean</span></span>|<span data-ttu-id="25f20-258">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="25f20-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="25f20-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="25f20-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="25f20-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="25f20-260">Boolean</span></span>|<span data-ttu-id="25f20-261">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="25f20-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="25f20-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="25f20-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="25f20-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="25f20-263">Boolean</span></span>|<span data-ttu-id="25f20-264">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="25f20-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="25f20-265">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="25f20-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="25f20-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="25f20-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="25f20-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="25f20-267">Boolean</span></span>|<span data-ttu-id="25f20-268">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="25f20-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="25f20-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="25f20-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="25f20-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="25f20-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="25f20-271">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="25f20-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="25f20-272">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f20-272">Response</span></span>
<span data-ttu-id="25f20-273">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25f20-273">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25f20-274">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25f20-274">Example</span></span>

### <a name="request"></a><span data-ttu-id="25f20-275">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25f20-275">Request</span></span>
<span data-ttu-id="25f20-276">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25f20-276">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4245

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="25f20-277">Resposta</span><span class="sxs-lookup"><span data-stu-id="25f20-277">Response</span></span>
<span data-ttu-id="25f20-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25f20-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



