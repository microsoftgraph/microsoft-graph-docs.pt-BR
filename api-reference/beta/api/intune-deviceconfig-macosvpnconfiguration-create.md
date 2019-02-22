---
title: Criar macOSVpnConfiguration
description: Criar um novo objeto macOSVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cddd5c692aae773ccb5421f61c1e122f8da6b82
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155115"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="ca6eb-103">Criar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca6eb-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="ca6eb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca6eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca6eb-106">Criar um novo objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ca6eb-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca6eb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca6eb-107">Prerequisites</span></span>
<span data-ttu-id="ca6eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca6eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca6eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca6eb-110">Permission type</span></span>|<span data-ttu-id="ca6eb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca6eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca6eb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca6eb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca6eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca6eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-115">Not supported.</span></span>|
|<span data-ttu-id="ca6eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca6eb-116">Application</span></span>|<span data-ttu-id="ca6eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca6eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca6eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6eb-119">Request headers</span></span>
|<span data-ttu-id="ca6eb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca6eb-120">Header</span></span>|<span data-ttu-id="ca6eb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca6eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca6eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca6eb-122">Authorization</span></span>|<span data-ttu-id="ca6eb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca6eb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca6eb-124">Accept</span></span>|<span data-ttu-id="ca6eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca6eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca6eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6eb-126">Request body</span></span>
<span data-ttu-id="ca6eb-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="ca6eb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="ca6eb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca6eb-129">Property</span></span>|<span data-ttu-id="ca6eb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca6eb-130">Type</span></span>|<span data-ttu-id="ca6eb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6eb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca6eb-132">id</span><span class="sxs-lookup"><span data-stu-id="ca6eb-132">id</span></span>|<span data-ttu-id="ca6eb-133">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-133">String</span></span>|<span data-ttu-id="ca6eb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-134">Key of the entity.</span></span> <span data-ttu-id="ca6eb-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca6eb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ca6eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca6eb-137">DateTimeOffset</span></span>|<span data-ttu-id="ca6eb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ca6eb-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca6eb-140">roleScopeTagIds</span></span>|<span data-ttu-id="ca6eb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6eb-141">String collection</span></span>|<span data-ttu-id="ca6eb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca6eb-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca6eb-144">supportsScopeTags</span></span>|<span data-ttu-id="ca6eb-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca6eb-145">Boolean</span></span>|<span data-ttu-id="ca6eb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca6eb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca6eb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca6eb-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-149">This property is read-only.</span></span> <span data-ttu-id="ca6eb-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca6eb-151">createdDateTime</span></span>|<span data-ttu-id="ca6eb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca6eb-152">DateTimeOffset</span></span>|<span data-ttu-id="ca6eb-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-153">DateTime the object was created.</span></span> <span data-ttu-id="ca6eb-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-155">description</span><span class="sxs-lookup"><span data-stu-id="ca6eb-155">description</span></span>|<span data-ttu-id="ca6eb-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6eb-156">String</span></span>|<span data-ttu-id="ca6eb-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca6eb-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ca6eb-159">displayName</span></span>|<span data-ttu-id="ca6eb-160">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-160">String</span></span>|<span data-ttu-id="ca6eb-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca6eb-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-163">version</span><span class="sxs-lookup"><span data-stu-id="ca6eb-163">version</span></span>|<span data-ttu-id="ca6eb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ca6eb-164">Int32</span></span>|<span data-ttu-id="ca6eb-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-165">Version of the device configuration.</span></span> <span data-ttu-id="ca6eb-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-167">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="ca6eb-167">connectionName</span></span>|<span data-ttu-id="ca6eb-168">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-168">String</span></span>|<span data-ttu-id="ca6eb-169">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-169">Connection name displayed to the user.</span></span> <span data-ttu-id="ca6eb-170">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-171">Connection</span><span class="sxs-lookup"><span data-stu-id="ca6eb-171">connectionType</span></span>|[<span data-ttu-id="ca6eb-172">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="ca6eb-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ca6eb-173">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-173">Connection type.</span></span> <span data-ttu-id="ca6eb-174">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca6eb-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ca6eb-175">Os valores possíveis são `ciscoAnyConnect`: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="ca6eb-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ca6eb-176">loginGroupOrDomain</span></span>|<span data-ttu-id="ca6eb-177">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-177">String</span></span>|<span data-ttu-id="ca6eb-178">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ca6eb-179">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-180">role</span><span class="sxs-lookup"><span data-stu-id="ca6eb-180">role</span></span>|<span data-ttu-id="ca6eb-181">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-181">String</span></span>|<span data-ttu-id="ca6eb-182">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ca6eb-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-184">esfera</span><span class="sxs-lookup"><span data-stu-id="ca6eb-184">realm</span></span>|<span data-ttu-id="ca6eb-185">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-185">String</span></span>|<span data-ttu-id="ca6eb-186">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ca6eb-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-188">do</span><span class="sxs-lookup"><span data-stu-id="ca6eb-188">server</span></span>|[<span data-ttu-id="ca6eb-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="ca6eb-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ca6eb-190">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-190">VPN Server on the network.</span></span> <span data-ttu-id="ca6eb-191">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="ca6eb-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-193">identificador</span><span class="sxs-lookup"><span data-stu-id="ca6eb-193">identifier</span></span>|<span data-ttu-id="ca6eb-194">String</span><span class="sxs-lookup"><span data-stu-id="ca6eb-194">String</span></span>|<span data-ttu-id="ca6eb-195">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ca6eb-196">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-197">customData</span><span class="sxs-lookup"><span data-stu-id="ca6eb-197">customData</span></span>|<span data-ttu-id="ca6eb-198">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ca6eb-199">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ca6eb-200">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ca6eb-201">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ca6eb-202">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ca6eb-203">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-204">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="ca6eb-204">customKeyValueData</span></span>|<span data-ttu-id="ca6eb-205">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ca6eb-206">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ca6eb-207">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ca6eb-208">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ca6eb-209">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ca6eb-210">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ca6eb-211">enableSplitTunneling</span></span>|<span data-ttu-id="ca6eb-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca6eb-212">Boolean</span></span>|<span data-ttu-id="ca6eb-213">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="ca6eb-214">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ca6eb-215">authenticationMethod</span></span>|[<span data-ttu-id="ca6eb-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ca6eb-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ca6eb-217">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ca6eb-218">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca6eb-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ca6eb-219">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="ca6eb-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="ca6eb-220">enablePerApp</span></span>|<span data-ttu-id="ca6eb-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca6eb-221">Boolean</span></span>|<span data-ttu-id="ca6eb-222">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ca6eb-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="ca6eb-224">safariDomains</span></span>|<span data-ttu-id="ca6eb-225">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6eb-225">String collection</span></span>|<span data-ttu-id="ca6eb-226">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ca6eb-227">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ca6eb-228">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="ca6eb-229">onDemandRules</span></span>|<span data-ttu-id="ca6eb-230">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ca6eb-231">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-231">On-Demand Rules.</span></span> <span data-ttu-id="ca6eb-232">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ca6eb-233">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ca6eb-234">proxyServer</span></span>|[<span data-ttu-id="ca6eb-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ca6eb-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ca6eb-236">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-236">Proxy Server.</span></span> <span data-ttu-id="ca6eb-237">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ca6eb-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="ca6eb-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ca6eb-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca6eb-239">Boolean</span></span>|<span data-ttu-id="ca6eb-240">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ca6eb-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca6eb-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ca6eb-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6eb-242">Response</span></span>
<span data-ttu-id="ca6eb-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-243">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca6eb-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca6eb-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca6eb-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6eb-245">Request</span></span>
<span data-ttu-id="ca6eb-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="ca6eb-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6eb-247">Response</span></span>
<span data-ttu-id="ca6eb-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca6eb-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




