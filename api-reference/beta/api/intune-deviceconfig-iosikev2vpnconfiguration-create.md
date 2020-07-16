---
title: Criar iosikEv2VpnConfiguration
description: Criar um novo objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aff0878c6bd2a921fc5f1c40a072555a6524d383
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123124"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="3bb33-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bb33-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="3bb33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bb33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bb33-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bb33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bb33-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bb33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bb33-107">Criar um novo objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3bb33-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bb33-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bb33-108">Prerequisites</span></span>
<span data-ttu-id="3bb33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bb33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bb33-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bb33-111">Permission type</span></span>|<span data-ttu-id="3bb33-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3bb33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bb33-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bb33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bb33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bb33-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bb33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bb33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bb33-116">Not supported.</span></span>|
|<span data-ttu-id="3bb33-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bb33-117">Application</span></span>|<span data-ttu-id="3bb33-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb33-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bb33-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bb33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bb33-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb33-120">Request headers</span></span>
|<span data-ttu-id="3bb33-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bb33-121">Header</span></span>|<span data-ttu-id="3bb33-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bb33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bb33-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bb33-123">Authorization</span></span>|<span data-ttu-id="3bb33-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bb33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bb33-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bb33-125">Accept</span></span>|<span data-ttu-id="3bb33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb33-127">Request body</span></span>
<span data-ttu-id="3bb33-128">No corpo da solicitação, forneça uma representação JSON do objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3bb33-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="3bb33-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3bb33-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="3bb33-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bb33-130">Property</span></span>|<span data-ttu-id="3bb33-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bb33-131">Type</span></span>|<span data-ttu-id="3bb33-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bb33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bb33-133">id</span><span class="sxs-lookup"><span data-stu-id="3bb33-133">id</span></span>|<span data-ttu-id="3bb33-134">String</span><span class="sxs-lookup"><span data-stu-id="3bb33-134">String</span></span>|<span data-ttu-id="3bb33-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3bb33-135">Key of the entity.</span></span> <span data-ttu-id="3bb33-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bb33-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3bb33-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bb33-138">DateTimeOffset</span></span>|<span data-ttu-id="3bb33-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3bb33-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3bb33-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3bb33-141">roleScopeTagIds</span></span>|<span data-ttu-id="3bb33-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-142">String collection</span></span>|<span data-ttu-id="3bb33-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3bb33-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3bb33-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3bb33-145">supportsScopeTags</span></span>|<span data-ttu-id="3bb33-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-146">Boolean</span></span>|<span data-ttu-id="3bb33-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3bb33-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3bb33-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3bb33-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3bb33-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bb33-150">This property is read-only.</span></span> <span data-ttu-id="3bb33-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bb33-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3bb33-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bb33-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3bb33-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3bb33-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3bb33-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bb33-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3bb33-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bb33-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3bb33-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3bb33-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3bb33-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bb33-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3bb33-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bb33-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3bb33-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3bb33-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3bb33-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bb33-164">createdDateTime</span></span>|<span data-ttu-id="3bb33-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bb33-165">DateTimeOffset</span></span>|<span data-ttu-id="3bb33-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3bb33-166">DateTime the object was created.</span></span> <span data-ttu-id="3bb33-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-168">descrição</span><span class="sxs-lookup"><span data-stu-id="3bb33-168">description</span></span>|<span data-ttu-id="3bb33-169">String</span><span class="sxs-lookup"><span data-stu-id="3bb33-169">String</span></span>|<span data-ttu-id="3bb33-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bb33-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3bb33-172">displayName</span></span>|<span data-ttu-id="3bb33-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-173">String</span></span>|<span data-ttu-id="3bb33-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bb33-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-176">versão</span><span class="sxs-lookup"><span data-stu-id="3bb33-176">version</span></span>|<span data-ttu-id="3bb33-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3bb33-177">Int32</span></span>|<span data-ttu-id="3bb33-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-178">Version of the device configuration.</span></span> <span data-ttu-id="3bb33-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="3bb33-180">connectionName</span></span>|<span data-ttu-id="3bb33-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-181">String</span></span>|<span data-ttu-id="3bb33-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3bb33-182">Connection name displayed to the user.</span></span> <span data-ttu-id="3bb33-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-184">Connection</span><span class="sxs-lookup"><span data-stu-id="3bb33-184">connectionType</span></span>|[<span data-ttu-id="3bb33-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="3bb33-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="3bb33-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="3bb33-186">Connection type.</span></span> <span data-ttu-id="3bb33-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bb33-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3bb33-188">Os valores possíveis são:, `ciscoAnyConnect` `pulseSecure` , `f5EdgeClient` , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` , `customVpn` ,,,,,,,,,,,,,,, `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="3bb33-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="3bb33-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3bb33-189">loginGroupOrDomain</span></span>|<span data-ttu-id="3bb33-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-190">String</span></span>|<span data-ttu-id="3bb33-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="3bb33-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="3bb33-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-193">role</span><span class="sxs-lookup"><span data-stu-id="3bb33-193">role</span></span>|<span data-ttu-id="3bb33-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-194">String</span></span>|<span data-ttu-id="3bb33-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="3bb33-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3bb33-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-197">esfera</span><span class="sxs-lookup"><span data-stu-id="3bb33-197">realm</span></span>|<span data-ttu-id="3bb33-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-198">String</span></span>|<span data-ttu-id="3bb33-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="3bb33-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3bb33-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-201">do</span><span class="sxs-lookup"><span data-stu-id="3bb33-201">server</span></span>|[<span data-ttu-id="3bb33-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="3bb33-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="3bb33-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="3bb33-203">VPN Server on the network.</span></span> <span data-ttu-id="3bb33-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="3bb33-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="3bb33-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-206">identificador</span><span class="sxs-lookup"><span data-stu-id="3bb33-206">identifier</span></span>|<span data-ttu-id="3bb33-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-207">String</span></span>|<span data-ttu-id="3bb33-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="3bb33-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3bb33-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-210">customData</span><span class="sxs-lookup"><span data-stu-id="3bb33-210">customData</span></span>|<span data-ttu-id="3bb33-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="3bb33-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="3bb33-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3bb33-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3bb33-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="3bb33-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3bb33-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="3bb33-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3bb33-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="3bb33-217">customKeyValueData</span></span>|<span data-ttu-id="3bb33-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3bb33-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="3bb33-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3bb33-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3bb33-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="3bb33-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3bb33-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="3bb33-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3bb33-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3bb33-224">enableSplitTunneling</span></span>|<span data-ttu-id="3bb33-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-225">Boolean</span></span>|<span data-ttu-id="3bb33-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="3bb33-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3bb33-228">authenticationMethod</span></span>|[<span data-ttu-id="3bb33-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3bb33-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3bb33-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="3bb33-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bb33-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3bb33-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="3bb33-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="3bb33-233">enablePerApp</span></span>|<span data-ttu-id="3bb33-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-234">Boolean</span></span>|<span data-ttu-id="3bb33-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="3bb33-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="3bb33-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="3bb33-237">safariDomains</span></span>|<span data-ttu-id="3bb33-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-238">String collection</span></span>|<span data-ttu-id="3bb33-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="3bb33-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="3bb33-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="3bb33-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="3bb33-242">onDemandRules</span></span>|<span data-ttu-id="3bb33-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="3bb33-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="3bb33-244">On-Demand Rules.</span></span> <span data-ttu-id="3bb33-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3bb33-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3bb33-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3bb33-247">proxyServer</span></span>|[<span data-ttu-id="3bb33-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3bb33-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="3bb33-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3bb33-249">Proxy Server.</span></span> <span data-ttu-id="3bb33-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="3bb33-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="3bb33-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-252">Boolean</span></span>|<span data-ttu-id="3bb33-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="3bb33-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="3bb33-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-255">providerType</span><span class="sxs-lookup"><span data-stu-id="3bb33-255">providerType</span></span>|[<span data-ttu-id="3bb33-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="3bb33-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="3bb33-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3bb33-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="3bb33-258">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bb33-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="3bb33-259">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="3bb33-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="3bb33-260">userDomain</span></span>|<span data-ttu-id="3bb33-261">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-261">String</span></span>|<span data-ttu-id="3bb33-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="3bb33-262">Zscaler only.</span></span> <span data-ttu-id="3bb33-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="3bb33-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="3bb33-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="3bb33-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="3bb33-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="3bb33-266">strictEnforcement</span></span>|<span data-ttu-id="3bb33-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-267">Boolean</span></span>|<span data-ttu-id="3bb33-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="3bb33-268">Zscaler only.</span></span> <span data-ttu-id="3bb33-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="3bb33-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="3bb33-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3bb33-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="3bb33-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="3bb33-272">cloudName</span></span>|<span data-ttu-id="3bb33-273">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-273">String</span></span>|<span data-ttu-id="3bb33-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="3bb33-274">Zscaler only.</span></span> <span data-ttu-id="3bb33-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="3bb33-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="3bb33-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="3bb33-277">excludeList</span></span>|<span data-ttu-id="3bb33-278">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-278">String collection</span></span>|<span data-ttu-id="3bb33-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="3bb33-279">Zscaler only.</span></span> <span data-ttu-id="3bb33-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="3bb33-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="3bb33-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3bb33-282">targetedMobileApps</span></span>|<span data-ttu-id="3bb33-283">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bb33-284">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="3bb33-284">Targeted mobile apps.</span></span> <span data-ttu-id="3bb33-285">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3bb33-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3bb33-286">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bb33-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bb33-287">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="3bb33-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="3bb33-289">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="3bb33-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="3bb33-290">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="3bb33-290">clientAuthenticationType</span></span>|[<span data-ttu-id="3bb33-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="3bb33-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="3bb33-292">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="3bb33-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="3bb33-293">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="3bb33-294">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="3bb33-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="3bb33-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="3bb33-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="3bb33-296">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="3bb33-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="3bb33-297">.</span><span class="sxs-lookup"><span data-stu-id="3bb33-297">.</span></span> <span data-ttu-id="3bb33-298">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="3bb33-299">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="3bb33-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="3bb33-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-300">Boolean</span></span>|<span data-ttu-id="3bb33-301">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="3bb33-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="3bb33-302">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="3bb33-302">disableRedirect</span></span>|<span data-ttu-id="3bb33-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-303">Boolean</span></span>|<span data-ttu-id="3bb33-304">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="3bb33-304">Disable Redirect</span></span>|
|<span data-ttu-id="3bb33-305">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="3bb33-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="3bb33-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-306">Boolean</span></span>|<span data-ttu-id="3bb33-307">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="3bb33-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="3bb33-308">enableEAP</span><span class="sxs-lookup"><span data-stu-id="3bb33-308">enableEAP</span></span>|<span data-ttu-id="3bb33-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-309">Boolean</span></span>|<span data-ttu-id="3bb33-310">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="3bb33-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="3bb33-311">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="3bb33-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="3bb33-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-312">Boolean</span></span>|<span data-ttu-id="3bb33-313">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="3bb33-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="3bb33-314">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="3bb33-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="3bb33-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-315">Boolean</span></span>|<span data-ttu-id="3bb33-316">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="3bb33-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="3bb33-317">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="3bb33-317">localIdentifier</span></span>|[<span data-ttu-id="3bb33-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="3bb33-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="3bb33-319">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="3bb33-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="3bb33-320">.</span><span class="sxs-lookup"><span data-stu-id="3bb33-320">.</span></span> <span data-ttu-id="3bb33-321">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="3bb33-322">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="3bb33-322">remoteIdentifier</span></span>|<span data-ttu-id="3bb33-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-323">String</span></span>|<span data-ttu-id="3bb33-324">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="3bb33-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="3bb33-325">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="3bb33-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="3bb33-326">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-326">securityAssociationParameters</span></span>|[<span data-ttu-id="3bb33-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="3bb33-328">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="3bb33-328">Security Association Parameters</span></span>|
|<span data-ttu-id="3bb33-329">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="3bb33-329">serverCertificateCommonName</span></span>|<span data-ttu-id="3bb33-330">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-330">String</span></span>|<span data-ttu-id="3bb33-331">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="3bb33-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="3bb33-332">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="3bb33-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="3bb33-333">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-333">String</span></span>|<span data-ttu-id="3bb33-334">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="3bb33-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="3bb33-335">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="3bb33-335">serverCertificateType</span></span>|[<span data-ttu-id="3bb33-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="3bb33-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="3bb33-337">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="3bb33-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="3bb33-338">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="3bb33-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="3bb33-339">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="3bb33-339">sharedSecret</span></span>|<span data-ttu-id="3bb33-340">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-340">String</span></span>|<span data-ttu-id="3bb33-341">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="3bb33-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="3bb33-342">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3bb33-342">tlsMaximumVersion</span></span>|<span data-ttu-id="3bb33-343">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-343">String</span></span>|<span data-ttu-id="3bb33-344">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="3bb33-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="3bb33-345">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3bb33-345">tlsMinimumVersion</span></span>|<span data-ttu-id="3bb33-346">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bb33-346">String</span></span>|<span data-ttu-id="3bb33-347">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="3bb33-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="3bb33-348">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="3bb33-349">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-349">Boolean</span></span>|<span data-ttu-id="3bb33-350">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="3bb33-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="3bb33-351">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3bb33-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="3bb33-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-352">Boolean</span></span>|<span data-ttu-id="3bb33-353">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="3bb33-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="3bb33-354">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bb33-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="3bb33-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bb33-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="3bb33-356">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="3bb33-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="3bb33-357">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bb33-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="3bb33-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bb33-358">Boolean</span></span>|<span data-ttu-id="3bb33-359">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="3bb33-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="3bb33-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bb33-360">Response</span></span>
<span data-ttu-id="3bb33-361">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bb33-361">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bb33-362">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bb33-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb33-363">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb33-363">Request</span></span>
<span data-ttu-id="3bb33-364">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bb33-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5241

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="3bb33-365">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bb33-365">Response</span></span>
<span data-ttu-id="3bb33-p140">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bb33-p140">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5413

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```



