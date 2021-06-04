---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3640c74a727c3137399cb53f41ddd7bdd7231c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753829"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="0c89c-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c89c-103">Create windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="0c89c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c89c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c89c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c89c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c89c-106">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c89c-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c89c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c89c-107">Prerequisites</span></span>
<span data-ttu-id="0c89c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c89c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c89c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c89c-110">Permission type</span></span>|<span data-ttu-id="0c89c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c89c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c89c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c89c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c89c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c89c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c89c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c89c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c89c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c89c-115">Not supported.</span></span>|
|<span data-ttu-id="0c89c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c89c-116">Application</span></span>|<span data-ttu-id="0c89c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c89c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c89c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c89c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c89c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c89c-119">Request headers</span></span>
|<span data-ttu-id="0c89c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c89c-120">Header</span></span>|<span data-ttu-id="0c89c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c89c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c89c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c89c-122">Authorization</span></span>|<span data-ttu-id="0c89c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c89c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c89c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c89c-124">Accept</span></span>|<span data-ttu-id="0c89c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c89c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c89c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c89c-126">Request body</span></span>
<span data-ttu-id="0c89c-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0c89c-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="0c89c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0c89c-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="0c89c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c89c-129">Property</span></span>|<span data-ttu-id="0c89c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c89c-130">Type</span></span>|<span data-ttu-id="0c89c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c89c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c89c-132">id</span><span class="sxs-lookup"><span data-stu-id="0c89c-132">id</span></span>|<span data-ttu-id="0c89c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c89c-133">String</span></span>|<span data-ttu-id="0c89c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c89c-134">Key of the entity.</span></span> <span data-ttu-id="0c89c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c89c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0c89c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c89c-137">DateTimeOffset</span></span>|<span data-ttu-id="0c89c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0c89c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0c89c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c89c-140">createdDateTime</span></span>|<span data-ttu-id="0c89c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c89c-141">DateTimeOffset</span></span>|<span data-ttu-id="0c89c-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c89c-142">DateTime the object was created.</span></span> <span data-ttu-id="0c89c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-144">descrição</span><span class="sxs-lookup"><span data-stu-id="0c89c-144">description</span></span>|<span data-ttu-id="0c89c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c89c-145">String</span></span>|<span data-ttu-id="0c89c-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c89c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c89c-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0c89c-148">displayName</span></span>|<span data-ttu-id="0c89c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c89c-149">String</span></span>|<span data-ttu-id="0c89c-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c89c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c89c-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-152">versão</span><span class="sxs-lookup"><span data-stu-id="0c89c-152">version</span></span>|<span data-ttu-id="0c89c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0c89c-153">Int32</span></span>|<span data-ttu-id="0c89c-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c89c-154">Version of the device configuration.</span></span> <span data-ttu-id="0c89c-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c89c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c89c-156">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="0c89c-156">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="0c89c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-157">Boolean</span></span>|<span data-ttu-id="0c89c-158">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c89c-158">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="0c89c-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="0c89c-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="0c89c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0c89c-160">Int32</span></span>|<span data-ttu-id="0c89c-161">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="0c89c-161">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="0c89c-162">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="0c89c-162">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="0c89c-163">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="0c89c-163">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="0c89c-164">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="0c89c-164">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="0c89c-165">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="0c89c-165">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="0c89c-166">Selecione a codificação de tecla pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="0c89c-166">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="0c89c-167">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-167">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="0c89c-168">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="0c89c-168">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="0c89c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-169">Boolean</span></span>|<span data-ttu-id="0c89c-170">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="0c89c-170">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="0c89c-171">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="0c89c-171">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="0c89c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-172">Boolean</span></span>|<span data-ttu-id="0c89c-173">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="0c89c-173">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="0c89c-174">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="0c89c-174">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="0c89c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-175">Boolean</span></span>|<span data-ttu-id="0c89c-176">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="0c89c-176">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="0c89c-177">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="0c89c-177">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="0c89c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-178">Boolean</span></span>|<span data-ttu-id="0c89c-179">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="0c89c-179">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="0c89c-180">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="0c89c-180">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="0c89c-181">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="0c89c-181">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="0c89c-182">Especifique como a lista de revogações de certificados deve ser imposta.</span><span class="sxs-lookup"><span data-stu-id="0c89c-182">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="0c89c-183">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-183">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="0c89c-184">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="0c89c-184">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="0c89c-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-185">Boolean</span></span>|<span data-ttu-id="0c89c-186">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="0c89c-186">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="0c89c-187">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="0c89c-187">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="0c89c-188">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="0c89c-188">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="0c89c-189">Configura como a fila de pacotes deve ser aplicada no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="0c89c-189">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="0c89c-190">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-190">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="0c89c-191">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="0c89c-191">firewallProfileDomain</span></span>|[<span data-ttu-id="0c89c-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0c89c-192">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0c89c-193">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="0c89c-193">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="0c89c-194">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="0c89c-194">firewallProfilePublic</span></span>|[<span data-ttu-id="0c89c-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0c89c-195">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0c89c-196">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="0c89c-196">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="0c89c-197">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="0c89c-197">firewallProfilePrivate</span></span>|[<span data-ttu-id="0c89c-198">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0c89c-198">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0c89c-199">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="0c89c-199">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="0c89c-200">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="0c89c-200">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="0c89c-201">String collection</span><span class="sxs-lookup"><span data-stu-id="0c89c-201">String collection</span></span>|<span data-ttu-id="0c89c-202">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="0c89c-202">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="0c89c-203">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="0c89c-203">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="0c89c-204">String collection</span><span class="sxs-lookup"><span data-stu-id="0c89c-204">String collection</span></span>|<span data-ttu-id="0c89c-205">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="0c89c-205">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="0c89c-206">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="0c89c-206">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="0c89c-207">String collection</span><span class="sxs-lookup"><span data-stu-id="0c89c-207">String collection</span></span>|<span data-ttu-id="0c89c-208">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="0c89c-208">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="0c89c-209">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="0c89c-209">defenderExploitProtectionXml</span></span>|<span data-ttu-id="0c89c-210">Binária</span><span class="sxs-lookup"><span data-stu-id="0c89c-210">Binary</span></span>|<span data-ttu-id="0c89c-211">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="0c89c-211">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="0c89c-212">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="0c89c-212">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="0c89c-213">String</span><span class="sxs-lookup"><span data-stu-id="0c89c-213">String</span></span>|<span data-ttu-id="0c89c-214">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="0c89c-214">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="0c89c-215">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="0c89c-215">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="0c89c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-216">Boolean</span></span>|<span data-ttu-id="0c89c-217">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="0c89c-217">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="0c89c-218">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="0c89c-218">appLockerApplicationControl</span></span>|[<span data-ttu-id="0c89c-219">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="0c89c-219">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="0c89c-220">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0c89c-220">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="0c89c-221">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-221">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="0c89c-222">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="0c89c-222">smartScreenEnableInShell</span></span>|<span data-ttu-id="0c89c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-223">Boolean</span></span>|<span data-ttu-id="0c89c-224">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="0c89c-224">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="0c89c-225">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="0c89c-225">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="0c89c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-226">Boolean</span></span>|<span data-ttu-id="0c89c-227">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="0c89c-227">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="0c89c-228">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="0c89c-228">applicationGuardEnabled</span></span>|<span data-ttu-id="0c89c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-229">Boolean</span></span>|<span data-ttu-id="0c89c-230">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="0c89c-230">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="0c89c-231">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="0c89c-231">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="0c89c-232">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="0c89c-232">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="0c89c-233">Bloqueie a área de transferência de arquivo de imagem, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="0c89c-233">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="0c89c-234">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-234">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="0c89c-235">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="0c89c-235">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="0c89c-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-236">Boolean</span></span>|<span data-ttu-id="0c89c-237">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="0c89c-237">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="0c89c-238">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="0c89c-238">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="0c89c-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-239">Boolean</span></span>|<span data-ttu-id="0c89c-240">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="0c89c-240">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="0c89c-241">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="0c89c-241">applicationGuardForceAuditing</span></span>|<span data-ttu-id="0c89c-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-242">Boolean</span></span>|<span data-ttu-id="0c89c-243">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="0c89c-243">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="0c89c-244">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="0c89c-244">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="0c89c-245">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="0c89c-245">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="0c89c-246">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="0c89c-246">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="0c89c-247">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="0c89c-247">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="0c89c-248">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="0c89c-248">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="0c89c-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-249">Boolean</span></span>|<span data-ttu-id="0c89c-250">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="0c89c-250">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="0c89c-251">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="0c89c-251">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="0c89c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-252">Boolean</span></span>|<span data-ttu-id="0c89c-253">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="0c89c-253">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="0c89c-254">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="0c89c-254">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="0c89c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-255">Boolean</span></span>|<span data-ttu-id="0c89c-256">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="0c89c-256">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="0c89c-257">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="0c89c-257">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="0c89c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-258">Boolean</span></span>|<span data-ttu-id="0c89c-259">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="0c89c-259">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="0c89c-260">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="0c89c-260">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="0c89c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-261">Boolean</span></span>|<span data-ttu-id="0c89c-262">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="0c89c-262">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="0c89c-263">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="0c89c-263">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="0c89c-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-264">Boolean</span></span>|<span data-ttu-id="0c89c-265">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="0c89c-265">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="0c89c-266">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="0c89c-266">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="0c89c-267">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="0c89c-267">bitLockerEncryptDevice</span></span>|<span data-ttu-id="0c89c-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c89c-268">Boolean</span></span>|<span data-ttu-id="0c89c-269">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="0c89c-269">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="0c89c-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0c89c-270">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="0c89c-271">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0c89c-271">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="0c89c-272">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="0c89c-272">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0c89c-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c89c-273">Response</span></span>
<span data-ttu-id="0c89c-274">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c89c-274">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c89c-275">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c89c-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c89c-276">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c89c-276">Request</span></span>
<span data-ttu-id="0c89c-277">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c89c-277">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c89c-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c89c-278">Response</span></span>
<span data-ttu-id="0c89c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c89c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




