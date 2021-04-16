---
title: Criar windows10DeviceFirmwareConfigurationInterface
description: Crie um novo objeto windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0ce46b7ca60529859fc23516bf64db8a1a36191
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866437"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="12c8c-103">Criar windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="12c8c-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="12c8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12c8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12c8c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12c8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12c8c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12c8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12c8c-107">Crie um novo [objeto windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-107">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12c8c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12c8c-108">Prerequisites</span></span>
<span data-ttu-id="12c8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12c8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c8c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12c8c-111">Permission type</span></span>|<span data-ttu-id="12c8c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12c8c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c8c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12c8c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12c8c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c8c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12c8c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12c8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c8c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12c8c-116">Not supported.</span></span>|
|<span data-ttu-id="12c8c-117">Application</span><span class="sxs-lookup"><span data-stu-id="12c8c-117">Application</span></span>|<span data-ttu-id="12c8c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c8c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c8c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12c8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12c8c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12c8c-120">Request headers</span></span>
|<span data-ttu-id="12c8c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12c8c-121">Header</span></span>|<span data-ttu-id="12c8c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12c8c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c8c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12c8c-123">Authorization</span></span>|<span data-ttu-id="12c8c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12c8c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c8c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12c8c-125">Accept</span></span>|<span data-ttu-id="12c8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12c8c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c8c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12c8c-127">Request body</span></span>
<span data-ttu-id="12c8c-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="12c8c-128">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="12c8c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="12c8c-129">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="12c8c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12c8c-130">Property</span></span>|<span data-ttu-id="12c8c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12c8c-131">Type</span></span>|<span data-ttu-id="12c8c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12c8c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c8c-133">id</span><span class="sxs-lookup"><span data-stu-id="12c8c-133">id</span></span>|<span data-ttu-id="12c8c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c8c-134">String</span></span>|<span data-ttu-id="12c8c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12c8c-135">Key of the entity.</span></span> <span data-ttu-id="12c8c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12c8c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="12c8c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c8c-138">DateTimeOffset</span></span>|<span data-ttu-id="12c8c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="12c8c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="12c8c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12c8c-141">roleScopeTagIds</span></span>|<span data-ttu-id="12c8c-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="12c8c-142">String collection</span></span>|<span data-ttu-id="12c8c-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="12c8c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12c8c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="12c8c-145">supportsScopeTags</span></span>|<span data-ttu-id="12c8c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="12c8c-146">Boolean</span></span>|<span data-ttu-id="12c8c-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12c8c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12c8c-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="12c8c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12c8c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12c8c-150">This property is read-only.</span></span> <span data-ttu-id="12c8c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12c8c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12c8c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12c8c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12c8c-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="12c8c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12c8c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12c8c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12c8c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12c8c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12c8c-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="12c8c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12c8c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12c8c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12c8c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12c8c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12c8c-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="12c8c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12c8c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12c8c-164">createdDateTime</span></span>|<span data-ttu-id="12c8c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c8c-165">DateTimeOffset</span></span>|<span data-ttu-id="12c8c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="12c8c-166">DateTime the object was created.</span></span> <span data-ttu-id="12c8c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-168">description</span><span class="sxs-lookup"><span data-stu-id="12c8c-168">description</span></span>|<span data-ttu-id="12c8c-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c8c-169">String</span></span>|<span data-ttu-id="12c8c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12c8c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="12c8c-172">displayName</span></span>|<span data-ttu-id="12c8c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c8c-173">String</span></span>|<span data-ttu-id="12c8c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12c8c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-176">versão</span><span class="sxs-lookup"><span data-stu-id="12c8c-176">version</span></span>|<span data-ttu-id="12c8c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="12c8c-177">Int32</span></span>|<span data-ttu-id="12c8c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-178">Version of the device configuration.</span></span> <span data-ttu-id="12c8c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12c8c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12c8c-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="12c8c-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="12c8c-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="12c8c-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="12c8c-182">Define o nível de permissão concedido aos usuários para alterar as configurações da UEFI.</span><span class="sxs-lookup"><span data-stu-id="12c8c-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="12c8c-183">Os valores possíveis são: `notConfiguredOnly` e `none`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="12c8c-184">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="12c8c-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="12c8c-185">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-186">Define se a virtualização de CPU e E/S está habilitada.</span><span class="sxs-lookup"><span data-stu-id="12c8c-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="12c8c-187">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-188">cameras</span><span class="sxs-lookup"><span data-stu-id="12c8c-188">cameras</span></span>|[<span data-ttu-id="12c8c-189">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-190">Define se as câmeras instaladas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="12c8c-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="12c8c-191">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-192">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="12c8c-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="12c8c-193">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-194">Define se microfones ou alto-falantes integrados estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="12c8c-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="12c8c-195">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-196">rádios</span><span class="sxs-lookup"><span data-stu-id="12c8c-196">radios</span></span>|[<span data-ttu-id="12c8c-197">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-198">Define se os rádios integrados, por exemplo, WIFI, NFC, Bluetooth, estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="12c8c-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="12c8c-199">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-200">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="12c8c-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="12c8c-201">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-202">Define se um usuário tem permissão para inicializar a partir de mídia externa.</span><span class="sxs-lookup"><span data-stu-id="12c8c-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="12c8c-203">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-204">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="12c8c-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="12c8c-205">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-206">Define se um usuário tem permissão para inicializar a partir de adaptadores de rede integrados.</span><span class="sxs-lookup"><span data-stu-id="12c8c-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="12c8c-207">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-208">windowsPlatformBinaryTable</span><span class="sxs-lookup"><span data-stu-id="12c8c-208">windowsPlatformBinaryTable</span></span>|[<span data-ttu-id="12c8c-209">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-209">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-210">Define se um usuário tem permissão para habilitar a Tabela Binária da Plataforma windows.</span><span class="sxs-lookup"><span data-stu-id="12c8c-210">Defines whether a user is allowed to enable Windows Platform Binary Table.</span></span> <span data-ttu-id="12c8c-211">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-211">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="12c8c-212">simultaneousMultiThreading</span><span class="sxs-lookup"><span data-stu-id="12c8c-212">simultaneousMultiThreading</span></span>|[<span data-ttu-id="12c8c-213">enablement</span><span class="sxs-lookup"><span data-stu-id="12c8c-213">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="12c8c-214">Define se um usuário tem permissão para habilitar MultiThreading Simultâneo.</span><span class="sxs-lookup"><span data-stu-id="12c8c-214">Defines whether a user is allowed to enable Simultaneous MultiThreading.</span></span> <span data-ttu-id="12c8c-215">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="12c8c-215">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="12c8c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c8c-216">Response</span></span>
<span data-ttu-id="12c8c-217">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12c8c-217">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c8c-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12c8c-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="12c8c-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12c8c-219">Request</span></span>
<span data-ttu-id="12c8c-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12c8c-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1397

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
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="12c8c-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c8c-221">Response</span></span>
<span data-ttu-id="12c8c-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12c8c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1569

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
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled"
}
```




