---
title: Atualizar iosVpnConfiguration
description: Atualizar as propriedades de um objeto iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88b7cc4f9a719afbc293b714c3319dfda750829d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154604"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="08966-103">Atualizar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08966-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="08966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08966-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08966-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08966-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08966-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08966-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08966-107">Atualizar as propriedades de um [objeto iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08966-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08966-108">Prerequisites</span></span>
<span data-ttu-id="08966-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08966-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08966-111">Permission type</span></span>|<span data-ttu-id="08966-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08966-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08966-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08966-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08966-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08966-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08966-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08966-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08966-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08966-116">Not supported.</span></span>|
|<span data-ttu-id="08966-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08966-117">Application</span></span>|<span data-ttu-id="08966-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08966-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08966-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08966-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="08966-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08966-120">Request headers</span></span>
|<span data-ttu-id="08966-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08966-121">Header</span></span>|<span data-ttu-id="08966-122">Valor</span><span class="sxs-lookup"><span data-stu-id="08966-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08966-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08966-123">Authorization</span></span>|<span data-ttu-id="08966-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08966-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08966-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08966-125">Accept</span></span>|<span data-ttu-id="08966-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08966-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08966-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08966-127">Request body</span></span>
<span data-ttu-id="08966-128">No corpo da solicitação, fornece uma representação JSON do [objeto iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="08966-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08966-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="08966-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08966-130">Property</span></span>|<span data-ttu-id="08966-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="08966-131">Type</span></span>|<span data-ttu-id="08966-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="08966-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08966-133">id</span><span class="sxs-lookup"><span data-stu-id="08966-133">id</span></span>|<span data-ttu-id="08966-134">String</span><span class="sxs-lookup"><span data-stu-id="08966-134">String</span></span>|<span data-ttu-id="08966-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="08966-135">Key of the entity.</span></span> <span data-ttu-id="08966-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08966-137">lastModifiedDateTime</span></span>|<span data-ttu-id="08966-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08966-138">DateTimeOffset</span></span>|<span data-ttu-id="08966-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="08966-139">DateTime the object was last modified.</span></span> <span data-ttu-id="08966-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08966-141">roleScopeTagIds</span></span>|<span data-ttu-id="08966-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08966-142">String collection</span></span>|<span data-ttu-id="08966-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="08966-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08966-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08966-145">supportsScopeTags</span></span>|<span data-ttu-id="08966-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-146">Boolean</span></span>|<span data-ttu-id="08966-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="08966-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08966-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="08966-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08966-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="08966-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08966-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08966-150">This property is read-only.</span></span> <span data-ttu-id="08966-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08966-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="08966-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08966-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="08966-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="08966-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="08966-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08966-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="08966-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08966-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="08966-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="08966-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="08966-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08966-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="08966-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08966-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="08966-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="08966-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="08966-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08966-164">createdDateTime</span></span>|<span data-ttu-id="08966-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08966-165">DateTimeOffset</span></span>|<span data-ttu-id="08966-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="08966-166">DateTime the object was created.</span></span> <span data-ttu-id="08966-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-168">description</span><span class="sxs-lookup"><span data-stu-id="08966-168">description</span></span>|<span data-ttu-id="08966-169">String</span><span class="sxs-lookup"><span data-stu-id="08966-169">String</span></span>|<span data-ttu-id="08966-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08966-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08966-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-172">displayName</span><span class="sxs-lookup"><span data-stu-id="08966-172">displayName</span></span>|<span data-ttu-id="08966-173">String</span><span class="sxs-lookup"><span data-stu-id="08966-173">String</span></span>|<span data-ttu-id="08966-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08966-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08966-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-176">versão</span><span class="sxs-lookup"><span data-stu-id="08966-176">version</span></span>|<span data-ttu-id="08966-177">Int32</span><span class="sxs-lookup"><span data-stu-id="08966-177">Int32</span></span>|<span data-ttu-id="08966-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08966-178">Version of the device configuration.</span></span> <span data-ttu-id="08966-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08966-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="08966-180">connectionName</span></span>|<span data-ttu-id="08966-181">String</span><span class="sxs-lookup"><span data-stu-id="08966-181">String</span></span>|<span data-ttu-id="08966-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="08966-182">Connection name displayed to the user.</span></span> <span data-ttu-id="08966-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="08966-184">connectionType</span></span>|[<span data-ttu-id="08966-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="08966-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="08966-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="08966-186">Connection type.</span></span> <span data-ttu-id="08966-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08966-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="08966-188">Os valores possíveis `ciscoAnyConnect` são: `pulseSecure` , , , , , , , , `f5EdgeClient` , , , , , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="08966-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="08966-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="08966-189">loginGroupOrDomain</span></span>|<span data-ttu-id="08966-190">String</span><span class="sxs-lookup"><span data-stu-id="08966-190">String</span></span>|<span data-ttu-id="08966-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="08966-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="08966-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-193">role</span><span class="sxs-lookup"><span data-stu-id="08966-193">role</span></span>|<span data-ttu-id="08966-194">String</span><span class="sxs-lookup"><span data-stu-id="08966-194">String</span></span>|<span data-ttu-id="08966-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="08966-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="08966-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-197">realm</span><span class="sxs-lookup"><span data-stu-id="08966-197">realm</span></span>|<span data-ttu-id="08966-198">String</span><span class="sxs-lookup"><span data-stu-id="08966-198">String</span></span>|<span data-ttu-id="08966-199">Realm quando o tipo de conexão está definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="08966-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="08966-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-201">server</span><span class="sxs-lookup"><span data-stu-id="08966-201">server</span></span>|[<span data-ttu-id="08966-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="08966-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="08966-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="08966-203">VPN Server on the network.</span></span> <span data-ttu-id="08966-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="08966-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="08966-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-206">identificador</span><span class="sxs-lookup"><span data-stu-id="08966-206">identifier</span></span>|<span data-ttu-id="08966-207">String</span><span class="sxs-lookup"><span data-stu-id="08966-207">String</span></span>|<span data-ttu-id="08966-208">Identificador fornecido pelo fornecedor de VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="08966-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="08966-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-210">customData</span><span class="sxs-lookup"><span data-stu-id="08966-210">customData</span></span>|<span data-ttu-id="08966-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="08966-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="08966-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="08966-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="08966-213">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="08966-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="08966-214">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="08966-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="08966-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="08966-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="08966-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="08966-217">customKeyValueData</span></span>|<span data-ttu-id="08966-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="08966-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="08966-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="08966-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="08966-220">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="08966-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="08966-221">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="08966-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="08966-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="08966-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="08966-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="08966-224">enableSplitTunneling</span></span>|<span data-ttu-id="08966-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-225">Boolean</span></span>|<span data-ttu-id="08966-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="08966-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="08966-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="08966-228">authenticationMethod</span></span>|[<span data-ttu-id="08966-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="08966-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="08966-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="08966-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="08966-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08966-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="08966-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="08966-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="08966-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="08966-233">enablePerApp</span></span>|<span data-ttu-id="08966-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-234">Boolean</span></span>|<span data-ttu-id="08966-235">Definir isso como verdadeiro cria Per-App de VPN que pode ser associada posteriormente a aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="08966-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="08966-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="08966-237">safariDomains</span></span>|<span data-ttu-id="08966-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08966-238">String collection</span></span>|<span data-ttu-id="08966-239">Domínios do Safari quando essa configuração vpn por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="08966-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="08966-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="08966-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="08966-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="08966-242">onDemandRules</span></span>|<span data-ttu-id="08966-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="08966-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="08966-244">Regras Sob Demanda.</span><span class="sxs-lookup"><span data-stu-id="08966-244">On-Demand Rules.</span></span> <span data-ttu-id="08966-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="08966-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="08966-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-247">providerType</span><span class="sxs-lookup"><span data-stu-id="08966-247">providerType</span></span>|[<span data-ttu-id="08966-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="08966-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="08966-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08966-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="08966-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08966-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="08966-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="08966-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="08966-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="08966-252">associatedDomains</span></span>|<span data-ttu-id="08966-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08966-253">String collection</span></span>|<span data-ttu-id="08966-254">Domínios Associados Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="08966-255">excludedDomains</span></span>|<span data-ttu-id="08966-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08966-256">String collection</span></span>|<span data-ttu-id="08966-257">Domínios que são acessados por meio da Internet pública em vez de via VPN, mesmo quando a VPN por aplicativo é ativada Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="08966-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="08966-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-259">Boolean</span></span>|<span data-ttu-id="08966-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="08966-261">proxyServer</span></span>|[<span data-ttu-id="08966-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="08966-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="08966-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="08966-263">Proxy Server.</span></span> <span data-ttu-id="08966-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="08966-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="08966-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-266">Boolean</span></span>|<span data-ttu-id="08966-267">Opt-In compartilhar a ID do dispositivo com clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="08966-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="08966-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08966-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="08966-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="08966-269">userDomain</span></span>|<span data-ttu-id="08966-270">String</span><span class="sxs-lookup"><span data-stu-id="08966-270">String</span></span>|<span data-ttu-id="08966-271">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-271">Zscaler only.</span></span> <span data-ttu-id="08966-272">Insira um domínio estático para pré-preencher o campo de logon no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="08966-273">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="08966-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="08966-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="08966-274">strictEnforcement</span></span>|<span data-ttu-id="08966-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="08966-275">Boolean</span></span>|<span data-ttu-id="08966-276">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-276">Zscaler only.</span></span> <span data-ttu-id="08966-277">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="08966-278">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="08966-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="08966-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="08966-279">cloudName</span></span>|<span data-ttu-id="08966-280">String</span><span class="sxs-lookup"><span data-stu-id="08966-280">String</span></span>|<span data-ttu-id="08966-281">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-281">Zscaler only.</span></span> <span data-ttu-id="08966-282">Nuvem Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="08966-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="08966-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="08966-283">excludeList</span></span>|<span data-ttu-id="08966-284">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08966-284">String collection</span></span>|<span data-ttu-id="08966-285">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-285">Zscaler only.</span></span> <span data-ttu-id="08966-286">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="08966-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="08966-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="08966-287">targetedMobileApps</span></span>|<span data-ttu-id="08966-288">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="08966-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="08966-289">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="08966-289">Targeted mobile apps.</span></span> <span data-ttu-id="08966-290">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="08966-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="08966-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="08966-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="08966-292">String</span><span class="sxs-lookup"><span data-stu-id="08966-292">String</span></span>|<span data-ttu-id="08966-293">ID do site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08966-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="08966-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="08966-294">Response</span></span>
<span data-ttu-id="08966-295">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08966-295">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08966-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08966-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="08966-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08966-297">Request</span></span>
<span data-ttu-id="08966-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08966-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3298

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="08966-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="08966-299">Response</span></span>
<span data-ttu-id="08966-p135">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08966-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3470

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




