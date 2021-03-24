---
title: Atualizar windows10VpnConfiguration
description: Atualize as propriedades de um objeto windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 271c9558083da7f3d8ba6a07c9043c983b3bfd50
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127316"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="284ff-103">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="284ff-103">Update windows10VpnConfiguration</span></span>

<span data-ttu-id="284ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="284ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="284ff-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="284ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="284ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="284ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="284ff-107">Atualize as propriedades de um [objeto windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="284ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="284ff-108">Prerequisites</span></span>
<span data-ttu-id="284ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="284ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="284ff-111">Permission type</span></span>|<span data-ttu-id="284ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="284ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="284ff-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="284ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="284ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="284ff-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="284ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="284ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="284ff-116">Not supported.</span></span>|
|<span data-ttu-id="284ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="284ff-117">Application</span></span>|<span data-ttu-id="284ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="284ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="284ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="284ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="284ff-120">Request headers</span></span>
|<span data-ttu-id="284ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="284ff-121">Header</span></span>|<span data-ttu-id="284ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="284ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="284ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="284ff-123">Authorization</span></span>|<span data-ttu-id="284ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="284ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="284ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="284ff-125">Accept</span></span>|<span data-ttu-id="284ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="284ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="284ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="284ff-127">Request body</span></span>
<span data-ttu-id="284ff-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="284ff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="284ff-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="284ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="284ff-130">Property</span></span>|<span data-ttu-id="284ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="284ff-131">Type</span></span>|<span data-ttu-id="284ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="284ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="284ff-133">id</span><span class="sxs-lookup"><span data-stu-id="284ff-133">id</span></span>|<span data-ttu-id="284ff-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-134">String</span></span>|<span data-ttu-id="284ff-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="284ff-135">Key of the entity.</span></span> <span data-ttu-id="284ff-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="284ff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="284ff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="284ff-138">DateTimeOffset</span></span>|<span data-ttu-id="284ff-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="284ff-139">DateTime the object was last modified.</span></span> <span data-ttu-id="284ff-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="284ff-141">roleScopeTagIds</span></span>|<span data-ttu-id="284ff-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-142">String collection</span></span>|<span data-ttu-id="284ff-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="284ff-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="284ff-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="284ff-145">supportsScopeTags</span></span>|<span data-ttu-id="284ff-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-146">Boolean</span></span>|<span data-ttu-id="284ff-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="284ff-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="284ff-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="284ff-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="284ff-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="284ff-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="284ff-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="284ff-150">This property is read-only.</span></span> <span data-ttu-id="284ff-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="284ff-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="284ff-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="284ff-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="284ff-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="284ff-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="284ff-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="284ff-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="284ff-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="284ff-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="284ff-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="284ff-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="284ff-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="284ff-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="284ff-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="284ff-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="284ff-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="284ff-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="284ff-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="284ff-164">createdDateTime</span></span>|<span data-ttu-id="284ff-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="284ff-165">DateTimeOffset</span></span>|<span data-ttu-id="284ff-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="284ff-166">DateTime the object was created.</span></span> <span data-ttu-id="284ff-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-168">descrição</span><span class="sxs-lookup"><span data-stu-id="284ff-168">description</span></span>|<span data-ttu-id="284ff-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-169">String</span></span>|<span data-ttu-id="284ff-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="284ff-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="284ff-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-172">displayName</span><span class="sxs-lookup"><span data-stu-id="284ff-172">displayName</span></span>|<span data-ttu-id="284ff-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-173">String</span></span>|<span data-ttu-id="284ff-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="284ff-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="284ff-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-176">versão</span><span class="sxs-lookup"><span data-stu-id="284ff-176">version</span></span>|<span data-ttu-id="284ff-177">Int32</span><span class="sxs-lookup"><span data-stu-id="284ff-177">Int32</span></span>|<span data-ttu-id="284ff-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="284ff-178">Version of the device configuration.</span></span> <span data-ttu-id="284ff-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="284ff-180">connectionName</span></span>|<span data-ttu-id="284ff-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-181">String</span></span>|<span data-ttu-id="284ff-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="284ff-182">Connection name displayed to the user.</span></span> <span data-ttu-id="284ff-183">Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-184">servers</span><span class="sxs-lookup"><span data-stu-id="284ff-184">servers</span></span>|<span data-ttu-id="284ff-185">[Coleção vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="284ff-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="284ff-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="284ff-187">Certifique-se de que os usuários finais possam acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="284ff-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="284ff-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="284ff-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="284ff-189">Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-190">customXml</span><span class="sxs-lookup"><span data-stu-id="284ff-190">customXml</span></span>|<span data-ttu-id="284ff-191">Binário</span><span class="sxs-lookup"><span data-stu-id="284ff-191">Binary</span></span>|<span data-ttu-id="284ff-192">Comandos XML personalizados que configuram a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="284ff-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="284ff-193">(Matriz de byte codificado UTF8) Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="284ff-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="284ff-194">profileTarget</span></span>|[<span data-ttu-id="284ff-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="284ff-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="284ff-196">Tipo de destino de perfil.</span><span class="sxs-lookup"><span data-stu-id="284ff-196">Profile target type.</span></span> <span data-ttu-id="284ff-197">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="284ff-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="284ff-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="284ff-198">connectionType</span></span>|[<span data-ttu-id="284ff-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="284ff-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="284ff-200">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="284ff-200">Connection type.</span></span> <span data-ttu-id="284ff-201">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span><span class="sxs-lookup"><span data-stu-id="284ff-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span></span>|
|<span data-ttu-id="284ff-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="284ff-202">enableSplitTunneling</span></span>|<span data-ttu-id="284ff-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-203">Boolean</span></span>|<span data-ttu-id="284ff-204">Habilitar o túnel dividido.</span><span class="sxs-lookup"><span data-stu-id="284ff-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="284ff-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="284ff-205">enableAlwaysOn</span></span>|<span data-ttu-id="284ff-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-206">Boolean</span></span>|<span data-ttu-id="284ff-207">Habilita o modo Always On.</span><span class="sxs-lookup"><span data-stu-id="284ff-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="284ff-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="284ff-208">enableDeviceTunnel</span></span>|<span data-ttu-id="284ff-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-209">Boolean</span></span>|<span data-ttu-id="284ff-210">Habilitar o túnel do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="284ff-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="284ff-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="284ff-211">enableDnsRegistration</span></span>|<span data-ttu-id="284ff-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-212">Boolean</span></span>|<span data-ttu-id="284ff-213">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="284ff-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="284ff-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="284ff-214">dnsSuffixes</span></span>|<span data-ttu-id="284ff-215">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-215">String collection</span></span>|<span data-ttu-id="284ff-216">Especifique sufixos DNS para adicionar à lista de pesquisa DNS para roteá-los corretamente.</span><span class="sxs-lookup"><span data-stu-id="284ff-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="284ff-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="284ff-217">authenticationMethod</span></span>|[<span data-ttu-id="284ff-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="284ff-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="284ff-219">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="284ff-219">Authentication method.</span></span> <span data-ttu-id="284ff-220">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="284ff-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="284ff-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="284ff-221">rememberUserCredentials</span></span>|<span data-ttu-id="284ff-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-222">Boolean</span></span>|<span data-ttu-id="284ff-223">Lembre-se das credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="284ff-223">Remember user credentials.</span></span>|
|<span data-ttu-id="284ff-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="284ff-224">enableConditionalAccess</span></span>|<span data-ttu-id="284ff-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-225">Boolean</span></span>|<span data-ttu-id="284ff-226">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="284ff-226">Enable conditional access.</span></span>|
|<span data-ttu-id="284ff-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="284ff-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="284ff-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-228">Boolean</span></span>|<span data-ttu-id="284ff-229">Habilitar o SSO (login único) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="284ff-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="284ff-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="284ff-230">singleSignOnEku</span></span>|[<span data-ttu-id="284ff-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="284ff-231">extendedKeyUsage</span></span>](../resources/intune-shared-extendedkeyusage.md)|<span data-ttu-id="284ff-232">EKU (Uso estendido de chave estendida) de login único.</span><span class="sxs-lookup"><span data-stu-id="284ff-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="284ff-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="284ff-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="284ff-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-234">String</span></span>|<span data-ttu-id="284ff-235">Hash do emissor de login único.</span><span class="sxs-lookup"><span data-stu-id="284ff-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="284ff-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="284ff-236">eapXml</span></span>|<span data-ttu-id="284ff-237">Binário</span><span class="sxs-lookup"><span data-stu-id="284ff-237">Binary</span></span>|<span data-ttu-id="284ff-238">XML do Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="284ff-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="284ff-239">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="284ff-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="284ff-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="284ff-240">proxyServer</span></span>|[<span data-ttu-id="284ff-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="284ff-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="284ff-242">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="284ff-242">Proxy Server.</span></span>|
|<span data-ttu-id="284ff-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="284ff-243">associatedApps</span></span>|<span data-ttu-id="284ff-244">[Coleção windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="284ff-245">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="284ff-245">Associated Apps.</span></span> <span data-ttu-id="284ff-246">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="284ff-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="284ff-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="284ff-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="284ff-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="284ff-248">Boolean</span></span>|<span data-ttu-id="284ff-249">Somente aplicativos associados podem usar conexão (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="284ff-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="284ff-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="284ff-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="284ff-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-251">String</span></span>|<span data-ttu-id="284ff-252">Domínio wip (Proteção de Informações do Windows) para associar a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="284ff-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="284ff-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="284ff-253">trafficRules</span></span>|<span data-ttu-id="284ff-254">[Coleção vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="284ff-255">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="284ff-255">Traffic rules.</span></span> <span data-ttu-id="284ff-256">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="284ff-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="284ff-257">routes</span><span class="sxs-lookup"><span data-stu-id="284ff-257">routes</span></span>|<span data-ttu-id="284ff-258">[Coleção vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="284ff-259">Rotas (opcional para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="284ff-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="284ff-260">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="284ff-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="284ff-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="284ff-261">dnsRules</span></span>|<span data-ttu-id="284ff-262">[Coleção vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="284ff-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="284ff-263">Regras DNS.</span><span class="sxs-lookup"><span data-stu-id="284ff-263">DNS rules.</span></span> <span data-ttu-id="284ff-264">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="284ff-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="284ff-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="284ff-265">trustedNetworkDomains</span></span>|<span data-ttu-id="284ff-266">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="284ff-266">String collection</span></span>|<span data-ttu-id="284ff-267">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="284ff-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="284ff-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="284ff-268">cryptographySuite</span></span>|[<span data-ttu-id="284ff-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="284ff-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="284ff-270">Configurações de segurança do Pacote de Criptografia para VPN IKEv2 no Windows10 e acima</span><span class="sxs-lookup"><span data-stu-id="284ff-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="284ff-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="284ff-271">Response</span></span>
<span data-ttu-id="284ff-272">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="284ff-272">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="284ff-273">Exemplo</span><span class="sxs-lookup"><span data-stu-id="284ff-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="284ff-274">Solicitação</span><span class="sxs-lookup"><span data-stu-id="284ff-274">Request</span></span>
<span data-ttu-id="284ff-275">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="284ff-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4463

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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="284ff-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="284ff-276">Response</span></span>
<span data-ttu-id="284ff-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="284ff-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4635

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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```




