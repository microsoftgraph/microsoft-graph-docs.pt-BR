---
title: Criar macOSVpnConfiguration
description: Crie um novo objeto macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5b22cb759459599118632047e12e9693910ad9f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157985"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="0912f-103">Criar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0912f-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="0912f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0912f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0912f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0912f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0912f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0912f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0912f-107">Crie um novo [objeto macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0912f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0912f-108">Prerequisites</span></span>
<span data-ttu-id="0912f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0912f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0912f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0912f-111">Permission type</span></span>|<span data-ttu-id="0912f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0912f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0912f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0912f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0912f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0912f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0912f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0912f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0912f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0912f-116">Not supported.</span></span>|
|<span data-ttu-id="0912f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0912f-117">Application</span></span>|<span data-ttu-id="0912f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0912f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0912f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0912f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0912f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0912f-120">Request headers</span></span>
|<span data-ttu-id="0912f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0912f-121">Header</span></span>|<span data-ttu-id="0912f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0912f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0912f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0912f-123">Authorization</span></span>|<span data-ttu-id="0912f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0912f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0912f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0912f-125">Accept</span></span>|<span data-ttu-id="0912f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0912f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0912f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0912f-127">Request body</span></span>
<span data-ttu-id="0912f-128">No corpo da solicitação, fornece uma representação JSON do objeto macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0912f-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="0912f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0912f-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="0912f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0912f-130">Property</span></span>|<span data-ttu-id="0912f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0912f-131">Type</span></span>|<span data-ttu-id="0912f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0912f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0912f-133">id</span><span class="sxs-lookup"><span data-stu-id="0912f-133">id</span></span>|<span data-ttu-id="0912f-134">String</span><span class="sxs-lookup"><span data-stu-id="0912f-134">String</span></span>|<span data-ttu-id="0912f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0912f-135">Key of the entity.</span></span> <span data-ttu-id="0912f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0912f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0912f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0912f-138">DateTimeOffset</span></span>|<span data-ttu-id="0912f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0912f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0912f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0912f-141">roleScopeTagIds</span></span>|<span data-ttu-id="0912f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0912f-142">String collection</span></span>|<span data-ttu-id="0912f-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="0912f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0912f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0912f-145">supportsScopeTags</span></span>|<span data-ttu-id="0912f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0912f-146">Boolean</span></span>|<span data-ttu-id="0912f-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0912f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0912f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0912f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0912f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0912f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0912f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0912f-150">This property is read-only.</span></span> <span data-ttu-id="0912f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0912f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0912f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0912f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0912f-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0912f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0912f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0912f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0912f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0912f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0912f-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0912f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0912f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0912f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0912f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0912f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0912f-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="0912f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0912f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0912f-164">createdDateTime</span></span>|<span data-ttu-id="0912f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0912f-165">DateTimeOffset</span></span>|<span data-ttu-id="0912f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0912f-166">DateTime the object was created.</span></span> <span data-ttu-id="0912f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-168">description</span><span class="sxs-lookup"><span data-stu-id="0912f-168">description</span></span>|<span data-ttu-id="0912f-169">String</span><span class="sxs-lookup"><span data-stu-id="0912f-169">String</span></span>|<span data-ttu-id="0912f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0912f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0912f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0912f-172">displayName</span></span>|<span data-ttu-id="0912f-173">String</span><span class="sxs-lookup"><span data-stu-id="0912f-173">String</span></span>|<span data-ttu-id="0912f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0912f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0912f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-176">versão</span><span class="sxs-lookup"><span data-stu-id="0912f-176">version</span></span>|<span data-ttu-id="0912f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0912f-177">Int32</span></span>|<span data-ttu-id="0912f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0912f-178">Version of the device configuration.</span></span> <span data-ttu-id="0912f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="0912f-180">connectionName</span></span>|<span data-ttu-id="0912f-181">String</span><span class="sxs-lookup"><span data-stu-id="0912f-181">String</span></span>|<span data-ttu-id="0912f-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0912f-182">Connection name displayed to the user.</span></span> <span data-ttu-id="0912f-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="0912f-184">connectionType</span></span>|[<span data-ttu-id="0912f-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0912f-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0912f-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="0912f-186">Connection type.</span></span> <span data-ttu-id="0912f-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0912f-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0912f-188">Os valores possíveis `ciscoAnyConnect` são: `pulseSecure` , , , , , , , , `f5EdgeClient` , , , , , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="0912f-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="0912f-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0912f-189">loginGroupOrDomain</span></span>|<span data-ttu-id="0912f-190">String</span><span class="sxs-lookup"><span data-stu-id="0912f-190">String</span></span>|<span data-ttu-id="0912f-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="0912f-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0912f-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-193">role</span><span class="sxs-lookup"><span data-stu-id="0912f-193">role</span></span>|<span data-ttu-id="0912f-194">String</span><span class="sxs-lookup"><span data-stu-id="0912f-194">String</span></span>|<span data-ttu-id="0912f-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="0912f-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0912f-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-197">realm</span><span class="sxs-lookup"><span data-stu-id="0912f-197">realm</span></span>|<span data-ttu-id="0912f-198">String</span><span class="sxs-lookup"><span data-stu-id="0912f-198">String</span></span>|<span data-ttu-id="0912f-199">Realm quando o tipo de conexão está definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="0912f-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0912f-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-201">server</span><span class="sxs-lookup"><span data-stu-id="0912f-201">server</span></span>|[<span data-ttu-id="0912f-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0912f-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0912f-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="0912f-203">VPN Server on the network.</span></span> <span data-ttu-id="0912f-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="0912f-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="0912f-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-206">identificador</span><span class="sxs-lookup"><span data-stu-id="0912f-206">identifier</span></span>|<span data-ttu-id="0912f-207">String</span><span class="sxs-lookup"><span data-stu-id="0912f-207">String</span></span>|<span data-ttu-id="0912f-208">Identificador fornecido pelo fornecedor de VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0912f-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0912f-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-210">customData</span><span class="sxs-lookup"><span data-stu-id="0912f-210">customData</span></span>|<span data-ttu-id="0912f-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0912f-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0912f-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0912f-213">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0912f-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0912f-214">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0912f-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0912f-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0912f-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0912f-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0912f-217">customKeyValueData</span></span>|<span data-ttu-id="0912f-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0912f-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="0912f-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0912f-220">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0912f-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0912f-221">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0912f-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0912f-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0912f-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0912f-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0912f-224">enableSplitTunneling</span></span>|<span data-ttu-id="0912f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0912f-225">Boolean</span></span>|<span data-ttu-id="0912f-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="0912f-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="0912f-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0912f-228">authenticationMethod</span></span>|[<span data-ttu-id="0912f-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0912f-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0912f-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0912f-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0912f-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0912f-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0912f-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="0912f-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="0912f-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0912f-233">enablePerApp</span></span>|<span data-ttu-id="0912f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0912f-234">Boolean</span></span>|<span data-ttu-id="0912f-235">Definir isso como verdadeiro cria Per-App de VPN que pode ser associada posteriormente a aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0912f-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0912f-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0912f-237">safariDomains</span></span>|<span data-ttu-id="0912f-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0912f-238">String collection</span></span>|<span data-ttu-id="0912f-239">Domínios do Safari quando essa configuração vpn por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="0912f-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0912f-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0912f-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0912f-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0912f-242">onDemandRules</span></span>|<span data-ttu-id="0912f-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0912f-244">Regras Sob Demanda.</span><span class="sxs-lookup"><span data-stu-id="0912f-244">On-Demand Rules.</span></span> <span data-ttu-id="0912f-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0912f-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0912f-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-247">providerType</span><span class="sxs-lookup"><span data-stu-id="0912f-247">providerType</span></span>|[<span data-ttu-id="0912f-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0912f-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0912f-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0912f-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="0912f-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0912f-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0912f-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="0912f-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0912f-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="0912f-252">associatedDomains</span></span>|<span data-ttu-id="0912f-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0912f-253">String collection</span></span>|<span data-ttu-id="0912f-254">Domínios Associados Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="0912f-255">excludedDomains</span></span>|<span data-ttu-id="0912f-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0912f-256">String collection</span></span>|<span data-ttu-id="0912f-257">Domínios que são acessados por meio da Internet pública em vez de via VPN, mesmo quando a VPN por aplicativo é ativada Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="0912f-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="0912f-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="0912f-259">Boolean</span></span>|<span data-ttu-id="0912f-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0912f-261">proxyServer</span></span>|[<span data-ttu-id="0912f-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0912f-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0912f-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="0912f-263">Proxy Server.</span></span> <span data-ttu-id="0912f-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0912f-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0912f-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0912f-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="0912f-266">Boolean</span></span>|<span data-ttu-id="0912f-267">Opt-In compartilhar a ID do dispositivo com clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="0912f-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0912f-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0912f-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0912f-269">Resposta</span><span class="sxs-lookup"><span data-stu-id="0912f-269">Response</span></span>
<span data-ttu-id="0912f-270">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0912f-270">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0912f-271">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0912f-271">Example</span></span>

### <a name="request"></a><span data-ttu-id="0912f-272">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0912f-272">Request</span></span>
<span data-ttu-id="0912f-273">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0912f-273">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2825

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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="0912f-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="0912f-274">Response</span></span>
<span data-ttu-id="0912f-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0912f-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2997

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
  "optInToDeviceIdSharing": true
}
```




