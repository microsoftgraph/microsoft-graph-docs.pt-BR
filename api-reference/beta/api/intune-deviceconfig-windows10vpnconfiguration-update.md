---
title: Atualizar windows10VpnConfiguration
description: Atualiza as propriedades de um objeto windows10VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3bbee7faa454593d9c11a12f5908350ebbe5a036
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477557"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="79729-103">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="79729-103">Update windows10VpnConfiguration</span></span>

<span data-ttu-id="79729-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79729-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79729-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79729-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79729-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79729-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79729-107">Atualiza as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79729-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79729-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79729-108">Prerequisites</span></span>
<span data-ttu-id="79729-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79729-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79729-111">Permission type</span></span>|<span data-ttu-id="79729-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79729-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79729-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79729-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79729-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79729-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79729-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79729-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79729-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79729-116">Not supported.</span></span>|
|<span data-ttu-id="79729-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79729-117">Application</span></span>|<span data-ttu-id="79729-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79729-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79729-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79729-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="79729-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79729-120">Request headers</span></span>
|<span data-ttu-id="79729-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79729-121">Header</span></span>|<span data-ttu-id="79729-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79729-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79729-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79729-123">Authorization</span></span>|<span data-ttu-id="79729-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79729-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79729-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79729-125">Accept</span></span>|<span data-ttu-id="79729-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79729-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79729-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79729-127">Request body</span></span>
<span data-ttu-id="79729-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79729-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="79729-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79729-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="79729-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79729-130">Property</span></span>|<span data-ttu-id="79729-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79729-131">Type</span></span>|<span data-ttu-id="79729-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79729-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79729-133">id</span><span class="sxs-lookup"><span data-stu-id="79729-133">id</span></span>|<span data-ttu-id="79729-134">String</span><span class="sxs-lookup"><span data-stu-id="79729-134">String</span></span>|<span data-ttu-id="79729-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="79729-135">Key of the entity.</span></span> <span data-ttu-id="79729-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79729-137">lastModifiedDateTime</span></span>|<span data-ttu-id="79729-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79729-138">DateTimeOffset</span></span>|<span data-ttu-id="79729-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="79729-139">DateTime the object was last modified.</span></span> <span data-ttu-id="79729-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79729-141">roleScopeTagIds</span></span>|<span data-ttu-id="79729-142">String collection</span><span class="sxs-lookup"><span data-stu-id="79729-142">String collection</span></span>|<span data-ttu-id="79729-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="79729-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79729-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="79729-145">supportsScopeTags</span></span>|<span data-ttu-id="79729-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-146">Boolean</span></span>|<span data-ttu-id="79729-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="79729-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79729-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="79729-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79729-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="79729-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79729-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79729-150">This property is read-only.</span></span> <span data-ttu-id="79729-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79729-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="79729-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79729-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="79729-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="79729-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="79729-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79729-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="79729-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79729-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="79729-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="79729-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="79729-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="79729-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="79729-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="79729-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="79729-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="79729-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="79729-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79729-164">createdDateTime</span></span>|<span data-ttu-id="79729-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79729-165">DateTimeOffset</span></span>|<span data-ttu-id="79729-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="79729-166">DateTime the object was created.</span></span> <span data-ttu-id="79729-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-168">description</span><span class="sxs-lookup"><span data-stu-id="79729-168">description</span></span>|<span data-ttu-id="79729-169">String</span><span class="sxs-lookup"><span data-stu-id="79729-169">String</span></span>|<span data-ttu-id="79729-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79729-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79729-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-172">displayName</span><span class="sxs-lookup"><span data-stu-id="79729-172">displayName</span></span>|<span data-ttu-id="79729-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79729-173">String</span></span>|<span data-ttu-id="79729-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79729-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79729-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-176">versão</span><span class="sxs-lookup"><span data-stu-id="79729-176">version</span></span>|<span data-ttu-id="79729-177">Int32</span><span class="sxs-lookup"><span data-stu-id="79729-177">Int32</span></span>|<span data-ttu-id="79729-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79729-178">Version of the device configuration.</span></span> <span data-ttu-id="79729-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79729-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="79729-180">connectionName</span></span>|<span data-ttu-id="79729-181">String</span><span class="sxs-lookup"><span data-stu-id="79729-181">String</span></span>|<span data-ttu-id="79729-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="79729-182">Connection name displayed to the user.</span></span> <span data-ttu-id="79729-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="79729-184">servidores</span><span class="sxs-lookup"><span data-stu-id="79729-184">servers</span></span>|<span data-ttu-id="79729-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="79729-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="79729-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="79729-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="79729-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="79729-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="79729-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="79729-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="79729-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="79729-190">customXml</span><span class="sxs-lookup"><span data-stu-id="79729-190">customXml</span></span>|<span data-ttu-id="79729-191">Binária</span><span class="sxs-lookup"><span data-stu-id="79729-191">Binary</span></span>|<span data-ttu-id="79729-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="79729-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="79729-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79729-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="79729-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="79729-194">profileTarget</span></span>|[<span data-ttu-id="79729-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="79729-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="79729-196">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="79729-196">Profile target type.</span></span> <span data-ttu-id="79729-197">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="79729-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="79729-198">Connection</span><span class="sxs-lookup"><span data-stu-id="79729-198">connectionType</span></span>|[<span data-ttu-id="79729-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="79729-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="79729-200">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="79729-200">Connection type.</span></span> <span data-ttu-id="79729-201">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="79729-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="79729-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="79729-202">enableSplitTunneling</span></span>|<span data-ttu-id="79729-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-203">Boolean</span></span>|<span data-ttu-id="79729-204">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="79729-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="79729-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="79729-205">enableAlwaysOn</span></span>|<span data-ttu-id="79729-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-206">Boolean</span></span>|<span data-ttu-id="79729-207">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="79729-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="79729-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="79729-208">enableDeviceTunnel</span></span>|<span data-ttu-id="79729-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-209">Boolean</span></span>|<span data-ttu-id="79729-210">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79729-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="79729-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="79729-211">enableDnsRegistration</span></span>|<span data-ttu-id="79729-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-212">Boolean</span></span>|<span data-ttu-id="79729-213">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="79729-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="79729-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="79729-214">dnsSuffixes</span></span>|<span data-ttu-id="79729-215">String collection</span><span class="sxs-lookup"><span data-stu-id="79729-215">String collection</span></span>|<span data-ttu-id="79729-216">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="79729-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="79729-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="79729-217">authenticationMethod</span></span>|[<span data-ttu-id="79729-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="79729-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="79729-219">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="79729-219">Authentication method.</span></span> <span data-ttu-id="79729-220">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="79729-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="79729-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="79729-221">rememberUserCredentials</span></span>|<span data-ttu-id="79729-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-222">Boolean</span></span>|<span data-ttu-id="79729-223">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="79729-223">Remember user credentials.</span></span>|
|<span data-ttu-id="79729-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="79729-224">enableConditionalAccess</span></span>|<span data-ttu-id="79729-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-225">Boolean</span></span>|<span data-ttu-id="79729-226">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="79729-226">Enable conditional access.</span></span>|
|<span data-ttu-id="79729-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="79729-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="79729-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-228">Boolean</span></span>|<span data-ttu-id="79729-229">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="79729-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="79729-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="79729-230">singleSignOnEku</span></span>|[<span data-ttu-id="79729-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="79729-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="79729-232">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="79729-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="79729-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="79729-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="79729-234">String</span><span class="sxs-lookup"><span data-stu-id="79729-234">String</span></span>|<span data-ttu-id="79729-235">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="79729-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="79729-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="79729-236">eapXml</span></span>|<span data-ttu-id="79729-237">Binária</span><span class="sxs-lookup"><span data-stu-id="79729-237">Binary</span></span>|<span data-ttu-id="79729-238">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="79729-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="79729-239">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="79729-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="79729-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="79729-240">proxyServer</span></span>|[<span data-ttu-id="79729-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="79729-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="79729-242">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="79729-242">Proxy Server.</span></span>|
|<span data-ttu-id="79729-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="79729-243">associatedApps</span></span>|<span data-ttu-id="79729-244">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="79729-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="79729-245">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="79729-245">Associated Apps.</span></span> <span data-ttu-id="79729-246">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="79729-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="79729-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="79729-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="79729-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="79729-248">Boolean</span></span>|<span data-ttu-id="79729-249">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="79729-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="79729-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="79729-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="79729-251">String</span><span class="sxs-lookup"><span data-stu-id="79729-251">String</span></span>|<span data-ttu-id="79729-252">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="79729-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="79729-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="79729-253">trafficRules</span></span>|<span data-ttu-id="79729-254">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="79729-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="79729-255">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="79729-255">Traffic rules.</span></span> <span data-ttu-id="79729-256">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="79729-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="79729-257">roteie</span><span class="sxs-lookup"><span data-stu-id="79729-257">routes</span></span>|<span data-ttu-id="79729-258">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="79729-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="79729-259">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="79729-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="79729-260">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="79729-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="79729-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="79729-261">dnsRules</span></span>|<span data-ttu-id="79729-262">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="79729-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="79729-263">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="79729-263">DNS rules.</span></span> <span data-ttu-id="79729-264">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="79729-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="79729-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="79729-265">trustedNetworkDomains</span></span>|<span data-ttu-id="79729-266">String collection</span><span class="sxs-lookup"><span data-stu-id="79729-266">String collection</span></span>|<span data-ttu-id="79729-267">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="79729-267">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="79729-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="79729-268">Response</span></span>
<span data-ttu-id="79729-269">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79729-269">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79729-270">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79729-270">Example</span></span>

### <a name="request"></a><span data-ttu-id="79729-271">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79729-271">Request</span></span>
<span data-ttu-id="79729-272">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79729-272">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4160

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="79729-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="79729-273">Response</span></span>
<span data-ttu-id="79729-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79729-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4332

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```





