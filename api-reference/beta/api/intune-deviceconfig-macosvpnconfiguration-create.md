---
title: Criar macOSVpnConfiguration
description: Criar um novo objeto macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16996ac54c4fd329d058196a5edeb612d1314c0a
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123026"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="5687b-103">Criar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5687b-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="5687b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5687b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5687b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5687b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5687b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5687b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5687b-107">Criar um novo objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5687b-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5687b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5687b-108">Prerequisites</span></span>
<span data-ttu-id="5687b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5687b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5687b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5687b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5687b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5687b-111">Permission type</span></span>|<span data-ttu-id="5687b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5687b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5687b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5687b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5687b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5687b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5687b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5687b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5687b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5687b-116">Not supported.</span></span>|
|<span data-ttu-id="5687b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5687b-117">Application</span></span>|<span data-ttu-id="5687b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5687b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5687b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5687b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5687b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5687b-120">Request headers</span></span>
|<span data-ttu-id="5687b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5687b-121">Header</span></span>|<span data-ttu-id="5687b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5687b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5687b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5687b-123">Authorization</span></span>|<span data-ttu-id="5687b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5687b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5687b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5687b-125">Accept</span></span>|<span data-ttu-id="5687b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5687b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5687b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5687b-127">Request body</span></span>
<span data-ttu-id="5687b-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5687b-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="5687b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5687b-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="5687b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5687b-130">Property</span></span>|<span data-ttu-id="5687b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5687b-131">Type</span></span>|<span data-ttu-id="5687b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5687b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5687b-133">id</span><span class="sxs-lookup"><span data-stu-id="5687b-133">id</span></span>|<span data-ttu-id="5687b-134">String</span><span class="sxs-lookup"><span data-stu-id="5687b-134">String</span></span>|<span data-ttu-id="5687b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5687b-135">Key of the entity.</span></span> <span data-ttu-id="5687b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5687b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5687b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5687b-138">DateTimeOffset</span></span>|<span data-ttu-id="5687b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5687b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5687b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5687b-141">roleScopeTagIds</span></span>|<span data-ttu-id="5687b-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-142">String collection</span></span>|<span data-ttu-id="5687b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5687b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5687b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5687b-145">supportsScopeTags</span></span>|<span data-ttu-id="5687b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="5687b-146">Boolean</span></span>|<span data-ttu-id="5687b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5687b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5687b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5687b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5687b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5687b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5687b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5687b-150">This property is read-only.</span></span> <span data-ttu-id="5687b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5687b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5687b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5687b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5687b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5687b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5687b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5687b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5687b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5687b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5687b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5687b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5687b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5687b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5687b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5687b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5687b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5687b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5687b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5687b-164">createdDateTime</span></span>|<span data-ttu-id="5687b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5687b-165">DateTimeOffset</span></span>|<span data-ttu-id="5687b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5687b-166">DateTime the object was created.</span></span> <span data-ttu-id="5687b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-168">descrição</span><span class="sxs-lookup"><span data-stu-id="5687b-168">description</span></span>|<span data-ttu-id="5687b-169">String</span><span class="sxs-lookup"><span data-stu-id="5687b-169">String</span></span>|<span data-ttu-id="5687b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5687b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5687b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5687b-172">displayName</span></span>|<span data-ttu-id="5687b-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-173">String</span></span>|<span data-ttu-id="5687b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5687b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5687b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-176">versão</span><span class="sxs-lookup"><span data-stu-id="5687b-176">version</span></span>|<span data-ttu-id="5687b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5687b-177">Int32</span></span>|<span data-ttu-id="5687b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5687b-178">Version of the device configuration.</span></span> <span data-ttu-id="5687b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="5687b-180">connectionName</span></span>|<span data-ttu-id="5687b-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-181">String</span></span>|<span data-ttu-id="5687b-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5687b-182">Connection name displayed to the user.</span></span> <span data-ttu-id="5687b-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-184">Connection</span><span class="sxs-lookup"><span data-stu-id="5687b-184">connectionType</span></span>|[<span data-ttu-id="5687b-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="5687b-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="5687b-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="5687b-186">Connection type.</span></span> <span data-ttu-id="5687b-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5687b-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="5687b-188">Os valores possíveis são:, `ciscoAnyConnect` `pulseSecure` , `f5EdgeClient` , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` , `customVpn` ,,,,,,,,,,,,,,, `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="5687b-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="5687b-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="5687b-189">loginGroupOrDomain</span></span>|<span data-ttu-id="5687b-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-190">String</span></span>|<span data-ttu-id="5687b-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="5687b-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="5687b-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-193">role</span><span class="sxs-lookup"><span data-stu-id="5687b-193">role</span></span>|<span data-ttu-id="5687b-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-194">String</span></span>|<span data-ttu-id="5687b-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="5687b-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="5687b-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-197">esfera</span><span class="sxs-lookup"><span data-stu-id="5687b-197">realm</span></span>|<span data-ttu-id="5687b-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-198">String</span></span>|<span data-ttu-id="5687b-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="5687b-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="5687b-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-201">do</span><span class="sxs-lookup"><span data-stu-id="5687b-201">server</span></span>|[<span data-ttu-id="5687b-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="5687b-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="5687b-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="5687b-203">VPN Server on the network.</span></span> <span data-ttu-id="5687b-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="5687b-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="5687b-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-206">identificador</span><span class="sxs-lookup"><span data-stu-id="5687b-206">identifier</span></span>|<span data-ttu-id="5687b-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-207">String</span></span>|<span data-ttu-id="5687b-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="5687b-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5687b-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-210">customData</span><span class="sxs-lookup"><span data-stu-id="5687b-210">customData</span></span>|<span data-ttu-id="5687b-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="5687b-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="5687b-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5687b-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="5687b-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5687b-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="5687b-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5687b-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="5687b-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="5687b-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="5687b-217">customKeyValueData</span></span>|<span data-ttu-id="5687b-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5687b-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="5687b-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5687b-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="5687b-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5687b-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="5687b-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5687b-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="5687b-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="5687b-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="5687b-224">enableSplitTunneling</span></span>|<span data-ttu-id="5687b-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="5687b-225">Boolean</span></span>|<span data-ttu-id="5687b-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="5687b-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="5687b-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5687b-228">authenticationMethod</span></span>|[<span data-ttu-id="5687b-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5687b-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="5687b-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="5687b-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="5687b-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5687b-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="5687b-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="5687b-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="5687b-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="5687b-233">enablePerApp</span></span>|<span data-ttu-id="5687b-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="5687b-234">Boolean</span></span>|<span data-ttu-id="5687b-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="5687b-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="5687b-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="5687b-237">safariDomains</span></span>|<span data-ttu-id="5687b-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5687b-238">String collection</span></span>|<span data-ttu-id="5687b-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="5687b-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="5687b-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="5687b-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="5687b-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="5687b-242">onDemandRules</span></span>|<span data-ttu-id="5687b-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="5687b-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="5687b-244">On-Demand Rules.</span></span> <span data-ttu-id="5687b-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5687b-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5687b-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="5687b-247">proxyServer</span></span>|[<span data-ttu-id="5687b-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="5687b-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="5687b-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="5687b-249">Proxy Server.</span></span> <span data-ttu-id="5687b-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5687b-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="5687b-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="5687b-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="5687b-252">Boolean</span></span>|<span data-ttu-id="5687b-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="5687b-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="5687b-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5687b-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5687b-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="5687b-255">Response</span></span>
<span data-ttu-id="5687b-256">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5687b-256">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5687b-257">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5687b-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="5687b-258">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5687b-258">Request</span></span>
<span data-ttu-id="5687b-259">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5687b-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2630

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="5687b-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="5687b-260">Response</span></span>
<span data-ttu-id="5687b-261">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5687b-261">Here is an example of the response.</span></span> <span data-ttu-id="5687b-262">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5687b-262">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5687b-263">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5687b-263">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2802

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```



