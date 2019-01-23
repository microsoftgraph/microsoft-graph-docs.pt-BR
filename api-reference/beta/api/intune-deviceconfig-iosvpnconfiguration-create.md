---
title: Criar iosVpnConfiguration
description: Crie um novo objeto de iosVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4d7b61d439af1403e684cbc54be05725ac2ef801
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409157"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="0317c-103">Criar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0317c-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="0317c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0317c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0317c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0317c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0317c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0317c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0317c-107">Crie um novo objeto de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0317c-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0317c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0317c-108">Prerequisites</span></span>
<span data-ttu-id="0317c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0317c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0317c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0317c-111">Permission type</span></span>|<span data-ttu-id="0317c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0317c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0317c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0317c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0317c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0317c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0317c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0317c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0317c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0317c-116">Not supported.</span></span>|
|<span data-ttu-id="0317c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0317c-117">Application</span></span>|<span data-ttu-id="0317c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0317c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0317c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0317c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0317c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0317c-120">Request headers</span></span>
|<span data-ttu-id="0317c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0317c-121">Header</span></span>|<span data-ttu-id="0317c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0317c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0317c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0317c-123">Authorization</span></span>|<span data-ttu-id="0317c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0317c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0317c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0317c-125">Accept</span></span>|<span data-ttu-id="0317c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0317c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0317c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0317c-127">Request body</span></span>
<span data-ttu-id="0317c-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0317c-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="0317c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0317c-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="0317c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0317c-130">Property</span></span>|<span data-ttu-id="0317c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0317c-131">Type</span></span>|<span data-ttu-id="0317c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0317c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0317c-133">id</span><span class="sxs-lookup"><span data-stu-id="0317c-133">id</span></span>|<span data-ttu-id="0317c-134">String</span><span class="sxs-lookup"><span data-stu-id="0317c-134">String</span></span>|<span data-ttu-id="0317c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0317c-135">Key of the entity.</span></span> <span data-ttu-id="0317c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0317c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0317c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0317c-138">DateTimeOffset</span></span>|<span data-ttu-id="0317c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0317c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0317c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0317c-141">roleScopeTagIds</span></span>|<span data-ttu-id="0317c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0317c-142">String collection</span></span>|<span data-ttu-id="0317c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="0317c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0317c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0317c-145">supportsScopeTags</span></span>|<span data-ttu-id="0317c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0317c-146">Boolean</span></span>|<span data-ttu-id="0317c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0317c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0317c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0317c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0317c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="0317c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0317c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0317c-150">This property is read-only.</span></span> <span data-ttu-id="0317c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0317c-152">createdDateTime</span></span>|<span data-ttu-id="0317c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0317c-153">DateTimeOffset</span></span>|<span data-ttu-id="0317c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0317c-154">DateTime the object was created.</span></span> <span data-ttu-id="0317c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-156">description</span><span class="sxs-lookup"><span data-stu-id="0317c-156">description</span></span>|<span data-ttu-id="0317c-157">String</span><span class="sxs-lookup"><span data-stu-id="0317c-157">String</span></span>|<span data-ttu-id="0317c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0317c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0317c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0317c-160">displayName</span></span>|<span data-ttu-id="0317c-161">String</span><span class="sxs-lookup"><span data-stu-id="0317c-161">String</span></span>|<span data-ttu-id="0317c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0317c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0317c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-164">version</span><span class="sxs-lookup"><span data-stu-id="0317c-164">version</span></span>|<span data-ttu-id="0317c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0317c-165">Int32</span></span>|<span data-ttu-id="0317c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0317c-166">Version of the device configuration.</span></span> <span data-ttu-id="0317c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="0317c-168">connectionName</span></span>|<span data-ttu-id="0317c-169">String</span><span class="sxs-lookup"><span data-stu-id="0317c-169">String</span></span>|<span data-ttu-id="0317c-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0317c-170">Connection name displayed to the user.</span></span> <span data-ttu-id="0317c-171">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="0317c-172">connectionType</span></span>|[<span data-ttu-id="0317c-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0317c-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0317c-174">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="0317c-174">Connection type.</span></span> <span data-ttu-id="0317c-175">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0317c-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0317c-176">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="0317c-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="0317c-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0317c-177">loginGroupOrDomain</span></span>|<span data-ttu-id="0317c-178">String</span><span class="sxs-lookup"><span data-stu-id="0317c-178">String</span></span>|<span data-ttu-id="0317c-179">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="0317c-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0317c-180">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-181">role</span><span class="sxs-lookup"><span data-stu-id="0317c-181">role</span></span>|<span data-ttu-id="0317c-182">String</span><span class="sxs-lookup"><span data-stu-id="0317c-182">String</span></span>|<span data-ttu-id="0317c-183">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="0317c-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0317c-184">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-185">território</span><span class="sxs-lookup"><span data-stu-id="0317c-185">realm</span></span>|<span data-ttu-id="0317c-186">String</span><span class="sxs-lookup"><span data-stu-id="0317c-186">String</span></span>|<span data-ttu-id="0317c-187">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="0317c-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0317c-188">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-189">servidor</span><span class="sxs-lookup"><span data-stu-id="0317c-189">server</span></span>|[<span data-ttu-id="0317c-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0317c-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0317c-191">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="0317c-191">VPN Server on the network.</span></span> <span data-ttu-id="0317c-192">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="0317c-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="0317c-193">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-194">identificador</span><span class="sxs-lookup"><span data-stu-id="0317c-194">identifier</span></span>|<span data-ttu-id="0317c-195">String</span><span class="sxs-lookup"><span data-stu-id="0317c-195">String</span></span>|<span data-ttu-id="0317c-196">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0317c-197">Por exemplo: AnyConnect do Cisco usa um identificador do formulário de com.cisco.anyconnect.applevpn.plugin Inherited de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-198">customData</span><span class="sxs-lookup"><span data-stu-id="0317c-198">customData</span></span>|<span data-ttu-id="0317c-199">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0317c-200">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0317c-201">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0317c-202">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0317c-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0317c-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0317c-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0317c-204">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0317c-205">customKeyValueData</span></span>|<span data-ttu-id="0317c-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0317c-207">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0317c-208">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0317c-209">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0317c-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0317c-210">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="0317c-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0317c-211">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0317c-212">enableSplitTunneling</span></span>|<span data-ttu-id="0317c-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0317c-213">Boolean</span></span>|<span data-ttu-id="0317c-214">Envie todo o tráfego de rede por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="0317c-215">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0317c-216">authenticationMethod</span></span>|[<span data-ttu-id="0317c-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0317c-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0317c-218">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0317c-219">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0317c-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0317c-220">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="0317c-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0317c-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0317c-221">enablePerApp</span></span>|<span data-ttu-id="0317c-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0317c-222">Boolean</span></span>|<span data-ttu-id="0317c-223">Essa configuração como true cria a carga de VPN-App que posteriormente pode ser associada aos aplicativos que podem disparar a esta conexão VPN no dispositivo de iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0317c-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0317c-224">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0317c-225">safariDomains</span></span>|<span data-ttu-id="0317c-226">String collection</span><span class="sxs-lookup"><span data-stu-id="0317c-226">String collection</span></span>|<span data-ttu-id="0317c-227">Domínios do Safari quando este VPN por configuração de App está habilitado.</span><span class="sxs-lookup"><span data-stu-id="0317c-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0317c-228">Além de aplicativos associados a este VPN, domínios Safari especificado aqui também poderão acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0317c-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0317c-229">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0317c-230">onDemandRules</span></span>|<span data-ttu-id="0317c-231">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0317c-232">Regras de sob demanda.</span><span class="sxs-lookup"><span data-stu-id="0317c-232">On-Demand Rules.</span></span> <span data-ttu-id="0317c-233">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0317c-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0317c-234">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0317c-235">proxyServer</span></span>|[<span data-ttu-id="0317c-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0317c-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0317c-237">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="0317c-237">Proxy Server.</span></span> <span data-ttu-id="0317c-238">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0317c-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0317c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="0317c-240">Boolean</span></span>|<span data-ttu-id="0317c-241">Opt-In de compartilhamento de Id do dispositivo para clientes de vpn de terceiros para uso durante a validação de controle de acesso de rede.</span><span class="sxs-lookup"><span data-stu-id="0317c-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0317c-242">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0317c-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0317c-243">providerType</span><span class="sxs-lookup"><span data-stu-id="0317c-243">providerType</span></span>|[<span data-ttu-id="0317c-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0317c-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0317c-245">Tipo de provedor para VPN-app.</span><span class="sxs-lookup"><span data-stu-id="0317c-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="0317c-246">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="0317c-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0317c-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="0317c-247">userDomain</span></span>|<span data-ttu-id="0317c-248">String</span><span class="sxs-lookup"><span data-stu-id="0317c-248">String</span></span>|<span data-ttu-id="0317c-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-249">Zscaler only.</span></span> <span data-ttu-id="0317c-250">Digite um domínio estático para preencher previamente o campo de logon com o aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0317c-251">Se isso estiver vazio, domínio do Active Directory do Azure o usuário do será usado.</span><span class="sxs-lookup"><span data-stu-id="0317c-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="0317c-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="0317c-252">strictEnforcement</span></span>|<span data-ttu-id="0317c-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="0317c-253">Boolean</span></span>|<span data-ttu-id="0317c-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-254">Zscaler only.</span></span> <span data-ttu-id="0317c-255">Bloqueia o tráfego de rede até que o usuário se conecta em Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="0317c-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0317c-256">"True" significa que o tráfego será bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0317c-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="0317c-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="0317c-257">cloudName</span></span>|<span data-ttu-id="0317c-258">String</span><span class="sxs-lookup"><span data-stu-id="0317c-258">String</span></span>|<span data-ttu-id="0317c-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-259">Zscaler only.</span></span> <span data-ttu-id="0317c-260">Nuvem de Zscaler que o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="0317c-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="0317c-261">excludeList</span><span class="sxs-lookup"><span data-stu-id="0317c-261">excludeList</span></span>|<span data-ttu-id="0317c-262">String collection</span><span class="sxs-lookup"><span data-stu-id="0317c-262">String collection</span></span>|<span data-ttu-id="0317c-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-263">Zscaler only.</span></span> <span data-ttu-id="0317c-264">Lista de endereços de rede que não são enviados através da nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="0317c-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="0317c-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="0317c-265">Response</span></span>
<span data-ttu-id="0317c-266">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0317c-266">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0317c-267">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0317c-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="0317c-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0317c-268">Request</span></span>
<span data-ttu-id="0317c-269">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0317c-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0317c-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="0317c-270">Response</span></span>
<span data-ttu-id="0317c-p132">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0317c-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```




