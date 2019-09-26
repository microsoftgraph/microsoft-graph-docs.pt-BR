---
title: Criar windows10DeviceFirmwareConfigurationInterface
description: Criar um novo objeto windows10DeviceFirmwareConfigurationInterface.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a2606c7faa1b76e04f12094e84793546db645d1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182950"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="9d36e-103">Criar windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="9d36e-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

> <span data-ttu-id="9d36e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d36e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d36e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d36e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d36e-106">Criar um novo objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="9d36e-106">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d36e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d36e-107">Prerequisites</span></span>
<span data-ttu-id="9d36e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d36e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d36e-110">Permission type</span></span>|<span data-ttu-id="9d36e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d36e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d36e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d36e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d36e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d36e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d36e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d36e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d36e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d36e-115">Not supported.</span></span>|
|<span data-ttu-id="9d36e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d36e-116">Application</span></span>|<span data-ttu-id="9d36e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d36e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d36e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d36e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9d36e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-119">Request headers</span></span>
|<span data-ttu-id="9d36e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d36e-120">Header</span></span>|<span data-ttu-id="9d36e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9d36e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d36e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d36e-122">Authorization</span></span>|<span data-ttu-id="9d36e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d36e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d36e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d36e-124">Accept</span></span>|<span data-ttu-id="9d36e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d36e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d36e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-126">Request body</span></span>
<span data-ttu-id="9d36e-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="9d36e-127">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="9d36e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="9d36e-128">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="9d36e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d36e-129">Property</span></span>|<span data-ttu-id="9d36e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d36e-130">Type</span></span>|<span data-ttu-id="9d36e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d36e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d36e-132">id</span><span class="sxs-lookup"><span data-stu-id="9d36e-132">id</span></span>|<span data-ttu-id="9d36e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d36e-133">String</span></span>|<span data-ttu-id="9d36e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d36e-134">Key of the entity.</span></span> <span data-ttu-id="9d36e-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d36e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9d36e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d36e-137">DateTimeOffset</span></span>|<span data-ttu-id="9d36e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9d36e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9d36e-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d36e-140">roleScopeTagIds</span></span>|<span data-ttu-id="9d36e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d36e-141">String collection</span></span>|<span data-ttu-id="9d36e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9d36e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9d36e-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9d36e-144">supportsScopeTags</span></span>|<span data-ttu-id="9d36e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d36e-145">Boolean</span></span>|<span data-ttu-id="9d36e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9d36e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9d36e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9d36e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9d36e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9d36e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9d36e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d36e-149">This property is read-only.</span></span> <span data-ttu-id="9d36e-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d36e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9d36e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d36e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9d36e-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9d36e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9d36e-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d36e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9d36e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d36e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9d36e-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9d36e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9d36e-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d36e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9d36e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d36e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9d36e-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9d36e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9d36e-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d36e-163">createdDateTime</span></span>|<span data-ttu-id="9d36e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d36e-164">DateTimeOffset</span></span>|<span data-ttu-id="9d36e-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9d36e-165">DateTime the object was created.</span></span> <span data-ttu-id="9d36e-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-167">descrição</span><span class="sxs-lookup"><span data-stu-id="9d36e-167">description</span></span>|<span data-ttu-id="9d36e-168">String</span><span class="sxs-lookup"><span data-stu-id="9d36e-168">String</span></span>|<span data-ttu-id="9d36e-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d36e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d36e-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9d36e-171">displayName</span></span>|<span data-ttu-id="9d36e-172">String</span><span class="sxs-lookup"><span data-stu-id="9d36e-172">String</span></span>|<span data-ttu-id="9d36e-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d36e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d36e-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-175">versão</span><span class="sxs-lookup"><span data-stu-id="9d36e-175">version</span></span>|<span data-ttu-id="9d36e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9d36e-176">Int32</span></span>|<span data-ttu-id="9d36e-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d36e-177">Version of the device configuration.</span></span> <span data-ttu-id="9d36e-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d36e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d36e-179">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="9d36e-179">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="9d36e-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="9d36e-180">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="9d36e-181">Define o nível de permissão concedido aos usuários para alterar as configurações de UEFI.</span><span class="sxs-lookup"><span data-stu-id="9d36e-181">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="9d36e-182">Os valores possíveis são: `notConfiguredOnly` e `none`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-182">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="9d36e-183">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="9d36e-183">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="9d36e-184">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-185">Define se a CPU e a virtualização de es estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="9d36e-185">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="9d36e-186">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9d36e-187">câmera</span><span class="sxs-lookup"><span data-stu-id="9d36e-187">cameras</span></span>|[<span data-ttu-id="9d36e-188">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-189">Define se as câmeras internas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="9d36e-189">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="9d36e-190">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9d36e-191">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="9d36e-191">microphonesAndSpeakers</span></span>|[<span data-ttu-id="9d36e-192">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-193">Define se microfones internos ou alto-falantes estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="9d36e-193">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="9d36e-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9d36e-195">rádios</span><span class="sxs-lookup"><span data-stu-id="9d36e-195">radios</span></span>|[<span data-ttu-id="9d36e-196">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-197">Define se os rádios internos, por exemplo, WIFI, NFC, Bluetooth, estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="9d36e-197">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="9d36e-198">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9d36e-199">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="9d36e-199">bootFromExternalMedia</span></span>|[<span data-ttu-id="9d36e-200">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-201">Define se um usuário tem permissão para inicializar a partir de mídia externa.</span><span class="sxs-lookup"><span data-stu-id="9d36e-201">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="9d36e-202">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9d36e-203">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="9d36e-203">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="9d36e-204">habilitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-204">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9d36e-205">Define se um usuário tem permissão para inicializar a partir de adaptadores de rede internos.</span><span class="sxs-lookup"><span data-stu-id="9d36e-205">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="9d36e-206">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d36e-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="9d36e-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d36e-207">Response</span></span>
<span data-ttu-id="9d36e-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d36e-208">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d36e-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d36e-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d36e-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d36e-210">Request</span></span>
<span data-ttu-id="9d36e-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d36e-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d36e-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d36e-212">Response</span></span>
<span data-ttu-id="9d36e-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d36e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




