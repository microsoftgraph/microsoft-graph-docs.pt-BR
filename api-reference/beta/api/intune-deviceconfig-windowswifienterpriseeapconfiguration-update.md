---
title: Atualizar windowsWifiEnterpriseEAPConfiguration
description: Atualizar as propriedades de um objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d092d4fd5cec9edd1ac102a935c63d9a96501808
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790717"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="ff2c6-103">Atualizar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff2c6-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="ff2c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff2c6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff2c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2c6-107">Atualizar as propriedades de um [objeto windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff2c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff2c6-108">Prerequisites</span></span>
<span data-ttu-id="ff2c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff2c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff2c6-111">Permission type</span></span>|<span data-ttu-id="ff2c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff2c6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff2c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff2c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff2c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff2c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-116">Not supported.</span></span>|
|<span data-ttu-id="ff2c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff2c6-117">Application</span></span>|<span data-ttu-id="ff2c6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff2c6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff2c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff2c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff2c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff2c6-120">Request headers</span></span>
|<span data-ttu-id="ff2c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff2c6-121">Header</span></span>|<span data-ttu-id="ff2c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff2c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff2c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff2c6-123">Authorization</span></span>|<span data-ttu-id="ff2c6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff2c6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff2c6-125">Accept</span></span>|<span data-ttu-id="ff2c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff2c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff2c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff2c6-127">Request body</span></span>
<span data-ttu-id="ff2c6-128">No corpo da solicitação, fornece uma representação JSON do [objeto windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="ff2c6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="ff2c6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff2c6-130">Property</span></span>|<span data-ttu-id="ff2c6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff2c6-131">Type</span></span>|<span data-ttu-id="ff2c6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff2c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2c6-133">id</span><span class="sxs-lookup"><span data-stu-id="ff2c6-133">id</span></span>|<span data-ttu-id="ff2c6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-134">String</span></span>|<span data-ttu-id="ff2c6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-135">Key of the entity.</span></span> <span data-ttu-id="ff2c6-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff2c6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ff2c6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff2c6-138">DateTimeOffset</span></span>|<span data-ttu-id="ff2c6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ff2c6-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff2c6-141">roleScopeTagIds</span></span>|<span data-ttu-id="ff2c6-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-142">String collection</span></span>|<span data-ttu-id="ff2c6-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff2c6-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ff2c6-145">supportsScopeTags</span></span>|<span data-ttu-id="ff2c6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-146">Boolean</span></span>|<span data-ttu-id="ff2c6-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ff2c6-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ff2c6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ff2c6-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-150">This property is read-only.</span></span> <span data-ttu-id="ff2c6-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff2c6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ff2c6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff2c6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ff2c6-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ff2c6-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff2c6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ff2c6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff2c6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ff2c6-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ff2c6-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff2c6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ff2c6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff2c6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ff2c6-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ff2c6-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff2c6-164">createdDateTime</span></span>|<span data-ttu-id="ff2c6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff2c6-165">DateTimeOffset</span></span>|<span data-ttu-id="ff2c6-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-166">DateTime the object was created.</span></span> <span data-ttu-id="ff2c6-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-168">description</span><span class="sxs-lookup"><span data-stu-id="ff2c6-168">description</span></span>|<span data-ttu-id="ff2c6-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-169">String</span></span>|<span data-ttu-id="ff2c6-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff2c6-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ff2c6-172">displayName</span></span>|<span data-ttu-id="ff2c6-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-173">String</span></span>|<span data-ttu-id="ff2c6-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff2c6-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-176">versão</span><span class="sxs-lookup"><span data-stu-id="ff2c6-176">version</span></span>|<span data-ttu-id="ff2c6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-177">Int32</span></span>|<span data-ttu-id="ff2c6-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-178">Version of the device configuration.</span></span> <span data-ttu-id="ff2c6-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ff2c6-180">preSharedKey</span></span>|<span data-ttu-id="ff2c6-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-181">String</span></span>|<span data-ttu-id="ff2c6-182">Essa é a chave pré-compartilhada para a rede WPA Personal Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="ff2c6-183">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-184">wifiSecurityType</span></span>|[<span data-ttu-id="ff2c6-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="ff2c6-186">Especifique o Tipo de Segurança Wifi.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="ff2c6-187">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="ff2c6-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="ff2c6-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="ff2c6-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="ff2c6-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="ff2c6-191">Especifique o tipo de limite de conexão limitado para a conexão wi-fi.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="ff2c6-192">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="ff2c6-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="ff2c6-194">ssid</span><span class="sxs-lookup"><span data-stu-id="ff2c6-194">ssid</span></span>|<span data-ttu-id="ff2c6-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-195">String</span></span>|<span data-ttu-id="ff2c6-196">Especifique o SSID da conexão wi-fi.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="ff2c6-197">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-198">networkName</span><span class="sxs-lookup"><span data-stu-id="ff2c6-198">networkName</span></span>|<span data-ttu-id="ff2c6-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-199">String</span></span>|<span data-ttu-id="ff2c6-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-200">Specify the network configuration name.</span></span> <span data-ttu-id="ff2c6-201">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ff2c6-202">connectAutomatically</span></span>|<span data-ttu-id="ff2c6-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-203">Boolean</span></span>|<span data-ttu-id="ff2c6-204">Especifique se a conexão wi-fi deve se conectar automaticamente quando estiver dentro do intervalo.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="ff2c6-205">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="ff2c6-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="ff2c6-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-207">Boolean</span></span>|<span data-ttu-id="ff2c6-208">Especifique se a conexão wi-fi deve se conectar a redes mais preferenciais quando já estiver conectada a esta.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="ff2c6-209">Requer ConnectAutomatically para ser true.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="ff2c6-210">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ff2c6-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ff2c6-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-212">Boolean</span></span>|<span data-ttu-id="ff2c6-213">Especifique se a conexão wi-fi deve se conectar automaticamente, mesmo quando o SSID não estiver sendo transmitido.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="ff2c6-214">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="ff2c6-215">proxySetting</span></span>|[<span data-ttu-id="ff2c6-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="ff2c6-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="ff2c6-217">Especifique a configuração de proxy Wi-Fi Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="ff2c6-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="ff2c6-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="ff2c6-219">proxyManualAddress</span></span>|<span data-ttu-id="ff2c6-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-220">String</span></span>|<span data-ttu-id="ff2c6-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="ff2c6-222">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="ff2c6-223">proxyManualPort</span></span>|<span data-ttu-id="ff2c6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-224">Int32</span></span>|<span data-ttu-id="ff2c6-225">Especifique a porta para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="ff2c6-226">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="ff2c6-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="ff2c6-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-228">String</span></span>|<span data-ttu-id="ff2c6-229">Especifique a URL para o script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="ff2c6-230">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="ff2c6-231">forceFIPSCompliance</span></span>|<span data-ttu-id="ff2c6-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-232">Boolean</span></span>|<span data-ttu-id="ff2c6-233">Especifica se é necessário forçar a conformidade FIPS.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="ff2c6-234">Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c6-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff2c6-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="ff2c6-235">networkSingleSignOn</span></span>|[<span data-ttu-id="ff2c6-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="ff2c6-237">Especifique o tipo de sinal único de rede.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-237">Specify the network single sign on type.</span></span> <span data-ttu-id="ff2c6-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="ff2c6-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="ff2c6-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="ff2c6-240">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-240">Int32</span></span>|<span data-ttu-id="ff2c6-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="ff2c6-242">Intervalo válido: 1 a 120</span><span class="sxs-lookup"><span data-stu-id="ff2c6-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="ff2c6-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="ff2c6-243">userBasedVirtualLan</span></span>|<span data-ttu-id="ff2c6-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-244">Boolean</span></span>|<span data-ttu-id="ff2c6-245">Especifica se deve alterar a LAN virtual usada pelo dispositivo com base nas credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="ff2c6-246">Não pode ser usado quando NetworkSingleSignOnType está definida como Desabilitada.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="ff2c6-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="ff2c6-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="ff2c6-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-248">Boolean</span></span>|<span data-ttu-id="ff2c6-249">Especifique se a conexão wi-fi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="ff2c6-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="ff2c6-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="ff2c6-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-251">Boolean</span></span>|<span data-ttu-id="ff2c6-252">Especifique se a conexão wi-fi deve habilitar o cache de chaves mestras pares.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="ff2c6-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="ff2c6-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="ff2c6-254">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-254">Int32</span></span>|<span data-ttu-id="ff2c6-255">Especifique o tempo máximo de cache da chave mestra em pares (em minutos).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="ff2c6-256">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="ff2c6-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="ff2c6-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="ff2c6-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="ff2c6-258">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-258">Int32</span></span>|<span data-ttu-id="ff2c6-259">Especifique o número máximo de chaves mestras pares em cache.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="ff2c6-260">Intervalo válido: 1 a 255</span><span class="sxs-lookup"><span data-stu-id="ff2c6-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="ff2c6-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="ff2c6-261">enablePreAuthentication</span></span>|<span data-ttu-id="ff2c6-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-262">Boolean</span></span>|<span data-ttu-id="ff2c6-263">Especifica se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="ff2c6-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="ff2c6-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="ff2c6-265">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-265">Int32</span></span>|<span data-ttu-id="ff2c6-266">Especifique o máximo de tentativas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="ff2c6-267">Intervalo válido: 1 a 16</span><span class="sxs-lookup"><span data-stu-id="ff2c6-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="ff2c6-268">eapType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-268">eapType</span></span>|[<span data-ttu-id="ff2c6-269">eapType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="ff2c6-270">Protocolo de autenticação extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="ff2c6-271">Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ff2c6-272">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="ff2c6-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="ff2c6-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="ff2c6-274">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-274">String collection</span></span>|<span data-ttu-id="ff2c6-275">Especifique nomes de certificados de servidor confiáveis.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="ff2c6-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff2c6-276">authenticationMethod</span></span>|[<span data-ttu-id="ff2c6-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff2c6-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ff2c6-278">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-278">Specify the authentication method.</span></span> <span data-ttu-id="ff2c6-279">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ff2c6-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="ff2c6-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="ff2c6-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ff2c6-282">Especifique o protocolo de autenticação interna para TTLS EAP.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="ff2c6-283">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ff2c6-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ff2c6-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ff2c6-285">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c6-285">String</span></span>|<span data-ttu-id="ff2c6-286">Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar TTLS EAP ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="ff2c6-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="ff2c6-287">requireCryptographicBinding</span></span>|<span data-ttu-id="ff2c6-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-288">Boolean</span></span>|<span data-ttu-id="ff2c6-289">Especifica se a associação criptográfica deve ser habilitada quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="ff2c6-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="ff2c6-290">performServerValidation</span></span>|<span data-ttu-id="ff2c6-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-291">Boolean</span></span>|<span data-ttu-id="ff2c6-292">Especifique se a verificação da identidade do servidor será habilitada validando o certificado quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="ff2c6-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="ff2c6-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="ff2c6-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-294">Boolean</span></span>|<span data-ttu-id="ff2c6-295">Especifique se deve impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="ff2c6-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="ff2c6-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="ff2c6-297">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-297">Int32</span></span>|<span data-ttu-id="ff2c6-298">Especifique o número de segundos para que o cliente aguarde após uma tentativa de autenticação antes de falhar.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="ff2c6-299">Intervalo válido de 1 a 3600.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="ff2c6-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="ff2c6-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="ff2c6-301">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-301">Int32</span></span>|<span data-ttu-id="ff2c6-302">Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="ff2c6-303">Intervalo válido de 1 a 3600.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="ff2c6-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="ff2c6-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="ff2c6-305">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-305">Int32</span></span>|<span data-ttu-id="ff2c6-306">Especifique o número de segundos de espera antes de enviar uma mensagem de início EAPOL (Extensible Authentication Protocol over LAN).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="ff2c6-307">Intervalo válido de 1 a 3600.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="ff2c6-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="ff2c6-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="ff2c6-309">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-309">Int32</span></span>|<span data-ttu-id="ff2c6-310">Especifica o número máximo de mensagens de início EAPOL (Extensible Authentication Protocol over LAN) a serem enviadas antes da falha de retorno.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="ff2c6-311">Intervalo válido de 1 a 100.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="ff2c6-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="ff2c6-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="ff2c6-313">Int32</span><span class="sxs-lookup"><span data-stu-id="ff2c6-313">Int32</span></span>|<span data-ttu-id="ff2c6-314">Especifique o máximo de falhas de autenticação permitidas para um conjunto de credenciais.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="ff2c6-315">Intervalo válido de 1 a 100.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="ff2c6-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="ff2c6-316">cacheCredentials</span></span>|<span data-ttu-id="ff2c6-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c6-317">Boolean</span></span>|<span data-ttu-id="ff2c6-318">Especifique se as credenciais do usuário devem ser armazenadas em cache no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="ff2c6-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-319">authenticationType</span></span>|[<span data-ttu-id="ff2c6-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="ff2c6-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="ff2c6-321">Especifique se o usuário, o dispositivo ou a autenticação de convidado devem ser autenticados (nenhum).</span><span class="sxs-lookup"><span data-stu-id="ff2c6-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="ff2c6-322">Se você estiver usando autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="ff2c6-323">Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="ff2c6-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff2c6-324">Response</span></span>
<span data-ttu-id="ff2c6-325">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff2c6-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff2c6-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff2c6-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff2c6-327">Request</span></span>
<span data-ttu-id="ff2c6-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2695

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a><span data-ttu-id="ff2c6-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff2c6-329">Response</span></span>
<span data-ttu-id="ff2c6-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff2c6-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2867

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




