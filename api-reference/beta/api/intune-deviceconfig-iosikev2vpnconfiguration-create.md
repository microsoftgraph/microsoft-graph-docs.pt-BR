---
title: Criar iosikEv2VpnConfiguration
description: Crie um novo objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0a75d638a623527458e43795e2bf6dc2b03a491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147914"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="7e9c4-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e9c4-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="7e9c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e9c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e9c4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e9c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e9c4-107">Crie um novo [objeto iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e9c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e9c4-108">Prerequisites</span></span>
<span data-ttu-id="7e9c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e9c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e9c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e9c4-111">Permission type</span></span>|<span data-ttu-id="7e9c4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e9c4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e9c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e9c4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e9c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-116">Not supported.</span></span>|
|<span data-ttu-id="7e9c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e9c4-117">Application</span></span>|<span data-ttu-id="7e9c4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9c4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e9c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e9c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9c4-120">Request headers</span></span>
|<span data-ttu-id="7e9c4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e9c4-121">Header</span></span>|<span data-ttu-id="7e9c4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e9c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e9c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e9c4-123">Authorization</span></span>|<span data-ttu-id="7e9c4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e9c4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e9c4-125">Accept</span></span>|<span data-ttu-id="7e9c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e9c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e9c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9c4-127">Request body</span></span>
<span data-ttu-id="7e9c4-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="7e9c4-129">A tabela a seguir mostra as propriedades necessárias ao criar o iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="7e9c4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e9c4-130">Property</span></span>|<span data-ttu-id="7e9c4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e9c4-131">Type</span></span>|<span data-ttu-id="7e9c4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e9c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e9c4-133">id</span><span class="sxs-lookup"><span data-stu-id="7e9c4-133">id</span></span>|<span data-ttu-id="7e9c4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-134">String</span></span>|<span data-ttu-id="7e9c4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-135">Key of the entity.</span></span> <span data-ttu-id="7e9c4-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9c4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7e9c4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9c4-138">DateTimeOffset</span></span>|<span data-ttu-id="7e9c4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7e9c4-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e9c4-141">roleScopeTagIds</span></span>|<span data-ttu-id="7e9c4-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-142">String collection</span></span>|<span data-ttu-id="7e9c4-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e9c4-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7e9c4-145">supportsScopeTags</span></span>|<span data-ttu-id="7e9c4-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-146">Boolean</span></span>|<span data-ttu-id="7e9c4-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7e9c4-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7e9c4-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7e9c4-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-150">This property is read-only.</span></span> <span data-ttu-id="7e9c4-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e9c4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7e9c4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e9c4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7e9c4-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7e9c4-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e9c4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7e9c4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e9c4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7e9c4-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7e9c4-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7e9c4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7e9c4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7e9c4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7e9c4-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7e9c4-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9c4-164">createdDateTime</span></span>|<span data-ttu-id="7e9c4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9c4-165">DateTimeOffset</span></span>|<span data-ttu-id="7e9c4-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-166">DateTime the object was created.</span></span> <span data-ttu-id="7e9c4-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-168">descrição</span><span class="sxs-lookup"><span data-stu-id="7e9c4-168">description</span></span>|<span data-ttu-id="7e9c4-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-169">String</span></span>|<span data-ttu-id="7e9c4-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e9c4-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7e9c4-172">displayName</span></span>|<span data-ttu-id="7e9c4-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-173">String</span></span>|<span data-ttu-id="7e9c4-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e9c4-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-176">versão</span><span class="sxs-lookup"><span data-stu-id="7e9c4-176">version</span></span>|<span data-ttu-id="7e9c4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7e9c4-177">Int32</span></span>|<span data-ttu-id="7e9c4-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-178">Version of the device configuration.</span></span> <span data-ttu-id="7e9c4-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="7e9c4-180">connectionName</span></span>|<span data-ttu-id="7e9c4-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-181">String</span></span>|<span data-ttu-id="7e9c4-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-182">Connection name displayed to the user.</span></span> <span data-ttu-id="7e9c4-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-184">connectionType</span></span>|[<span data-ttu-id="7e9c4-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="7e9c4-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-186">Connection type.</span></span> <span data-ttu-id="7e9c4-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e9c4-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7e9c4-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="7e9c4-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="7e9c4-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="7e9c4-189">loginGroupOrDomain</span></span>|<span data-ttu-id="7e9c4-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-190">String</span></span>|<span data-ttu-id="7e9c4-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="7e9c4-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-193">role</span><span class="sxs-lookup"><span data-stu-id="7e9c4-193">role</span></span>|<span data-ttu-id="7e9c4-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-194">String</span></span>|<span data-ttu-id="7e9c4-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7e9c4-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-197">realm</span><span class="sxs-lookup"><span data-stu-id="7e9c4-197">realm</span></span>|<span data-ttu-id="7e9c4-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-198">String</span></span>|<span data-ttu-id="7e9c4-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7e9c4-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-201">server</span><span class="sxs-lookup"><span data-stu-id="7e9c4-201">server</span></span>|[<span data-ttu-id="7e9c4-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="7e9c4-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="7e9c4-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-203">VPN Server on the network.</span></span> <span data-ttu-id="7e9c4-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="7e9c4-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-206">identificador</span><span class="sxs-lookup"><span data-stu-id="7e9c4-206">identifier</span></span>|<span data-ttu-id="7e9c4-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-207">String</span></span>|<span data-ttu-id="7e9c4-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7e9c4-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-210">customData</span><span class="sxs-lookup"><span data-stu-id="7e9c4-210">customData</span></span>|<span data-ttu-id="7e9c4-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="7e9c4-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7e9c4-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7e9c4-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7e9c4-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7e9c4-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="7e9c4-217">customKeyValueData</span></span>|<span data-ttu-id="7e9c4-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7e9c4-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7e9c4-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7e9c4-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7e9c4-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7e9c4-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="7e9c4-224">enableSplitTunneling</span></span>|<span data-ttu-id="7e9c4-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-225">Boolean</span></span>|<span data-ttu-id="7e9c4-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="7e9c4-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e9c4-228">authenticationMethod</span></span>|[<span data-ttu-id="7e9c4-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e9c4-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7e9c4-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="7e9c4-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e9c4-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7e9c4-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="7e9c4-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="7e9c4-233">enablePerApp</span></span>|<span data-ttu-id="7e9c4-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-234">Boolean</span></span>|<span data-ttu-id="7e9c4-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="7e9c4-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="7e9c4-237">safariDomains</span></span>|<span data-ttu-id="7e9c4-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-238">String collection</span></span>|<span data-ttu-id="7e9c4-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="7e9c4-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="7e9c4-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="7e9c4-242">onDemandRules</span></span>|<span data-ttu-id="7e9c4-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="7e9c4-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-244">On-Demand Rules.</span></span> <span data-ttu-id="7e9c4-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7e9c4-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-247">providerType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-247">providerType</span></span>|[<span data-ttu-id="7e9c4-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="7e9c4-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="7e9c4-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e9c4-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7e9c4-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="7e9c4-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="7e9c4-252">associatedDomains</span></span>|<span data-ttu-id="7e9c4-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-253">String collection</span></span>|<span data-ttu-id="7e9c4-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="7e9c4-255">excludedDomains</span></span>|<span data-ttu-id="7e9c4-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-256">String collection</span></span>|<span data-ttu-id="7e9c4-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="7e9c4-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="7e9c4-259">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-259">Boolean</span></span>|<span data-ttu-id="7e9c4-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="7e9c4-261">proxyServer</span></span>|[<span data-ttu-id="7e9c4-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7e9c4-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="7e9c4-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-263">Proxy Server.</span></span> <span data-ttu-id="7e9c4-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="7e9c4-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="7e9c4-266">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-266">Boolean</span></span>|<span data-ttu-id="7e9c4-267">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="7e9c4-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="7e9c4-269">userDomain</span></span>|<span data-ttu-id="7e9c4-270">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-270">String</span></span>|<span data-ttu-id="7e9c4-271">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-271">Zscaler only.</span></span> <span data-ttu-id="7e9c4-272">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="7e9c4-273">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="7e9c4-274">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-274">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-275">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="7e9c4-275">strictEnforcement</span></span>|<span data-ttu-id="7e9c4-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-276">Boolean</span></span>|<span data-ttu-id="7e9c4-277">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-277">Zscaler only.</span></span> <span data-ttu-id="7e9c4-278">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-278">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="7e9c4-279">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-279">"True" means traffic is blocked.</span></span> <span data-ttu-id="7e9c4-280">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-281">cloudName</span><span class="sxs-lookup"><span data-stu-id="7e9c4-281">cloudName</span></span>|<span data-ttu-id="7e9c4-282">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-282">String</span></span>|<span data-ttu-id="7e9c4-283">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-283">Zscaler only.</span></span> <span data-ttu-id="7e9c4-284">Nuvem Zscaler à qual o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-284">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="7e9c4-285">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-285">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-286">excludeList</span><span class="sxs-lookup"><span data-stu-id="7e9c4-286">excludeList</span></span>|<span data-ttu-id="7e9c4-287">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-287">String collection</span></span>|<span data-ttu-id="7e9c4-288">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-288">Zscaler only.</span></span> <span data-ttu-id="7e9c4-289">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-289">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="7e9c4-290">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-290">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-291">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7e9c4-291">targetedMobileApps</span></span>|<span data-ttu-id="7e9c4-292">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-292">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7e9c4-293">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-293">Targeted mobile apps.</span></span> <span data-ttu-id="7e9c4-294">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-294">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7e9c4-295">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-295">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-296">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="7e9c4-296">microsoftTunnelSiteId</span></span>|<span data-ttu-id="7e9c4-297">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-297">String</span></span>|<span data-ttu-id="7e9c4-298">ID do site do Túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-298">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="7e9c4-299">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e9c4-299">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e9c4-300">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-300">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="7e9c4-301">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-301">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="7e9c4-302">Parâmetros de associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="7e9c4-302">Child Security Association Parameters</span></span>|
|<span data-ttu-id="7e9c4-303">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-303">clientAuthenticationType</span></span>|[<span data-ttu-id="7e9c4-304">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-304">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="7e9c4-305">Tipo de Autenticação de Cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-305">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="7e9c4-306">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-306">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="7e9c4-307">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="7e9c4-307">deadPeerDetectionRate</span></span>|[<span data-ttu-id="7e9c4-308">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="7e9c4-308">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="7e9c4-309">Determine com que frequência verificar se uma conexão de par ainda está ativa.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-309">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="7e9c4-310">.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-310">.</span></span> <span data-ttu-id="7e9c4-311">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-311">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="7e9c4-312">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="7e9c4-312">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="7e9c4-313">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-313">Boolean</span></span>|<span data-ttu-id="7e9c4-314">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="7e9c4-314">Disable MOBIKE</span></span>|
|<span data-ttu-id="7e9c4-315">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="7e9c4-315">disableRedirect</span></span>|<span data-ttu-id="7e9c4-316">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-316">Boolean</span></span>|<span data-ttu-id="7e9c4-317">Desabilitar Redirecionamento</span><span class="sxs-lookup"><span data-stu-id="7e9c4-317">Disable Redirect</span></span>|
|<span data-ttu-id="7e9c4-318">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="7e9c4-318">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="7e9c4-319">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-319">Boolean</span></span>|<span data-ttu-id="7e9c4-320">Habilita uma verificação de revogação de melhor esforço; tempo-de-tempo de resposta do servidor não fará com que ele falhe</span><span class="sxs-lookup"><span data-stu-id="7e9c4-320">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="7e9c4-321">enableEAP</span><span class="sxs-lookup"><span data-stu-id="7e9c4-321">enableEAP</span></span>|<span data-ttu-id="7e9c4-322">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-322">Boolean</span></span>|<span data-ttu-id="7e9c4-323">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="7e9c4-323">Enables EAP only authentication</span></span>|
|<span data-ttu-id="7e9c4-324">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="7e9c4-324">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="7e9c4-325">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-325">Boolean</span></span>|<span data-ttu-id="7e9c4-326">Habilitar o PFS (Segredo de Encaminhamento Perfeito).</span><span class="sxs-lookup"><span data-stu-id="7e9c4-326">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="7e9c4-327">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="7e9c4-327">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="7e9c4-328">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-328">Boolean</span></span>|<span data-ttu-id="7e9c4-329">Habilitar usar atributos de sub-rede internas.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-329">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="7e9c4-330">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e9c4-330">localIdentifier</span></span>|[<span data-ttu-id="7e9c4-331">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e9c4-331">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="7e9c4-332">Método de identificar o cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-332">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="7e9c4-333">.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-333">.</span></span> <span data-ttu-id="7e9c4-334">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-334">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="7e9c4-335">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e9c4-335">remoteIdentifier</span></span>|<span data-ttu-id="7e9c4-336">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-336">String</span></span>|<span data-ttu-id="7e9c4-337">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-337">Address of the IKEv2 server.</span></span> <span data-ttu-id="7e9c4-338">Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="7e9c4-338">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="7e9c4-339">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-339">securityAssociationParameters</span></span>|[<span data-ttu-id="7e9c4-340">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-340">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="7e9c4-341">Parâmetros de Associação de Segurança</span><span class="sxs-lookup"><span data-stu-id="7e9c4-341">Security Association Parameters</span></span>|
|<span data-ttu-id="7e9c4-342">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="7e9c4-342">serverCertificateCommonName</span></span>|<span data-ttu-id="7e9c4-343">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-343">String</span></span>|<span data-ttu-id="7e9c4-344">Nome comum do Certificado de Servidor IKEv2 usado na Autenticação do Servidor</span><span class="sxs-lookup"><span data-stu-id="7e9c4-344">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="7e9c4-345">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="7e9c4-345">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="7e9c4-346">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-346">String</span></span>|<span data-ttu-id="7e9c4-347">Nome comum do emissor do emissor de Certificado do Servidor IKEv2 usado na Autenticação</span><span class="sxs-lookup"><span data-stu-id="7e9c4-347">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="7e9c4-348">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-348">serverCertificateType</span></span>|[<span data-ttu-id="7e9c4-349">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="7e9c4-349">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="7e9c4-350">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-350">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="7e9c4-351">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-351">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="7e9c4-352">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="7e9c4-352">sharedSecret</span></span>|<span data-ttu-id="7e9c4-353">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-353">String</span></span>|<span data-ttu-id="7e9c4-354">Usado quando a Autenticação Secreta Compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="7e9c4-354">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="7e9c4-355">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7e9c4-355">tlsMaximumVersion</span></span>|<span data-ttu-id="7e9c4-356">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-356">String</span></span>|<span data-ttu-id="7e9c4-357">A versão TLS máxima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="7e9c4-357">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="7e9c4-358">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7e9c4-358">tlsMinimumVersion</span></span>|<span data-ttu-id="7e9c4-359">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9c4-359">String</span></span>|<span data-ttu-id="7e9c4-360">A versão TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="7e9c4-360">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="7e9c4-361">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-361">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="7e9c4-362">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-362">Boolean</span></span>|<span data-ttu-id="7e9c4-363">Permite o uso de parâmetros de associação de segurança definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-363">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="7e9c4-364">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7e9c4-364">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="7e9c4-365">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-365">Boolean</span></span>|<span data-ttu-id="7e9c4-366">Permite o uso de parâmetros de associação de segurança filho definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-366">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="7e9c4-367">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e9c4-367">alwaysOnConfiguration</span></span>|[<span data-ttu-id="7e9c4-368">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e9c4-368">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="7e9c4-369">Configuração AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="7e9c4-369">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="7e9c4-370">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e9c4-370">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="7e9c4-371">Booleano</span><span class="sxs-lookup"><span data-stu-id="7e9c4-371">Boolean</span></span>|<span data-ttu-id="7e9c4-372">Determina se a VPN Always on está habilitada</span><span class="sxs-lookup"><span data-stu-id="7e9c4-372">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="7e9c4-373">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="7e9c4-373">mtuSizeInBytes</span></span>|<span data-ttu-id="7e9c4-374">Int32</span><span class="sxs-lookup"><span data-stu-id="7e9c4-374">Int32</span></span>|<span data-ttu-id="7e9c4-375">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-375">Maximum transmission unit.</span></span> <span data-ttu-id="7e9c4-376">Valores válidos de 1280 a 1400</span><span class="sxs-lookup"><span data-stu-id="7e9c4-376">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="7e9c4-377">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9c4-377">Response</span></span>
<span data-ttu-id="7e9c4-378">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-378">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e9c4-379">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e9c4-379">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e9c4-380">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9c4-380">Request</span></span>
<span data-ttu-id="7e9c4-381">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-381">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5492

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```

### <a name="response"></a><span data-ttu-id="7e9c4-382">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9c4-382">Response</span></span>
<span data-ttu-id="7e9c4-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e9c4-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5664

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```




