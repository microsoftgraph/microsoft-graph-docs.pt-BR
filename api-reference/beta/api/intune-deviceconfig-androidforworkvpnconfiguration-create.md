---
title: Criar androidForWorkVpnConfiguration
description: Crie um novo objeto androidForWorkVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6061004519c86b25ae8aa3794e5c02f56ff810
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138215"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="9bb61-103">Criar androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bb61-103">Create androidForWorkVpnConfiguration</span></span>

<span data-ttu-id="9bb61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bb61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bb61-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bb61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bb61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bb61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb61-107">Crie um novo [objeto androidForWorkVpnConfiguration.](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb61-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bb61-108">Prerequisites</span></span>
<span data-ttu-id="9bb61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb61-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bb61-111">Permission type</span></span>|<span data-ttu-id="9bb61-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bb61-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb61-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bb61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bb61-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bb61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bb61-116">Not supported.</span></span>|
|<span data-ttu-id="9bb61-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bb61-117">Application</span></span>|<span data-ttu-id="9bb61-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb61-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb61-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bb61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9bb61-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb61-120">Request headers</span></span>
|<span data-ttu-id="9bb61-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bb61-121">Header</span></span>|<span data-ttu-id="9bb61-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bb61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb61-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bb61-123">Authorization</span></span>|<span data-ttu-id="9bb61-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bb61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb61-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bb61-125">Accept</span></span>|<span data-ttu-id="9bb61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb61-127">Request body</span></span>
<span data-ttu-id="9bb61-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bb61-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="9bb61-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bb61-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="9bb61-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bb61-130">Property</span></span>|<span data-ttu-id="9bb61-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bb61-131">Type</span></span>|<span data-ttu-id="9bb61-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bb61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb61-133">id</span><span class="sxs-lookup"><span data-stu-id="9bb61-133">id</span></span>|<span data-ttu-id="9bb61-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-134">String</span></span>|<span data-ttu-id="9bb61-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9bb61-135">Key of the entity.</span></span> <span data-ttu-id="9bb61-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb61-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9bb61-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb61-138">DateTimeOffset</span></span>|<span data-ttu-id="9bb61-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9bb61-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9bb61-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bb61-141">roleScopeTagIds</span></span>|<span data-ttu-id="9bb61-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-142">String collection</span></span>|<span data-ttu-id="9bb61-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="9bb61-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9bb61-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9bb61-145">supportsScopeTags</span></span>|<span data-ttu-id="9bb61-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="9bb61-146">Boolean</span></span>|<span data-ttu-id="9bb61-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9bb61-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9bb61-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9bb61-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9bb61-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bb61-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9bb61-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bb61-150">This property is read-only.</span></span> <span data-ttu-id="9bb61-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9bb61-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9bb61-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9bb61-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9bb61-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9bb61-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9bb61-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9bb61-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9bb61-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9bb61-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9bb61-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9bb61-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9bb61-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9bb61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9bb61-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9bb61-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9bb61-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9bb61-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9bb61-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bb61-164">createdDateTime</span></span>|<span data-ttu-id="9bb61-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bb61-165">DateTimeOffset</span></span>|<span data-ttu-id="9bb61-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9bb61-166">DateTime the object was created.</span></span> <span data-ttu-id="9bb61-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-168">descrição</span><span class="sxs-lookup"><span data-stu-id="9bb61-168">description</span></span>|<span data-ttu-id="9bb61-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-169">String</span></span>|<span data-ttu-id="9bb61-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bb61-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9bb61-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9bb61-172">displayName</span></span>|<span data-ttu-id="9bb61-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-173">String</span></span>|<span data-ttu-id="9bb61-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bb61-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9bb61-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-176">versão</span><span class="sxs-lookup"><span data-stu-id="9bb61-176">version</span></span>|<span data-ttu-id="9bb61-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9bb61-177">Int32</span></span>|<span data-ttu-id="9bb61-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bb61-178">Version of the device configuration.</span></span> <span data-ttu-id="9bb61-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bb61-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="9bb61-180">connectionName</span></span>|<span data-ttu-id="9bb61-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-181">String</span></span>|<span data-ttu-id="9bb61-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9bb61-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="9bb61-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="9bb61-183">connectionType</span></span>|[<span data-ttu-id="9bb61-184">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9bb61-184">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="9bb61-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="9bb61-185">Connection type.</span></span> <span data-ttu-id="9bb61-186">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="9bb61-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="9bb61-187">role</span><span class="sxs-lookup"><span data-stu-id="9bb61-187">role</span></span>|<span data-ttu-id="9bb61-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-188">String</span></span>|<span data-ttu-id="9bb61-189">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="9bb61-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9bb61-190">realm</span><span class="sxs-lookup"><span data-stu-id="9bb61-190">realm</span></span>|<span data-ttu-id="9bb61-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-191">String</span></span>|<span data-ttu-id="9bb61-192">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="9bb61-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9bb61-193">servers</span><span class="sxs-lookup"><span data-stu-id="9bb61-193">servers</span></span>|<span data-ttu-id="9bb61-194">[Coleção vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9bb61-195">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="9bb61-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="9bb61-196">Certifique-se de que os usuários finais possam acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="9bb61-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9bb61-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9bb61-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9bb61-198">fingerprint</span><span class="sxs-lookup"><span data-stu-id="9bb61-198">fingerprint</span></span>|<span data-ttu-id="9bb61-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bb61-199">String</span></span>|<span data-ttu-id="9bb61-200">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é Check Point Capsule VPN.</span><span class="sxs-lookup"><span data-stu-id="9bb61-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9bb61-201">customData</span><span class="sxs-lookup"><span data-stu-id="9bb61-201">customData</span></span>|<span data-ttu-id="9bb61-202">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="9bb61-203">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="9bb61-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9bb61-204">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="9bb61-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9bb61-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="9bb61-205">customKeyValueData</span></span>|<span data-ttu-id="9bb61-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9bb61-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9bb61-207">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="9bb61-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9bb61-208">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="9bb61-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9bb61-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bb61-209">authenticationMethod</span></span>|[<span data-ttu-id="9bb61-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bb61-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9bb61-211">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="9bb61-211">Authentication method.</span></span> <span data-ttu-id="9bb61-212">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="9bb61-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="9bb61-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb61-213">Response</span></span>
<span data-ttu-id="9bb61-214">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bb61-214">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb61-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bb61-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb61-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bb61-216">Request</span></span>
<span data-ttu-id="9bb61-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bb61-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1758

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="9bb61-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bb61-218">Response</span></span>
<span data-ttu-id="9bb61-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bb61-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1930

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```




