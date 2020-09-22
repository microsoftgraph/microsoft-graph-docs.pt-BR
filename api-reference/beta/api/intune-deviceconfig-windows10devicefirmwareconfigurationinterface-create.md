---
title: Criar windows10DeviceFirmwareConfigurationInterface
description: Criar um novo objeto windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b0ee87406d77f27184364f5a7f941c57f36c38e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994768"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="bd852-103">Criar windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="bd852-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="bd852-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd852-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd852-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd852-107">Criar um novo objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="bd852-107">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd852-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd852-108">Prerequisites</span></span>
<span data-ttu-id="bd852-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd852-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd852-111">Permission type</span></span>|<span data-ttu-id="bd852-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd852-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd852-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd852-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd852-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd852-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd852-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd852-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd852-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd852-116">Not supported.</span></span>|
|<span data-ttu-id="bd852-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd852-117">Application</span></span>|<span data-ttu-id="bd852-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd852-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd852-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd852-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd852-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd852-120">Request headers</span></span>
|<span data-ttu-id="bd852-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd852-121">Header</span></span>|<span data-ttu-id="bd852-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bd852-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd852-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd852-123">Authorization</span></span>|<span data-ttu-id="bd852-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd852-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd852-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd852-125">Accept</span></span>|<span data-ttu-id="bd852-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd852-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd852-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd852-127">Request body</span></span>
<span data-ttu-id="bd852-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="bd852-128">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="bd852-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="bd852-129">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="bd852-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd852-130">Property</span></span>|<span data-ttu-id="bd852-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd852-131">Type</span></span>|<span data-ttu-id="bd852-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd852-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd852-133">id</span><span class="sxs-lookup"><span data-stu-id="bd852-133">id</span></span>|<span data-ttu-id="bd852-134">String</span><span class="sxs-lookup"><span data-stu-id="bd852-134">String</span></span>|<span data-ttu-id="bd852-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bd852-135">Key of the entity.</span></span> <span data-ttu-id="bd852-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd852-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bd852-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd852-138">DateTimeOffset</span></span>|<span data-ttu-id="bd852-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bd852-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bd852-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd852-141">roleScopeTagIds</span></span>|<span data-ttu-id="bd852-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd852-142">String collection</span></span>|<span data-ttu-id="bd852-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bd852-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd852-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bd852-145">supportsScopeTags</span></span>|<span data-ttu-id="bd852-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd852-146">Boolean</span></span>|<span data-ttu-id="bd852-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bd852-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bd852-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bd852-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bd852-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bd852-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bd852-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd852-150">This property is read-only.</span></span> <span data-ttu-id="bd852-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bd852-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bd852-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bd852-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bd852-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="bd852-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bd852-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bd852-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bd852-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bd852-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bd852-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="bd852-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bd852-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bd852-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bd852-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bd852-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bd852-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="bd852-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bd852-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd852-164">createdDateTime</span></span>|<span data-ttu-id="bd852-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd852-165">DateTimeOffset</span></span>|<span data-ttu-id="bd852-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bd852-166">DateTime the object was created.</span></span> <span data-ttu-id="bd852-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-168">description</span><span class="sxs-lookup"><span data-stu-id="bd852-168">description</span></span>|<span data-ttu-id="bd852-169">String</span><span class="sxs-lookup"><span data-stu-id="bd852-169">String</span></span>|<span data-ttu-id="bd852-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bd852-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd852-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bd852-172">displayName</span></span>|<span data-ttu-id="bd852-173">String</span><span class="sxs-lookup"><span data-stu-id="bd852-173">String</span></span>|<span data-ttu-id="bd852-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bd852-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd852-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-176">versão</span><span class="sxs-lookup"><span data-stu-id="bd852-176">version</span></span>|<span data-ttu-id="bd852-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bd852-177">Int32</span></span>|<span data-ttu-id="bd852-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bd852-178">Version of the device configuration.</span></span> <span data-ttu-id="bd852-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd852-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd852-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="bd852-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="bd852-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="bd852-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="bd852-182">Define o nível de permissão concedido aos usuários para alterar as configurações de UEFI.</span><span class="sxs-lookup"><span data-stu-id="bd852-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="bd852-183">Os valores possíveis são: `notConfiguredOnly` e `none`.</span><span class="sxs-lookup"><span data-stu-id="bd852-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="bd852-184">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="bd852-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="bd852-185">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-186">Define se a CPU e a virtualização de es estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="bd852-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="bd852-187">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd852-188">câmera</span><span class="sxs-lookup"><span data-stu-id="bd852-188">cameras</span></span>|[<span data-ttu-id="bd852-189">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-190">Define se as câmeras internas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="bd852-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="bd852-191">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd852-192">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="bd852-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="bd852-193">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-194">Define se microfones internos ou alto-falantes estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="bd852-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="bd852-195">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd852-196">rádios</span><span class="sxs-lookup"><span data-stu-id="bd852-196">radios</span></span>|[<span data-ttu-id="bd852-197">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-198">Define se os rádios internos, por exemplo, WIFI, NFC, Bluetooth, estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="bd852-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="bd852-199">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd852-200">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="bd852-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="bd852-201">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-202">Define se um usuário tem permissão para inicializar a partir de mídia externa.</span><span class="sxs-lookup"><span data-stu-id="bd852-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="bd852-203">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bd852-204">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="bd852-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="bd852-205">habilitação</span><span class="sxs-lookup"><span data-stu-id="bd852-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bd852-206">Define se um usuário tem permissão para inicializar a partir de adaptadores de rede internos.</span><span class="sxs-lookup"><span data-stu-id="bd852-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="bd852-207">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bd852-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="bd852-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd852-208">Response</span></span>
<span data-ttu-id="bd852-209">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd852-209">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd852-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd852-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd852-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd852-211">Request</span></span>
<span data-ttu-id="bd852-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd852-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1309

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="bd852-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd852-213">Response</span></span>
<span data-ttu-id="bd852-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd852-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1481

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```






