---
title: Atualizar windows10DeviceFirmwareConfigurationInterface
description: Atualiza as propriedades de um objeto windows10DeviceFirmwareConfigurationInterface.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ecc5c30ff2fa9b73ffb33a2d4ca3965bd89081a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533247"
---
# <a name="update-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="334d3-103">Atualizar windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="334d3-103">Update windows10DeviceFirmwareConfigurationInterface</span></span>

> <span data-ttu-id="334d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="334d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="334d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="334d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="334d3-106">Atualiza as propriedades de um objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="334d3-106">Update the properties of a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="334d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="334d3-107">Prerequisites</span></span>
<span data-ttu-id="334d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="334d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="334d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="334d3-110">Permission type</span></span>|<span data-ttu-id="334d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="334d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="334d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="334d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="334d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="334d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="334d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="334d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="334d3-115">Not supported.</span></span>|
|<span data-ttu-id="334d3-116">Application</span><span class="sxs-lookup"><span data-stu-id="334d3-116">Application</span></span>|<span data-ttu-id="334d3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334d3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="334d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="334d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="334d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="334d3-119">Request headers</span></span>
|<span data-ttu-id="334d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="334d3-120">Header</span></span>|<span data-ttu-id="334d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="334d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="334d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="334d3-122">Authorization</span></span>|<span data-ttu-id="334d3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="334d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="334d3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="334d3-124">Accept</span></span>|<span data-ttu-id="334d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="334d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="334d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="334d3-126">Request body</span></span>
<span data-ttu-id="334d3-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="334d3-127">In the request body, supply a JSON representation for the [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

<span data-ttu-id="334d3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).</span><span class="sxs-lookup"><span data-stu-id="334d3-128">The following table shows the properties that are required when you create the [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).</span></span>

|<span data-ttu-id="334d3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="334d3-129">Property</span></span>|<span data-ttu-id="334d3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="334d3-130">Type</span></span>|<span data-ttu-id="334d3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="334d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="334d3-132">id</span><span class="sxs-lookup"><span data-stu-id="334d3-132">id</span></span>|<span data-ttu-id="334d3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="334d3-133">String</span></span>|<span data-ttu-id="334d3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="334d3-134">Key of the entity.</span></span> <span data-ttu-id="334d3-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="334d3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="334d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="334d3-137">DateTimeOffset</span></span>|<span data-ttu-id="334d3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="334d3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="334d3-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="334d3-140">roleScopeTagIds</span></span>|<span data-ttu-id="334d3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="334d3-141">String collection</span></span>|<span data-ttu-id="334d3-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="334d3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="334d3-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="334d3-144">supportsScopeTags</span></span>|<span data-ttu-id="334d3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="334d3-145">Boolean</span></span>|<span data-ttu-id="334d3-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="334d3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="334d3-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="334d3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="334d3-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="334d3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="334d3-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="334d3-149">This property is read-only.</span></span> <span data-ttu-id="334d3-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="334d3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="334d3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="334d3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="334d3-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="334d3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="334d3-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="334d3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="334d3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="334d3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="334d3-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="334d3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="334d3-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="334d3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="334d3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="334d3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="334d3-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="334d3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="334d3-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="334d3-163">createdDateTime</span></span>|<span data-ttu-id="334d3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="334d3-164">DateTimeOffset</span></span>|<span data-ttu-id="334d3-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="334d3-165">DateTime the object was created.</span></span> <span data-ttu-id="334d3-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-167">description</span><span class="sxs-lookup"><span data-stu-id="334d3-167">description</span></span>|<span data-ttu-id="334d3-168">String</span><span class="sxs-lookup"><span data-stu-id="334d3-168">String</span></span>|<span data-ttu-id="334d3-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="334d3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="334d3-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="334d3-171">displayName</span></span>|<span data-ttu-id="334d3-172">String</span><span class="sxs-lookup"><span data-stu-id="334d3-172">String</span></span>|<span data-ttu-id="334d3-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="334d3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="334d3-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-175">versão</span><span class="sxs-lookup"><span data-stu-id="334d3-175">version</span></span>|<span data-ttu-id="334d3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="334d3-176">Int32</span></span>|<span data-ttu-id="334d3-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="334d3-177">Version of the device configuration.</span></span> <span data-ttu-id="334d3-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="334d3-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="334d3-179">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="334d3-179">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="334d3-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="334d3-180">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="334d3-181">Define o nível de permissão concedido aos usuários para alterar as configurações de UEFI.</span><span class="sxs-lookup"><span data-stu-id="334d3-181">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="334d3-182">Os valores possíveis são: `notConfiguredOnly` e `none`.</span><span class="sxs-lookup"><span data-stu-id="334d3-182">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="334d3-183">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="334d3-183">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="334d3-184">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-185">Define se a CPU e a virtualização de es estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="334d3-185">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="334d3-186">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="334d3-187">câmera</span><span class="sxs-lookup"><span data-stu-id="334d3-187">cameras</span></span>|[<span data-ttu-id="334d3-188">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-189">Define se as câmeras internas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="334d3-189">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="334d3-190">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="334d3-191">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="334d3-191">microphonesAndSpeakers</span></span>|[<span data-ttu-id="334d3-192">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-193">Define se microfones internos ou alto-falantes estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="334d3-193">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="334d3-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="334d3-195">rádios</span><span class="sxs-lookup"><span data-stu-id="334d3-195">radios</span></span>|[<span data-ttu-id="334d3-196">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-197">Define se os rádios internos, por exemplo, WIFI, NFC, Bluetooth, estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="334d3-197">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="334d3-198">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="334d3-199">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="334d3-199">bootFromExternalMedia</span></span>|[<span data-ttu-id="334d3-200">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-201">Define se um usuário tem permissão para inicializar a partir de mídia externa.</span><span class="sxs-lookup"><span data-stu-id="334d3-201">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="334d3-202">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="334d3-203">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="334d3-203">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="334d3-204">habilitação</span><span class="sxs-lookup"><span data-stu-id="334d3-204">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="334d3-205">Define se um usuário tem permissão para inicializar a partir de adaptadores de rede internos.</span><span class="sxs-lookup"><span data-stu-id="334d3-205">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="334d3-206">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="334d3-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="334d3-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="334d3-207">Response</span></span>
<span data-ttu-id="334d3-208">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="334d3-208">If successful, this method returns a `200 OK` response code and an updated [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="334d3-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="334d3-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="334d3-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="334d3-210">Request</span></span>
<span data-ttu-id="334d3-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="334d3-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="334d3-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="334d3-212">Response</span></span>
<span data-ttu-id="334d3-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="334d3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






