---
title: Criar macOSVpnConfiguration
description: Criar um novo objeto macOSVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5499c1359b37d8b6880a17df7c7d92a4b7eb643
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448680"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="64e52-103">Criar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64e52-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="64e52-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64e52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64e52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64e52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64e52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e52-107">Criar um novo objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64e52-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64e52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64e52-108">Prerequisites</span></span>
<span data-ttu-id="64e52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64e52-111">Permission type</span></span>|<span data-ttu-id="64e52-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64e52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e52-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64e52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64e52-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e52-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64e52-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64e52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64e52-116">Not supported.</span></span>|
|<span data-ttu-id="64e52-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64e52-117">Application</span></span>|<span data-ttu-id="64e52-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e52-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64e52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64e52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64e52-120">Request headers</span></span>
|<span data-ttu-id="64e52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64e52-121">Header</span></span>|<span data-ttu-id="64e52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64e52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64e52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64e52-123">Authorization</span></span>|<span data-ttu-id="64e52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64e52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64e52-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64e52-125">Accept</span></span>|<span data-ttu-id="64e52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64e52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64e52-127">Request body</span></span>
<span data-ttu-id="64e52-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="64e52-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="64e52-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="64e52-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="64e52-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64e52-130">Property</span></span>|<span data-ttu-id="64e52-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64e52-131">Type</span></span>|<span data-ttu-id="64e52-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e52-133">id</span><span class="sxs-lookup"><span data-stu-id="64e52-133">id</span></span>|<span data-ttu-id="64e52-134">String</span><span class="sxs-lookup"><span data-stu-id="64e52-134">String</span></span>|<span data-ttu-id="64e52-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64e52-135">Key of the entity.</span></span> <span data-ttu-id="64e52-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64e52-137">lastModifiedDateTime</span></span>|<span data-ttu-id="64e52-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e52-138">DateTimeOffset</span></span>|<span data-ttu-id="64e52-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="64e52-139">DateTime the object was last modified.</span></span> <span data-ttu-id="64e52-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64e52-141">roleScopeTagIds</span></span>|<span data-ttu-id="64e52-142">String collection</span><span class="sxs-lookup"><span data-stu-id="64e52-142">String collection</span></span>|<span data-ttu-id="64e52-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="64e52-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64e52-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64e52-145">supportsScopeTags</span></span>|<span data-ttu-id="64e52-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e52-146">Boolean</span></span>|<span data-ttu-id="64e52-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="64e52-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64e52-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="64e52-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64e52-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="64e52-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64e52-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e52-150">This property is read-only.</span></span> <span data-ttu-id="64e52-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64e52-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64e52-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64e52-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64e52-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="64e52-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64e52-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64e52-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64e52-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64e52-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64e52-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="64e52-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64e52-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64e52-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64e52-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64e52-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64e52-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="64e52-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64e52-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64e52-164">createdDateTime</span></span>|<span data-ttu-id="64e52-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e52-165">DateTimeOffset</span></span>|<span data-ttu-id="64e52-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="64e52-166">DateTime the object was created.</span></span> <span data-ttu-id="64e52-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-168">description</span><span class="sxs-lookup"><span data-stu-id="64e52-168">description</span></span>|<span data-ttu-id="64e52-169">String</span><span class="sxs-lookup"><span data-stu-id="64e52-169">String</span></span>|<span data-ttu-id="64e52-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e52-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64e52-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-172">displayName</span><span class="sxs-lookup"><span data-stu-id="64e52-172">displayName</span></span>|<span data-ttu-id="64e52-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e52-173">String</span></span>|<span data-ttu-id="64e52-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e52-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64e52-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-176">versão</span><span class="sxs-lookup"><span data-stu-id="64e52-176">version</span></span>|<span data-ttu-id="64e52-177">Int32</span><span class="sxs-lookup"><span data-stu-id="64e52-177">Int32</span></span>|<span data-ttu-id="64e52-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64e52-178">Version of the device configuration.</span></span> <span data-ttu-id="64e52-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="64e52-180">connectionName</span></span>|<span data-ttu-id="64e52-181">String</span><span class="sxs-lookup"><span data-stu-id="64e52-181">String</span></span>|<span data-ttu-id="64e52-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="64e52-182">Connection name displayed to the user.</span></span> <span data-ttu-id="64e52-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-184">Connection</span><span class="sxs-lookup"><span data-stu-id="64e52-184">connectionType</span></span>|[<span data-ttu-id="64e52-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="64e52-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="64e52-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="64e52-186">Connection type.</span></span> <span data-ttu-id="64e52-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64e52-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="64e52-188">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="64e52-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="64e52-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="64e52-189">loginGroupOrDomain</span></span>|<span data-ttu-id="64e52-190">String</span><span class="sxs-lookup"><span data-stu-id="64e52-190">String</span></span>|<span data-ttu-id="64e52-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="64e52-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="64e52-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-193">role</span><span class="sxs-lookup"><span data-stu-id="64e52-193">role</span></span>|<span data-ttu-id="64e52-194">String</span><span class="sxs-lookup"><span data-stu-id="64e52-194">String</span></span>|<span data-ttu-id="64e52-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="64e52-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="64e52-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-197">esfera</span><span class="sxs-lookup"><span data-stu-id="64e52-197">realm</span></span>|<span data-ttu-id="64e52-198">String</span><span class="sxs-lookup"><span data-stu-id="64e52-198">String</span></span>|<span data-ttu-id="64e52-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="64e52-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="64e52-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-201">do</span><span class="sxs-lookup"><span data-stu-id="64e52-201">server</span></span>|[<span data-ttu-id="64e52-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="64e52-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="64e52-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="64e52-203">VPN Server on the network.</span></span> <span data-ttu-id="64e52-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="64e52-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="64e52-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-206">identificador</span><span class="sxs-lookup"><span data-stu-id="64e52-206">identifier</span></span>|<span data-ttu-id="64e52-207">String</span><span class="sxs-lookup"><span data-stu-id="64e52-207">String</span></span>|<span data-ttu-id="64e52-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="64e52-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64e52-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-210">customData</span><span class="sxs-lookup"><span data-stu-id="64e52-210">customData</span></span>|<span data-ttu-id="64e52-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="64e52-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="64e52-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64e52-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="64e52-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="64e52-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="64e52-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="64e52-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="64e52-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="64e52-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="64e52-217">customKeyValueData</span></span>|<span data-ttu-id="64e52-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="64e52-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="64e52-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64e52-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="64e52-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="64e52-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="64e52-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="64e52-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="64e52-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="64e52-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="64e52-224">enableSplitTunneling</span></span>|<span data-ttu-id="64e52-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e52-225">Boolean</span></span>|<span data-ttu-id="64e52-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="64e52-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="64e52-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64e52-228">authenticationMethod</span></span>|[<span data-ttu-id="64e52-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64e52-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="64e52-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="64e52-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="64e52-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64e52-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="64e52-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="64e52-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="64e52-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="64e52-233">enablePerApp</span></span>|<span data-ttu-id="64e52-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e52-234">Boolean</span></span>|<span data-ttu-id="64e52-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="64e52-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="64e52-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="64e52-237">safariDomains</span></span>|<span data-ttu-id="64e52-238">String collection</span><span class="sxs-lookup"><span data-stu-id="64e52-238">String collection</span></span>|<span data-ttu-id="64e52-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="64e52-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="64e52-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="64e52-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="64e52-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="64e52-242">onDemandRules</span></span>|<span data-ttu-id="64e52-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="64e52-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="64e52-244">On-Demand Rules.</span></span> <span data-ttu-id="64e52-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="64e52-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="64e52-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="64e52-247">proxyServer</span></span>|[<span data-ttu-id="64e52-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="64e52-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="64e52-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="64e52-249">Proxy Server.</span></span> <span data-ttu-id="64e52-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64e52-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="64e52-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="64e52-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e52-252">Boolean</span></span>|<span data-ttu-id="64e52-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="64e52-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="64e52-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64e52-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="64e52-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e52-255">Response</span></span>
<span data-ttu-id="64e52-256">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64e52-256">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e52-257">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64e52-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="64e52-258">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64e52-258">Request</span></span>
<span data-ttu-id="64e52-259">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64e52-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64e52-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e52-260">Response</span></span>
<span data-ttu-id="64e52-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64e52-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





