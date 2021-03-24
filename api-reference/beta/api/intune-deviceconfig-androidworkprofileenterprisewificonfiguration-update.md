---
title: Atualizar androidWorkProfileEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc2fecf44bd3adab0d4f78dea8dfb0d7b07331a2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148180"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="29b19-103">Atualizar androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="29b19-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="29b19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29b19-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29b19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29b19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29b19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b19-107">Atualize as propriedades de [um objeto androidWorkProfileEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-107">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29b19-108">Prerequisites</span></span>
<span data-ttu-id="29b19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29b19-111">Permission type</span></span>|<span data-ttu-id="29b19-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29b19-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b19-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29b19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29b19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29b19-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29b19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29b19-116">Not supported.</span></span>|
|<span data-ttu-id="29b19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29b19-117">Application</span></span>|<span data-ttu-id="29b19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29b19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29b19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29b19-120">Request headers</span></span>
|<span data-ttu-id="29b19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29b19-121">Header</span></span>|<span data-ttu-id="29b19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29b19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29b19-123">Authorization</span></span>|<span data-ttu-id="29b19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29b19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29b19-125">Accept</span></span>|<span data-ttu-id="29b19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29b19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29b19-127">Request body</span></span>
<span data-ttu-id="29b19-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWorkProfileEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-128">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="29b19-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29b19-129">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="29b19-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29b19-130">Property</span></span>|<span data-ttu-id="29b19-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b19-131">Type</span></span>|<span data-ttu-id="29b19-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b19-133">id</span><span class="sxs-lookup"><span data-stu-id="29b19-133">id</span></span>|<span data-ttu-id="29b19-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-134">String</span></span>|<span data-ttu-id="29b19-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29b19-135">Key of the entity.</span></span> <span data-ttu-id="29b19-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29b19-137">lastModifiedDateTime</span></span>|<span data-ttu-id="29b19-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b19-138">DateTimeOffset</span></span>|<span data-ttu-id="29b19-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="29b19-139">DateTime the object was last modified.</span></span> <span data-ttu-id="29b19-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29b19-141">roleScopeTagIds</span></span>|<span data-ttu-id="29b19-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-142">String collection</span></span>|<span data-ttu-id="29b19-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="29b19-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="29b19-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="29b19-145">supportsScopeTags</span></span>|<span data-ttu-id="29b19-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="29b19-146">Boolean</span></span>|<span data-ttu-id="29b19-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="29b19-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="29b19-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="29b19-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="29b19-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="29b19-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="29b19-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29b19-150">This property is read-only.</span></span> <span data-ttu-id="29b19-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29b19-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="29b19-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29b19-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="29b19-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="29b19-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="29b19-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29b19-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="29b19-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29b19-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="29b19-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="29b19-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="29b19-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29b19-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="29b19-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29b19-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="29b19-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="29b19-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="29b19-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29b19-164">createdDateTime</span></span>|<span data-ttu-id="29b19-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b19-165">DateTimeOffset</span></span>|<span data-ttu-id="29b19-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="29b19-166">DateTime the object was created.</span></span> <span data-ttu-id="29b19-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-168">descrição</span><span class="sxs-lookup"><span data-stu-id="29b19-168">description</span></span>|<span data-ttu-id="29b19-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-169">String</span></span>|<span data-ttu-id="29b19-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29b19-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="29b19-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-172">displayName</span><span class="sxs-lookup"><span data-stu-id="29b19-172">displayName</span></span>|<span data-ttu-id="29b19-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-173">String</span></span>|<span data-ttu-id="29b19-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29b19-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="29b19-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-176">versão</span><span class="sxs-lookup"><span data-stu-id="29b19-176">version</span></span>|<span data-ttu-id="29b19-177">Int32</span><span class="sxs-lookup"><span data-stu-id="29b19-177">Int32</span></span>|<span data-ttu-id="29b19-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29b19-178">Version of the device configuration.</span></span> <span data-ttu-id="29b19-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29b19-180">networkName</span><span class="sxs-lookup"><span data-stu-id="29b19-180">networkName</span></span>|<span data-ttu-id="29b19-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-181">String</span></span>|<span data-ttu-id="29b19-182">Nome da rede Herdado [do androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="29b19-183">ssid</span><span class="sxs-lookup"><span data-stu-id="29b19-183">ssid</span></span>|<span data-ttu-id="29b19-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-184">String</span></span>|<span data-ttu-id="29b19-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="29b19-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="29b19-186">Herdado [do androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="29b19-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="29b19-187">connectAutomatically</span></span>|<span data-ttu-id="29b19-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="29b19-188">Boolean</span></span>|<span data-ttu-id="29b19-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="29b19-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="29b19-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="29b19-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="29b19-191">Herdado [do androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="29b19-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="29b19-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="29b19-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="29b19-193">Boolean</span></span>|<span data-ttu-id="29b19-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="29b19-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="29b19-195">Herdado [do androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29b19-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="29b19-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="29b19-196">wiFiSecurityType</span></span>|[<span data-ttu-id="29b19-197">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="29b19-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="29b19-198">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="29b19-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="29b19-199">Herdado [do androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29b19-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="29b19-200">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="29b19-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="29b19-201">eapType</span><span class="sxs-lookup"><span data-stu-id="29b19-201">eapType</span></span>|[<span data-ttu-id="29b19-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="29b19-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="29b19-203">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="29b19-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="29b19-204">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="29b19-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="29b19-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="29b19-205">authenticationMethod</span></span>|[<span data-ttu-id="29b19-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="29b19-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="29b19-207">Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="29b19-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="29b19-208">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="29b19-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="29b19-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="29b19-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="29b19-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="29b19-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="29b19-211">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="29b19-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="29b19-212">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="29b19-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="29b19-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="29b19-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="29b19-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="29b19-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="29b19-215">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é PEAP e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="29b19-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="29b19-216">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="29b19-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="29b19-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="29b19-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="29b19-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-218">String</span></span>|<span data-ttu-id="29b19-219">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="29b19-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="29b19-220">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="29b19-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="29b19-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="29b19-221">proxySettings</span></span>|[<span data-ttu-id="29b19-222">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="29b19-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="29b19-223">Tipo de proxy para essa Wi-Fi conexão.</span><span class="sxs-lookup"><span data-stu-id="29b19-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="29b19-224">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="29b19-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="29b19-225">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="29b19-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="29b19-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b19-226">String</span></span>|<span data-ttu-id="29b19-227">URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada.</span><span class="sxs-lookup"><span data-stu-id="29b19-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="29b19-228">Normalmente, essa URL é o local do arquivo PAC (Configuração Automática de Proxy).</span><span class="sxs-lookup"><span data-stu-id="29b19-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="29b19-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b19-229">Response</span></span>
<span data-ttu-id="29b19-230">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29b19-230">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29b19-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29b19-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b19-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29b19-232">Request</span></span>
<span data-ttu-id="29b19-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29b19-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1671

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```

### <a name="response"></a><span data-ttu-id="29b19-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b19-234">Response</span></span>
<span data-ttu-id="29b19-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29b19-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1843

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```




