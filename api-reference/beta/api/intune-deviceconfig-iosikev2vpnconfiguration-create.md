---
title: Criar iosikEv2VpnConfiguration
description: Criar um novo objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4711abe1db999fc22559a05b213e4888cb784c71
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792356"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="894c5-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="894c5-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="894c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="894c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="894c5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="894c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="894c5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="894c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="894c5-107">Criar um novo objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="894c5-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="894c5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="894c5-108">Prerequisites</span></span>
<span data-ttu-id="894c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="894c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="894c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="894c5-111">Permission type</span></span>|<span data-ttu-id="894c5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="894c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="894c5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="894c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="894c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="894c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="894c5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="894c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="894c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="894c5-116">Not supported.</span></span>|
|<span data-ttu-id="894c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="894c5-117">Application</span></span>|<span data-ttu-id="894c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="894c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="894c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="894c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="894c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="894c5-120">Request headers</span></span>
|<span data-ttu-id="894c5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="894c5-121">Header</span></span>|<span data-ttu-id="894c5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="894c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="894c5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="894c5-123">Authorization</span></span>|<span data-ttu-id="894c5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="894c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="894c5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="894c5-125">Accept</span></span>|<span data-ttu-id="894c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="894c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="894c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="894c5-127">Request body</span></span>
<span data-ttu-id="894c5-128">No corpo da solicitação, forneça uma representação JSON do objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="894c5-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="894c5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="894c5-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="894c5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="894c5-130">Property</span></span>|<span data-ttu-id="894c5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="894c5-131">Type</span></span>|<span data-ttu-id="894c5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="894c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="894c5-133">id</span><span class="sxs-lookup"><span data-stu-id="894c5-133">id</span></span>|<span data-ttu-id="894c5-134">String</span><span class="sxs-lookup"><span data-stu-id="894c5-134">String</span></span>|<span data-ttu-id="894c5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="894c5-135">Key of the entity.</span></span> <span data-ttu-id="894c5-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="894c5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="894c5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894c5-138">DateTimeOffset</span></span>|<span data-ttu-id="894c5-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="894c5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="894c5-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="894c5-141">roleScopeTagIds</span></span>|<span data-ttu-id="894c5-142">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="894c5-142">String collection</span></span>|<span data-ttu-id="894c5-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="894c5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="894c5-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="894c5-145">supportsScopeTags</span></span>|<span data-ttu-id="894c5-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-146">Boolean</span></span>|<span data-ttu-id="894c5-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="894c5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="894c5-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="894c5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="894c5-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="894c5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="894c5-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="894c5-150">This property is read-only.</span></span> <span data-ttu-id="894c5-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="894c5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="894c5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="894c5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="894c5-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="894c5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="894c5-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="894c5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="894c5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="894c5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="894c5-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="894c5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="894c5-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="894c5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="894c5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="894c5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="894c5-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="894c5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="894c5-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="894c5-164">createdDateTime</span></span>|<span data-ttu-id="894c5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894c5-165">DateTimeOffset</span></span>|<span data-ttu-id="894c5-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="894c5-166">DateTime the object was created.</span></span> <span data-ttu-id="894c5-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-168">description</span><span class="sxs-lookup"><span data-stu-id="894c5-168">description</span></span>|<span data-ttu-id="894c5-169">String</span><span class="sxs-lookup"><span data-stu-id="894c5-169">String</span></span>|<span data-ttu-id="894c5-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="894c5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="894c5-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="894c5-172">displayName</span></span>|<span data-ttu-id="894c5-173">String</span><span class="sxs-lookup"><span data-stu-id="894c5-173">String</span></span>|<span data-ttu-id="894c5-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="894c5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="894c5-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-176">versão</span><span class="sxs-lookup"><span data-stu-id="894c5-176">version</span></span>|<span data-ttu-id="894c5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="894c5-177">Int32</span></span>|<span data-ttu-id="894c5-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="894c5-178">Version of the device configuration.</span></span> <span data-ttu-id="894c5-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="894c5-180">connectionName</span></span>|<span data-ttu-id="894c5-181">String</span><span class="sxs-lookup"><span data-stu-id="894c5-181">String</span></span>|<span data-ttu-id="894c5-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="894c5-182">Connection name displayed to the user.</span></span> <span data-ttu-id="894c5-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-184">Connection</span><span class="sxs-lookup"><span data-stu-id="894c5-184">connectionType</span></span>|[<span data-ttu-id="894c5-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="894c5-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="894c5-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="894c5-186">Connection type.</span></span> <span data-ttu-id="894c5-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="894c5-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="894c5-188">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` , `alwaysOn` , `microsoftTunnel` , `netMotionMobility` .</span><span class="sxs-lookup"><span data-stu-id="894c5-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="894c5-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="894c5-189">loginGroupOrDomain</span></span>|<span data-ttu-id="894c5-190">String</span><span class="sxs-lookup"><span data-stu-id="894c5-190">String</span></span>|<span data-ttu-id="894c5-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="894c5-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="894c5-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-193">role</span><span class="sxs-lookup"><span data-stu-id="894c5-193">role</span></span>|<span data-ttu-id="894c5-194">String</span><span class="sxs-lookup"><span data-stu-id="894c5-194">String</span></span>|<span data-ttu-id="894c5-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="894c5-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="894c5-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-197">esfera</span><span class="sxs-lookup"><span data-stu-id="894c5-197">realm</span></span>|<span data-ttu-id="894c5-198">String</span><span class="sxs-lookup"><span data-stu-id="894c5-198">String</span></span>|<span data-ttu-id="894c5-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="894c5-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="894c5-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-201">do</span><span class="sxs-lookup"><span data-stu-id="894c5-201">server</span></span>|[<span data-ttu-id="894c5-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="894c5-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="894c5-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="894c5-203">VPN Server on the network.</span></span> <span data-ttu-id="894c5-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="894c5-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="894c5-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-206">identificador</span><span class="sxs-lookup"><span data-stu-id="894c5-206">identifier</span></span>|<span data-ttu-id="894c5-207">String</span><span class="sxs-lookup"><span data-stu-id="894c5-207">String</span></span>|<span data-ttu-id="894c5-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="894c5-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="894c5-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-210">customData</span><span class="sxs-lookup"><span data-stu-id="894c5-210">customData</span></span>|<span data-ttu-id="894c5-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="894c5-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="894c5-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="894c5-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="894c5-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="894c5-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="894c5-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="894c5-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="894c5-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="894c5-217">customKeyValueData</span></span>|<span data-ttu-id="894c5-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="894c5-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="894c5-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="894c5-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="894c5-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="894c5-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="894c5-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="894c5-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="894c5-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="894c5-224">enableSplitTunneling</span></span>|<span data-ttu-id="894c5-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-225">Boolean</span></span>|<span data-ttu-id="894c5-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="894c5-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="894c5-228">authenticationMethod</span></span>|[<span data-ttu-id="894c5-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="894c5-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="894c5-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="894c5-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="894c5-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="894c5-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="894c5-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="894c5-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="894c5-233">enablePerApp</span></span>|<span data-ttu-id="894c5-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-234">Boolean</span></span>|<span data-ttu-id="894c5-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="894c5-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="894c5-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="894c5-237">safariDomains</span></span>|<span data-ttu-id="894c5-238">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="894c5-238">String collection</span></span>|<span data-ttu-id="894c5-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="894c5-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="894c5-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="894c5-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="894c5-242">onDemandRules</span></span>|<span data-ttu-id="894c5-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="894c5-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="894c5-244">On-Demand Rules.</span></span> <span data-ttu-id="894c5-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="894c5-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="894c5-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-247">providerType</span><span class="sxs-lookup"><span data-stu-id="894c5-247">providerType</span></span>|[<span data-ttu-id="894c5-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="894c5-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="894c5-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="894c5-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="894c5-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="894c5-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="894c5-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="894c5-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="894c5-252">proxyServer</span><span class="sxs-lookup"><span data-stu-id="894c5-252">proxyServer</span></span>|[<span data-ttu-id="894c5-253">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="894c5-253">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="894c5-254">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="894c5-254">Proxy Server.</span></span> <span data-ttu-id="894c5-255">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-255">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-256">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="894c5-256">optInToDeviceIdSharing</span></span>|<span data-ttu-id="894c5-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-257">Boolean</span></span>|<span data-ttu-id="894c5-258">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="894c5-258">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="894c5-259">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-259">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="894c5-260">userDomain</span></span>|<span data-ttu-id="894c5-261">String</span><span class="sxs-lookup"><span data-stu-id="894c5-261">String</span></span>|<span data-ttu-id="894c5-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="894c5-262">Zscaler only.</span></span> <span data-ttu-id="894c5-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="894c5-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="894c5-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="894c5-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="894c5-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="894c5-266">strictEnforcement</span></span>|<span data-ttu-id="894c5-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-267">Boolean</span></span>|<span data-ttu-id="894c5-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="894c5-268">Zscaler only.</span></span> <span data-ttu-id="894c5-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="894c5-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="894c5-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="894c5-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="894c5-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="894c5-272">cloudName</span></span>|<span data-ttu-id="894c5-273">String</span><span class="sxs-lookup"><span data-stu-id="894c5-273">String</span></span>|<span data-ttu-id="894c5-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="894c5-274">Zscaler only.</span></span> <span data-ttu-id="894c5-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="894c5-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="894c5-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="894c5-277">excludeList</span></span>|<span data-ttu-id="894c5-278">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="894c5-278">String collection</span></span>|<span data-ttu-id="894c5-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="894c5-279">Zscaler only.</span></span> <span data-ttu-id="894c5-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="894c5-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="894c5-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="894c5-282">targetedMobileApps</span></span>|<span data-ttu-id="894c5-283">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="894c5-284">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="894c5-284">Targeted mobile apps.</span></span> <span data-ttu-id="894c5-285">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="894c5-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="894c5-286">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="894c5-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="894c5-287">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="894c5-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="894c5-289">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="894c5-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="894c5-290">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="894c5-290">clientAuthenticationType</span></span>|[<span data-ttu-id="894c5-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="894c5-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="894c5-292">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="894c5-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="894c5-293">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="894c5-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="894c5-294">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="894c5-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="894c5-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="894c5-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="894c5-296">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="894c5-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="894c5-297">.</span><span class="sxs-lookup"><span data-stu-id="894c5-297">.</span></span> <span data-ttu-id="894c5-298">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="894c5-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="894c5-299">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="894c5-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="894c5-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-300">Boolean</span></span>|<span data-ttu-id="894c5-301">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="894c5-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="894c5-302">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="894c5-302">disableRedirect</span></span>|<span data-ttu-id="894c5-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-303">Boolean</span></span>|<span data-ttu-id="894c5-304">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="894c5-304">Disable Redirect</span></span>|
|<span data-ttu-id="894c5-305">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="894c5-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="894c5-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-306">Boolean</span></span>|<span data-ttu-id="894c5-307">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="894c5-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="894c5-308">enableEAP</span><span class="sxs-lookup"><span data-stu-id="894c5-308">enableEAP</span></span>|<span data-ttu-id="894c5-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-309">Boolean</span></span>|<span data-ttu-id="894c5-310">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="894c5-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="894c5-311">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="894c5-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="894c5-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-312">Boolean</span></span>|<span data-ttu-id="894c5-313">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="894c5-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="894c5-314">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="894c5-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="894c5-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-315">Boolean</span></span>|<span data-ttu-id="894c5-316">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="894c5-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="894c5-317">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="894c5-317">localIdentifier</span></span>|[<span data-ttu-id="894c5-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="894c5-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="894c5-319">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="894c5-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="894c5-320">.</span><span class="sxs-lookup"><span data-stu-id="894c5-320">.</span></span> <span data-ttu-id="894c5-321">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="894c5-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="894c5-322">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="894c5-322">remoteIdentifier</span></span>|<span data-ttu-id="894c5-323">String</span><span class="sxs-lookup"><span data-stu-id="894c5-323">String</span></span>|<span data-ttu-id="894c5-324">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="894c5-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="894c5-325">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="894c5-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="894c5-326">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-326">securityAssociationParameters</span></span>|[<span data-ttu-id="894c5-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="894c5-328">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="894c5-328">Security Association Parameters</span></span>|
|<span data-ttu-id="894c5-329">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="894c5-329">serverCertificateCommonName</span></span>|<span data-ttu-id="894c5-330">String</span><span class="sxs-lookup"><span data-stu-id="894c5-330">String</span></span>|<span data-ttu-id="894c5-331">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="894c5-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="894c5-332">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="894c5-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="894c5-333">String</span><span class="sxs-lookup"><span data-stu-id="894c5-333">String</span></span>|<span data-ttu-id="894c5-334">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="894c5-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="894c5-335">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="894c5-335">serverCertificateType</span></span>|[<span data-ttu-id="894c5-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="894c5-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="894c5-337">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="894c5-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="894c5-338">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="894c5-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="894c5-339">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="894c5-339">sharedSecret</span></span>|<span data-ttu-id="894c5-340">String</span><span class="sxs-lookup"><span data-stu-id="894c5-340">String</span></span>|<span data-ttu-id="894c5-341">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="894c5-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="894c5-342">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="894c5-342">tlsMaximumVersion</span></span>|<span data-ttu-id="894c5-343">String</span><span class="sxs-lookup"><span data-stu-id="894c5-343">String</span></span>|<span data-ttu-id="894c5-344">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="894c5-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="894c5-345">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="894c5-345">tlsMinimumVersion</span></span>|<span data-ttu-id="894c5-346">String</span><span class="sxs-lookup"><span data-stu-id="894c5-346">String</span></span>|<span data-ttu-id="894c5-347">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="894c5-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="894c5-348">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="894c5-349">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-349">Boolean</span></span>|<span data-ttu-id="894c5-350">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="894c5-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="894c5-351">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="894c5-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="894c5-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-352">Boolean</span></span>|<span data-ttu-id="894c5-353">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="894c5-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="894c5-354">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="894c5-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="894c5-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="894c5-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="894c5-356">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="894c5-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="894c5-357">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="894c5-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="894c5-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="894c5-358">Boolean</span></span>|<span data-ttu-id="894c5-359">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="894c5-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="894c5-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="894c5-360">Response</span></span>
<span data-ttu-id="894c5-361">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="894c5-361">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="894c5-362">Exemplo</span><span class="sxs-lookup"><span data-stu-id="894c5-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="894c5-363">Solicitação</span><span class="sxs-lookup"><span data-stu-id="894c5-363">Request</span></span>
<span data-ttu-id="894c5-364">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="894c5-364">Here is an example of the request.</span></span>
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
  "providerType": "appProxy",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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

### <a name="response"></a><span data-ttu-id="894c5-365">Resposta</span><span class="sxs-lookup"><span data-stu-id="894c5-365">Response</span></span>
<span data-ttu-id="894c5-p140">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="894c5-p140">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "providerType": "appProxy",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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



