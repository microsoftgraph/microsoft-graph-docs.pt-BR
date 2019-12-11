---
title: Atualizar windowsUpdateForBusinessConfiguration
description: Atualizar as propriedades de um objeto windowsUpdateForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4aa3a5c3d81deb2d59c6a669569d0a035fef34c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946340"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="a7b2b-103">Atualizar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7b2b-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="a7b2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7b2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7b2b-106">Atualizar as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7b2b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7b2b-107">Prerequisites</span></span>
<span data-ttu-id="a7b2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7b2b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7b2b-110">Permission type</span></span>|<span data-ttu-id="a7b2b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7b2b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7b2b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7b2b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7b2b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7b2b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-115">Not supported.</span></span>|
|<span data-ttu-id="a7b2b-116">Application</span><span class="sxs-lookup"><span data-stu-id="a7b2b-116">Application</span></span>|<span data-ttu-id="a7b2b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7b2b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7b2b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7b2b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-119">Request headers</span></span>
|<span data-ttu-id="a7b2b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7b2b-120">Header</span></span>|<span data-ttu-id="a7b2b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7b2b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7b2b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7b2b-122">Authorization</span></span>|<span data-ttu-id="a7b2b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7b2b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7b2b-124">Accept</span></span>|<span data-ttu-id="a7b2b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7b2b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7b2b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-126">Request body</span></span>
<span data-ttu-id="a7b2b-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a7b2b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a7b2b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7b2b-129">Property</span></span>|<span data-ttu-id="a7b2b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7b2b-130">Type</span></span>|<span data-ttu-id="a7b2b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7b2b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b2b-132">id</span><span class="sxs-lookup"><span data-stu-id="a7b2b-132">id</span></span>|<span data-ttu-id="a7b2b-133">String</span><span class="sxs-lookup"><span data-stu-id="a7b2b-133">String</span></span>|<span data-ttu-id="a7b2b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-134">Key of the entity.</span></span> <span data-ttu-id="a7b2b-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a7b2b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-137">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a7b2b-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7b2b-140">roleScopeTagIds</span></span>|<span data-ttu-id="a7b2b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7b2b-141">String collection</span></span>|<span data-ttu-id="a7b2b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7b2b-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7b2b-144">supportsScopeTags</span></span>|<span data-ttu-id="a7b2b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-145">Boolean</span></span>|<span data-ttu-id="a7b2b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7b2b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7b2b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7b2b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-149">This property is read-only.</span></span> <span data-ttu-id="a7b2b-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a7b2b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a7b2b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a7b2b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a7b2b-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a7b2b-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a7b2b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a7b2b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a7b2b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a7b2b-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a7b2b-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a7b2b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a7b2b-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a7b2b-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-163">createdDateTime</span></span>|<span data-ttu-id="a7b2b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-164">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-165">DateTime the object was created.</span></span> <span data-ttu-id="a7b2b-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-167">description</span><span class="sxs-lookup"><span data-stu-id="a7b2b-167">description</span></span>|<span data-ttu-id="a7b2b-168">String</span><span class="sxs-lookup"><span data-stu-id="a7b2b-168">String</span></span>|<span data-ttu-id="a7b2b-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7b2b-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a7b2b-171">displayName</span></span>|<span data-ttu-id="a7b2b-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7b2b-172">String</span></span>|<span data-ttu-id="a7b2b-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7b2b-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-175">versão</span><span class="sxs-lookup"><span data-stu-id="a7b2b-175">version</span></span>|<span data-ttu-id="a7b2b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-176">Int32</span></span>|<span data-ttu-id="a7b2b-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-177">Version of the device configuration.</span></span> <span data-ttu-id="a7b2b-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b2b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b2b-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="a7b2b-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="a7b2b-181">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="a7b2b-182">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="a7b2b-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="a7b2b-183">prereleaseFeatures</span></span>|[<span data-ttu-id="a7b2b-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="a7b2b-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="a7b2b-185">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-185">The pre-release features.</span></span> <span data-ttu-id="a7b2b-186">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="a7b2b-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-187">automaticUpdateMode</span></span>|[<span data-ttu-id="a7b2b-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="a7b2b-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="a7b2b-189">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-189">Automatic update mode.</span></span> <span data-ttu-id="a7b2b-190">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="a7b2b-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="a7b2b-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="a7b2b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-192">Boolean</span></span>|<span data-ttu-id="a7b2b-193">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="a7b2b-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="a7b2b-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="a7b2b-194">driversExcluded</span></span>|<span data-ttu-id="a7b2b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-195">Boolean</span></span>|<span data-ttu-id="a7b2b-196">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="a7b2b-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="a7b2b-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="a7b2b-197">installationSchedule</span></span>|[<span data-ttu-id="a7b2b-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="a7b2b-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="a7b2b-199">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-199">Installation schedule</span></span>|
|<span data-ttu-id="a7b2b-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a7b2b-201">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-201">Int32</span></span>|<span data-ttu-id="a7b2b-202">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="a7b2b-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a7b2b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-204">Int32</span></span>|<span data-ttu-id="a7b2b-205">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="a7b2b-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a7b2b-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="a7b2b-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-207">Boolean</span></span>|<span data-ttu-id="a7b2b-208">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="a7b2b-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="a7b2b-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a7b2b-209">featureUpdatesPaused</span></span>|<span data-ttu-id="a7b2b-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-210">Boolean</span></span>|<span data-ttu-id="a7b2b-211">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="a7b2b-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="a7b2b-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a7b2b-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-213">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-214">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="a7b2b-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a7b2b-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a7b2b-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-216">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-217">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="a7b2b-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a7b2b-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="a7b2b-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="a7b2b-219">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="a7b2b-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="a7b2b-220">Determina quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="a7b2b-221">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="a7b2b-222">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="a7b2b-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="a7b2b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-223">Boolean</span></span>|<span data-ttu-id="a7b2b-224">Definido como ignorar todas as verificação antes de reiniciar: nível da bateria = 40%, presença do usuário, exibição necessária, modo de apresentação, modo de tela cheia, estado de chamada telefônica, modo de jogo, etc.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="a7b2b-225">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="a7b2b-225">updateWeeks</span></span>|[<span data-ttu-id="a7b2b-226">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="a7b2b-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="a7b2b-227">Agendou a instalação da atualização nas semanas do mês.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="a7b2b-228">Os possíveis valores são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="a7b2b-229">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="a7b2b-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="a7b2b-230">Data</span><span class="sxs-lookup"><span data-stu-id="a7b2b-230">Date</span></span>|<span data-ttu-id="a7b2b-231">Atualização de qualidade pausar data de início.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="a7b2b-232">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-232">This property is read-only.</span></span>|
|<span data-ttu-id="a7b2b-233">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="a7b2b-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="a7b2b-234">Data</span><span class="sxs-lookup"><span data-stu-id="a7b2b-234">Date</span></span>|<span data-ttu-id="a7b2b-235">Atualização de recursos pausar data de início.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="a7b2b-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-236">This property is read-only.</span></span>|
|<span data-ttu-id="a7b2b-237">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="a7b2b-238">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-238">Int32</span></span>|<span data-ttu-id="a7b2b-239">O número de dias após uma atualização de recurso para a qual uma reversão é válida</span><span class="sxs-lookup"><span data-stu-id="a7b2b-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="a7b2b-240">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="a7b2b-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="a7b2b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-241">Boolean</span></span>|<span data-ttu-id="a7b2b-242">Especifica se é para reverter as atualizações de qualidade no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a7b2b-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="a7b2b-243">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="a7b2b-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="a7b2b-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-244">Boolean</span></span>|<span data-ttu-id="a7b2b-245">Especifica se as atualizações de recursos devem ser revertidas no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a7b2b-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="a7b2b-246">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="a7b2b-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-247">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-248">Data de início da reversão de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="a7b2b-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="a7b2b-249">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2b-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="a7b2b-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2b-250">DateTimeOffset</span></span>|<span data-ttu-id="a7b2b-251">Atualização de recursos data de início da reversão</span><span class="sxs-lookup"><span data-stu-id="a7b2b-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="a7b2b-252">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="a7b2b-253">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-253">Int32</span></span>|<span data-ttu-id="a7b2b-254">Prazo em dias antes de agendar automaticamente e executar uma reinicialização pendente fora do horário ativo, com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a7b2b-255">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="a7b2b-256">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-256">Int32</span></span>|<span data-ttu-id="a7b2b-257">Número de dias durante os quais um usuário pode adiar notificações de lembrete de reinício envolvidos com um intervalo válido de 1 a 3 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="a7b2b-258">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="a7b2b-259">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-259">Int32</span></span>|<span data-ttu-id="a7b2b-260">Número de dias antes da transição de reinícios automáticos agendados fora do horário ativo para o reinício envolvido, o que requer que o usuário agende, com o intervalo válido de 0 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="a7b2b-261">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-261">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="a7b2b-262">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-262">Int32</span></span>|<span data-ttu-id="a7b2b-263">Número de dias antes que as atualizações de recursos sejam instaladas automaticamente com um intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-263">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a7b2b-264">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-264">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="a7b2b-265">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-265">Int32</span></span>|<span data-ttu-id="a7b2b-266">Número de dias antes de as atualizações de qualidade serem instaladas automaticamente com um intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-266">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a7b2b-267">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a7b2b-267">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="a7b2b-268">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-268">Int32</span></span>|<span data-ttu-id="a7b2b-269">Número de dias após o prazo até que as reinicializações ocorram automaticamente com um intervalo válido de 0 a 7 dias</span><span class="sxs-lookup"><span data-stu-id="a7b2b-269">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="a7b2b-270">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="a7b2b-270">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="a7b2b-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7b2b-271">Boolean</span></span>|<span data-ttu-id="a7b2b-272">Especifica se o dispositivo deve aguardar até o prazo final para reinicialização fora do horário ativo</span><span class="sxs-lookup"><span data-stu-id="a7b2b-272">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="a7b2b-273">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="a7b2b-273">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="a7b2b-274">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="a7b2b-274">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="a7b2b-275">Especifique o método pelo qual a notificação de reinício automático necessário é ignorada.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-275">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="a7b2b-276">Os valores possíveis são: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-276">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="a7b2b-277">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="a7b2b-277">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="a7b2b-278">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-278">Int32</span></span>|<span data-ttu-id="a7b2b-279">Especifique o período para notificações de lembrete de aviso de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-279">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="a7b2b-280">Valores com suporte: 2, 4, 8, 12 ou 24 (horas).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-280">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="a7b2b-281">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="a7b2b-281">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="a7b2b-282">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b2b-282">Int32</span></span>|<span data-ttu-id="a7b2b-283">Especifique o período para notificações de aviso iminentes de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-283">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="a7b2b-284">Valores com suporte: 15, 30 ou 60 (minutos).</span><span class="sxs-lookup"><span data-stu-id="a7b2b-284">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="a7b2b-285">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="a7b2b-285">userPauseAccess</span></span>|[<span data-ttu-id="a7b2b-286">habilitação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-286">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a7b2b-287">Especifica se o acesso do usuário final deve ser habilitado para pausar as atualizações de software.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-287">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="a7b2b-288">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a7b2b-289">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="a7b2b-289">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="a7b2b-290">habilitação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-290">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a7b2b-291">Especifica se é para desabilitar o acesso do usuário para verificar o Windows Update.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-291">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="a7b2b-292">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a7b2b-293">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="a7b2b-293">updateNotificationLevel</span></span>|[<span data-ttu-id="a7b2b-294">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="a7b2b-294">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="a7b2b-295">Especifica quais usuários de notificações do Windows Update são exibidos.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-295">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="a7b2b-296">Os valores possíveis são: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-296">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="a7b2b-297">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b2b-297">Response</span></span>
<span data-ttu-id="a7b2b-298">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-298">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7b2b-299">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7b2b-299">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7b2b-300">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b2b-300">Request</span></span>
<span data-ttu-id="a7b2b-301">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-301">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2840

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="a7b2b-302">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b2b-302">Response</span></span>
<span data-ttu-id="a7b2b-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7b2b-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3012

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```





