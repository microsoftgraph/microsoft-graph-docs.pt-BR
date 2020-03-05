---
title: Criar iosikEv2VpnConfiguration
description: Criar um novo objeto iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 104a115acd07324c98ef7e3c8598734663dba7c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442758"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="0113d-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0113d-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="0113d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0113d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0113d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0113d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0113d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0113d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0113d-107">Criar um novo objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0113d-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0113d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0113d-108">Prerequisites</span></span>
<span data-ttu-id="0113d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0113d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0113d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0113d-111">Permission type</span></span>|<span data-ttu-id="0113d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0113d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0113d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0113d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0113d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0113d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0113d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0113d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0113d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0113d-116">Not supported.</span></span>|
|<span data-ttu-id="0113d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0113d-117">Application</span></span>|<span data-ttu-id="0113d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0113d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0113d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0113d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0113d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0113d-120">Request headers</span></span>
|<span data-ttu-id="0113d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0113d-121">Header</span></span>|<span data-ttu-id="0113d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0113d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0113d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0113d-123">Authorization</span></span>|<span data-ttu-id="0113d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0113d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0113d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0113d-125">Accept</span></span>|<span data-ttu-id="0113d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0113d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0113d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0113d-127">Request body</span></span>
<span data-ttu-id="0113d-128">No corpo da solicitação, forneça uma representação JSON do objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0113d-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="0113d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0113d-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="0113d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0113d-130">Property</span></span>|<span data-ttu-id="0113d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0113d-131">Type</span></span>|<span data-ttu-id="0113d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0113d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0113d-133">id</span><span class="sxs-lookup"><span data-stu-id="0113d-133">id</span></span>|<span data-ttu-id="0113d-134">String</span><span class="sxs-lookup"><span data-stu-id="0113d-134">String</span></span>|<span data-ttu-id="0113d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0113d-135">Key of the entity.</span></span> <span data-ttu-id="0113d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0113d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0113d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0113d-138">DateTimeOffset</span></span>|<span data-ttu-id="0113d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0113d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0113d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0113d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0113d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0113d-142">String collection</span></span>|<span data-ttu-id="0113d-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0113d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0113d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0113d-145">supportsScopeTags</span></span>|<span data-ttu-id="0113d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-146">Boolean</span></span>|<span data-ttu-id="0113d-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0113d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0113d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0113d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0113d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0113d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0113d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0113d-150">This property is read-only.</span></span> <span data-ttu-id="0113d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0113d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0113d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0113d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0113d-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="0113d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0113d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0113d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0113d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0113d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0113d-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="0113d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0113d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0113d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0113d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0113d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0113d-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="0113d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0113d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0113d-164">createdDateTime</span></span>|<span data-ttu-id="0113d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0113d-165">DateTimeOffset</span></span>|<span data-ttu-id="0113d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0113d-166">DateTime the object was created.</span></span> <span data-ttu-id="0113d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-168">description</span><span class="sxs-lookup"><span data-stu-id="0113d-168">description</span></span>|<span data-ttu-id="0113d-169">String</span><span class="sxs-lookup"><span data-stu-id="0113d-169">String</span></span>|<span data-ttu-id="0113d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0113d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0113d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0113d-172">displayName</span></span>|<span data-ttu-id="0113d-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0113d-173">String</span></span>|<span data-ttu-id="0113d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0113d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0113d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-176">versão</span><span class="sxs-lookup"><span data-stu-id="0113d-176">version</span></span>|<span data-ttu-id="0113d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0113d-177">Int32</span></span>|<span data-ttu-id="0113d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0113d-178">Version of the device configuration.</span></span> <span data-ttu-id="0113d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="0113d-180">connectionName</span></span>|<span data-ttu-id="0113d-181">String</span><span class="sxs-lookup"><span data-stu-id="0113d-181">String</span></span>|<span data-ttu-id="0113d-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0113d-182">Connection name displayed to the user.</span></span> <span data-ttu-id="0113d-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-184">Connection</span><span class="sxs-lookup"><span data-stu-id="0113d-184">connectionType</span></span>|[<span data-ttu-id="0113d-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="0113d-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0113d-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="0113d-186">Connection type.</span></span> <span data-ttu-id="0113d-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0113d-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0113d-188">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="0113d-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="0113d-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0113d-189">loginGroupOrDomain</span></span>|<span data-ttu-id="0113d-190">String</span><span class="sxs-lookup"><span data-stu-id="0113d-190">String</span></span>|<span data-ttu-id="0113d-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="0113d-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0113d-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-193">role</span><span class="sxs-lookup"><span data-stu-id="0113d-193">role</span></span>|<span data-ttu-id="0113d-194">String</span><span class="sxs-lookup"><span data-stu-id="0113d-194">String</span></span>|<span data-ttu-id="0113d-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="0113d-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0113d-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-197">esfera</span><span class="sxs-lookup"><span data-stu-id="0113d-197">realm</span></span>|<span data-ttu-id="0113d-198">String</span><span class="sxs-lookup"><span data-stu-id="0113d-198">String</span></span>|<span data-ttu-id="0113d-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="0113d-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0113d-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-201">do</span><span class="sxs-lookup"><span data-stu-id="0113d-201">server</span></span>|[<span data-ttu-id="0113d-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0113d-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0113d-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="0113d-203">VPN Server on the network.</span></span> <span data-ttu-id="0113d-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="0113d-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="0113d-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-206">identificador</span><span class="sxs-lookup"><span data-stu-id="0113d-206">identifier</span></span>|<span data-ttu-id="0113d-207">String</span><span class="sxs-lookup"><span data-stu-id="0113d-207">String</span></span>|<span data-ttu-id="0113d-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0113d-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0113d-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-210">customData</span><span class="sxs-lookup"><span data-stu-id="0113d-210">customData</span></span>|<span data-ttu-id="0113d-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0113d-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0113d-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0113d-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0113d-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0113d-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0113d-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0113d-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0113d-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="0113d-217">customKeyValueData</span></span>|<span data-ttu-id="0113d-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0113d-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0113d-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0113d-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0113d-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0113d-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0113d-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0113d-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0113d-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0113d-224">enableSplitTunneling</span></span>|<span data-ttu-id="0113d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-225">Boolean</span></span>|<span data-ttu-id="0113d-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="0113d-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0113d-228">authenticationMethod</span></span>|[<span data-ttu-id="0113d-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0113d-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0113d-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0113d-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0113d-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0113d-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0113d-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0113d-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0113d-233">enablePerApp</span></span>|<span data-ttu-id="0113d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-234">Boolean</span></span>|<span data-ttu-id="0113d-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0113d-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0113d-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0113d-237">safariDomains</span></span>|<span data-ttu-id="0113d-238">String collection</span><span class="sxs-lookup"><span data-stu-id="0113d-238">String collection</span></span>|<span data-ttu-id="0113d-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="0113d-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0113d-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0113d-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0113d-242">onDemandRules</span></span>|<span data-ttu-id="0113d-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0113d-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="0113d-244">On-Demand Rules.</span></span> <span data-ttu-id="0113d-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0113d-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0113d-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0113d-247">proxyServer</span></span>|[<span data-ttu-id="0113d-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0113d-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0113d-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0113d-249">Proxy Server.</span></span> <span data-ttu-id="0113d-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0113d-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0113d-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-252">Boolean</span></span>|<span data-ttu-id="0113d-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="0113d-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0113d-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-255">providerType</span><span class="sxs-lookup"><span data-stu-id="0113d-255">providerType</span></span>|[<span data-ttu-id="0113d-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0113d-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0113d-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0113d-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="0113d-258">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0113d-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="0113d-259">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="0113d-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0113d-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="0113d-260">userDomain</span></span>|<span data-ttu-id="0113d-261">String</span><span class="sxs-lookup"><span data-stu-id="0113d-261">String</span></span>|<span data-ttu-id="0113d-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="0113d-262">Zscaler only.</span></span> <span data-ttu-id="0113d-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0113d-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0113d-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="0113d-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="0113d-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="0113d-266">strictEnforcement</span></span>|<span data-ttu-id="0113d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-267">Boolean</span></span>|<span data-ttu-id="0113d-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="0113d-268">Zscaler only.</span></span> <span data-ttu-id="0113d-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="0113d-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0113d-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0113d-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="0113d-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="0113d-272">cloudName</span></span>|<span data-ttu-id="0113d-273">String</span><span class="sxs-lookup"><span data-stu-id="0113d-273">String</span></span>|<span data-ttu-id="0113d-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="0113d-274">Zscaler only.</span></span> <span data-ttu-id="0113d-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="0113d-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="0113d-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="0113d-277">excludeList</span></span>|<span data-ttu-id="0113d-278">String collection</span><span class="sxs-lookup"><span data-stu-id="0113d-278">String collection</span></span>|<span data-ttu-id="0113d-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="0113d-279">Zscaler only.</span></span> <span data-ttu-id="0113d-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0113d-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="0113d-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0113d-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0113d-282">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="0113d-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0113d-284">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="0113d-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="0113d-285">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0113d-285">clientAuthenticationType</span></span>|[<span data-ttu-id="0113d-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0113d-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="0113d-287">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="0113d-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="0113d-288">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="0113d-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="0113d-289">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0113d-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="0113d-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0113d-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="0113d-291">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="0113d-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="0113d-292">.</span><span class="sxs-lookup"><span data-stu-id="0113d-292">.</span></span> <span data-ttu-id="0113d-293">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0113d-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="0113d-294">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="0113d-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="0113d-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-295">Boolean</span></span>|<span data-ttu-id="0113d-296">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="0113d-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="0113d-297">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="0113d-297">disableRedirect</span></span>|<span data-ttu-id="0113d-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-298">Boolean</span></span>|<span data-ttu-id="0113d-299">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="0113d-299">Disable Redirect</span></span>|
|<span data-ttu-id="0113d-300">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="0113d-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="0113d-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-301">Boolean</span></span>|<span data-ttu-id="0113d-302">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="0113d-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="0113d-303">enableEAP</span><span class="sxs-lookup"><span data-stu-id="0113d-303">enableEAP</span></span>|<span data-ttu-id="0113d-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-304">Boolean</span></span>|<span data-ttu-id="0113d-305">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="0113d-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="0113d-306">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="0113d-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="0113d-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-307">Boolean</span></span>|<span data-ttu-id="0113d-308">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="0113d-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="0113d-309">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="0113d-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="0113d-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-310">Boolean</span></span>|<span data-ttu-id="0113d-311">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="0113d-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="0113d-312">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="0113d-312">localIdentifier</span></span>|[<span data-ttu-id="0113d-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="0113d-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="0113d-314">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="0113d-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="0113d-315">.</span><span class="sxs-lookup"><span data-stu-id="0113d-315">.</span></span> <span data-ttu-id="0113d-316">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="0113d-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="0113d-317">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="0113d-317">remoteIdentifier</span></span>|<span data-ttu-id="0113d-318">String</span><span class="sxs-lookup"><span data-stu-id="0113d-318">String</span></span>|<span data-ttu-id="0113d-319">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="0113d-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="0113d-320">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="0113d-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="0113d-321">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-321">securityAssociationParameters</span></span>|[<span data-ttu-id="0113d-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0113d-323">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="0113d-323">Security Association Parameters</span></span>|
|<span data-ttu-id="0113d-324">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="0113d-324">serverCertificateCommonName</span></span>|<span data-ttu-id="0113d-325">String</span><span class="sxs-lookup"><span data-stu-id="0113d-325">String</span></span>|<span data-ttu-id="0113d-326">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="0113d-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="0113d-327">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="0113d-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="0113d-328">String</span><span class="sxs-lookup"><span data-stu-id="0113d-328">String</span></span>|<span data-ttu-id="0113d-329">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="0113d-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="0113d-330">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="0113d-330">serverCertificateType</span></span>|[<span data-ttu-id="0113d-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="0113d-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="0113d-332">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="0113d-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="0113d-333">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="0113d-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="0113d-334">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="0113d-334">sharedSecret</span></span>|<span data-ttu-id="0113d-335">String</span><span class="sxs-lookup"><span data-stu-id="0113d-335">String</span></span>|<span data-ttu-id="0113d-336">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="0113d-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="0113d-337">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0113d-337">tlsMaximumVersion</span></span>|<span data-ttu-id="0113d-338">String</span><span class="sxs-lookup"><span data-stu-id="0113d-338">String</span></span>|<span data-ttu-id="0113d-339">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="0113d-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0113d-340">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0113d-340">tlsMinimumVersion</span></span>|<span data-ttu-id="0113d-341">String</span><span class="sxs-lookup"><span data-stu-id="0113d-341">String</span></span>|<span data-ttu-id="0113d-342">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="0113d-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0113d-343">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="0113d-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-344">Boolean</span></span>|<span data-ttu-id="0113d-345">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="0113d-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0113d-346">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0113d-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="0113d-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-347">Boolean</span></span>|<span data-ttu-id="0113d-348">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="0113d-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0113d-349">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0113d-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="0113d-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0113d-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="0113d-351">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="0113d-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="0113d-352">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0113d-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="0113d-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="0113d-353">Boolean</span></span>|<span data-ttu-id="0113d-354">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="0113d-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="0113d-355">Resposta</span><span class="sxs-lookup"><span data-stu-id="0113d-355">Response</span></span>
<span data-ttu-id="0113d-356">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0113d-356">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0113d-357">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0113d-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="0113d-358">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0113d-358">Request</span></span>
<span data-ttu-id="0113d-359">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0113d-359">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4984

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

### <a name="response"></a><span data-ttu-id="0113d-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="0113d-360">Response</span></span>
<span data-ttu-id="0113d-p139">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0113d-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5156

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





