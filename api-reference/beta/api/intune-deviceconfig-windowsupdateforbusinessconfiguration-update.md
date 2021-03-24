---
title: Atualizar windowsUpdateForBusinessConfiguration
description: Atualizar as propriedades de um objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf6816b8aa6a79a7f4b2b6f1a56f91a4ef319de1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127218"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="03e7a-103">Atualizar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="03e7a-103">Update windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="03e7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03e7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03e7a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03e7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03e7a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03e7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e7a-107">Atualizar as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e7a-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03e7a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03e7a-108">Prerequisites</span></span>
<span data-ttu-id="03e7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e7a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03e7a-111">Permission type</span></span>|<span data-ttu-id="03e7a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03e7a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03e7a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03e7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03e7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03e7a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03e7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03e7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e7a-116">Not supported.</span></span>|
|<span data-ttu-id="03e7a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03e7a-117">Application</span></span>|<span data-ttu-id="03e7a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e7a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03e7a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03e7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03e7a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03e7a-120">Request headers</span></span>
|<span data-ttu-id="03e7a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03e7a-121">Header</span></span>|<span data-ttu-id="03e7a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03e7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03e7a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03e7a-123">Authorization</span></span>|<span data-ttu-id="03e7a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03e7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03e7a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03e7a-125">Accept</span></span>|<span data-ttu-id="03e7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03e7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03e7a-127">Request body</span></span>
<span data-ttu-id="03e7a-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e7a-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="03e7a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e7a-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="03e7a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03e7a-130">Property</span></span>|<span data-ttu-id="03e7a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e7a-131">Type</span></span>|<span data-ttu-id="03e7a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e7a-133">id</span><span class="sxs-lookup"><span data-stu-id="03e7a-133">id</span></span>|<span data-ttu-id="03e7a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e7a-134">String</span></span>|<span data-ttu-id="03e7a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03e7a-135">Key of the entity.</span></span> <span data-ttu-id="03e7a-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03e7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-138">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03e7a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03e7a-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03e7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="03e7a-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e7a-142">String collection</span></span>|<span data-ttu-id="03e7a-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="03e7a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03e7a-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03e7a-145">supportsScopeTags</span></span>|<span data-ttu-id="03e7a-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="03e7a-146">Boolean</span></span>|<span data-ttu-id="03e7a-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="03e7a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03e7a-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="03e7a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03e7a-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="03e7a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03e7a-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03e7a-150">This property is read-only.</span></span> <span data-ttu-id="03e7a-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03e7a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="03e7a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03e7a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="03e7a-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="03e7a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="03e7a-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03e7a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="03e7a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03e7a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="03e7a-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="03e7a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="03e7a-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="03e7a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="03e7a-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="03e7a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="03e7a-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-164">createdDateTime</span></span>|<span data-ttu-id="03e7a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-165">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03e7a-166">DateTime the object was created.</span></span> <span data-ttu-id="03e7a-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-168">descrição</span><span class="sxs-lookup"><span data-stu-id="03e7a-168">description</span></span>|<span data-ttu-id="03e7a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e7a-169">String</span></span>|<span data-ttu-id="03e7a-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e7a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03e7a-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="03e7a-172">displayName</span></span>|<span data-ttu-id="03e7a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e7a-173">String</span></span>|<span data-ttu-id="03e7a-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e7a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03e7a-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-176">versão</span><span class="sxs-lookup"><span data-stu-id="03e7a-176">version</span></span>|<span data-ttu-id="03e7a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-177">Int32</span></span>|<span data-ttu-id="03e7a-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e7a-178">Version of the device configuration.</span></span> <span data-ttu-id="03e7a-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e7a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e7a-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="03e7a-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="03e7a-182">Modo de Otimização de Entrega.</span><span class="sxs-lookup"><span data-stu-id="03e7a-182">Delivery Optimization Mode.</span></span> <span data-ttu-id="03e7a-183">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="03e7a-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="03e7a-184">prereleaseFeatures</span></span>|[<span data-ttu-id="03e7a-185">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="03e7a-185">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="03e7a-186">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="03e7a-186">The pre-release features.</span></span> <span data-ttu-id="03e7a-187">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-187">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="03e7a-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-188">automaticUpdateMode</span></span>|[<span data-ttu-id="03e7a-189">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="03e7a-189">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="03e7a-190">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="03e7a-190">Automatic update mode.</span></span> <span data-ttu-id="03e7a-191">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-191">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="03e7a-192">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="03e7a-192">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="03e7a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e7a-193">Boolean</span></span>|<span data-ttu-id="03e7a-194">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="03e7a-194">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="03e7a-195">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="03e7a-195">driversExcluded</span></span>|<span data-ttu-id="03e7a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e7a-196">Boolean</span></span>|<span data-ttu-id="03e7a-197">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="03e7a-197">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="03e7a-198">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="03e7a-198">installationSchedule</span></span>|[<span data-ttu-id="03e7a-199">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="03e7a-199">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="03e7a-200">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="03e7a-200">Installation schedule</span></span>|
|<span data-ttu-id="03e7a-201">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-201">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="03e7a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-202">Int32</span></span>|<span data-ttu-id="03e7a-203">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-203">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="03e7a-204">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-204">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="03e7a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-205">Int32</span></span>|<span data-ttu-id="03e7a-206">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-206">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="03e7a-207">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="03e7a-207">qualityUpdatesPaused</span></span>|<span data-ttu-id="03e7a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e7a-208">Boolean</span></span>|<span data-ttu-id="03e7a-209">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="03e7a-209">Pause Quality Updates</span></span>|
|<span data-ttu-id="03e7a-210">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="03e7a-210">featureUpdatesPaused</span></span>|<span data-ttu-id="03e7a-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e7a-211">Boolean</span></span>|<span data-ttu-id="03e7a-212">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="03e7a-212">Pause Feature Updates</span></span>|
|<span data-ttu-id="03e7a-213">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-213">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="03e7a-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-214">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-215">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="03e7a-215">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="03e7a-216">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-216">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="03e7a-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-217">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-218">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="03e7a-218">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="03e7a-219">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="03e7a-219">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="03e7a-220">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="03e7a-220">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="03e7a-221">Determina de quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="03e7a-221">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="03e7a-222">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-222">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="03e7a-223">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="03e7a-223">skipChecksBeforeRestart</span></span>|<span data-ttu-id="03e7a-224">Booleano</span><span class="sxs-lookup"><span data-stu-id="03e7a-224">Boolean</span></span>|<span data-ttu-id="03e7a-225">Desmarcar todas as verificações antes da reinicialização: Nível da bateria = 40%, Presença do usuário, Exibição Necessária, Modo de Apresentação, modo de tela inteira, estado de chamada telefônica, modo de jogo etc.</span><span class="sxs-lookup"><span data-stu-id="03e7a-225">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="03e7a-226">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="03e7a-226">updateWeeks</span></span>|[<span data-ttu-id="03e7a-227">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="03e7a-227">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="03e7a-228">Agendou a instalação da atualização nas semanas do mês.</span><span class="sxs-lookup"><span data-stu-id="03e7a-228">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="03e7a-229">Os possíveis valores são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-229">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="03e7a-230">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="03e7a-230">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="03e7a-231">Data</span><span class="sxs-lookup"><span data-stu-id="03e7a-231">Date</span></span>|<span data-ttu-id="03e7a-232">Atualizações de qualidade Pausar a data de início.</span><span class="sxs-lookup"><span data-stu-id="03e7a-232">Quality Updates Pause start date.</span></span> <span data-ttu-id="03e7a-233">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03e7a-233">This property is read-only.</span></span>|
|<span data-ttu-id="03e7a-234">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="03e7a-234">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="03e7a-235">Data</span><span class="sxs-lookup"><span data-stu-id="03e7a-235">Date</span></span>|<span data-ttu-id="03e7a-236">Atualizações de recursos Pausar a data de início.</span><span class="sxs-lookup"><span data-stu-id="03e7a-236">Feature Updates Pause start date.</span></span> <span data-ttu-id="03e7a-237">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03e7a-237">This property is read-only.</span></span>|
|<span data-ttu-id="03e7a-238">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-238">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="03e7a-239">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-239">Int32</span></span>|<span data-ttu-id="03e7a-240">O número de dias após uma Atualização de Recursos para a qual uma reação é válida</span><span class="sxs-lookup"><span data-stu-id="03e7a-240">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="03e7a-241">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="03e7a-241">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="03e7a-242">Booleano</span><span class="sxs-lookup"><span data-stu-id="03e7a-242">Boolean</span></span>|<span data-ttu-id="03e7a-243">Especifica se as Atualizações de Qualidade de rebaixamento no próximo dispositivo de check-in</span><span class="sxs-lookup"><span data-stu-id="03e7a-243">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="03e7a-244">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="03e7a-244">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="03e7a-245">Booleano</span><span class="sxs-lookup"><span data-stu-id="03e7a-245">Boolean</span></span>|<span data-ttu-id="03e7a-246">Especifica se as Atualizações de Recursos de rebaixamento no próximo dispositivo de check-in</span><span class="sxs-lookup"><span data-stu-id="03e7a-246">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="03e7a-247">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-247">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="03e7a-248">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-248">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-249">Data de início das atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="03e7a-249">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="03e7a-250">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="03e7a-250">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="03e7a-251">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e7a-251">DateTimeOffset</span></span>|<span data-ttu-id="03e7a-252">Data de início das atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="03e7a-252">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="03e7a-253">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-253">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="03e7a-254">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-254">Int32</span></span>|<span data-ttu-id="03e7a-255">Prazo em dias antes de agendar automaticamente e executar uma reinicialização pendente fora do horário ativo, com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-255">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="03e7a-256">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-256">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="03e7a-257">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-257">Int32</span></span>|<span data-ttu-id="03e7a-258">Número de dias em que um usuário pode esnocar notificações de lembrete de Reinicialização Comprometida com intervalo válido de 1 a 3 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-258">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="03e7a-259">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-259">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="03e7a-260">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-260">Int32</span></span>|<span data-ttu-id="03e7a-261">Número de dias antes da transição de Reinicializações Automáticas agendadas fora do horário ativo para Reinicialização Ativa, o que exige que o usuário agende, com intervalo válido de 0 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-261">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="03e7a-262">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-262">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="03e7a-263">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-263">Int32</span></span>|<span data-ttu-id="03e7a-264">Número de dias antes que as atualizações de recursos sejam instaladas automaticamente com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-264">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="03e7a-265">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-265">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="03e7a-266">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-266">Int32</span></span>|<span data-ttu-id="03e7a-267">Número de dias antes que as atualizações de qualidade sejam instaladas automaticamente com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-267">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="03e7a-268">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="03e7a-268">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="03e7a-269">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-269">Int32</span></span>|<span data-ttu-id="03e7a-270">Número de dias após o prazo até que as reinicializações ocorram automaticamente com intervalo válido de 0 a 7 dias</span><span class="sxs-lookup"><span data-stu-id="03e7a-270">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="03e7a-271">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="03e7a-271">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="03e7a-272">Booleano</span><span class="sxs-lookup"><span data-stu-id="03e7a-272">Boolean</span></span>|<span data-ttu-id="03e7a-273">Especifica se o dispositivo deve esperar até o prazo final para reiniciar fora do horário ativo</span><span class="sxs-lookup"><span data-stu-id="03e7a-273">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="03e7a-274">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="03e7a-274">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="03e7a-275">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="03e7a-275">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="03e7a-276">Especifique o método pelo qual a notificação necessária de reinicialização automática é descartada.</span><span class="sxs-lookup"><span data-stu-id="03e7a-276">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="03e7a-277">Os valores possíveis são: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-277">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="03e7a-278">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="03e7a-278">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="03e7a-279">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-279">Int32</span></span>|<span data-ttu-id="03e7a-280">Especifique o período para notificações de lembrete de aviso de reinicialização automática.</span><span class="sxs-lookup"><span data-stu-id="03e7a-280">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="03e7a-281">Valores suportados: 2, 4, 8, 12 ou 24 (horas).</span><span class="sxs-lookup"><span data-stu-id="03e7a-281">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="03e7a-282">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="03e7a-282">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="03e7a-283">Int32</span><span class="sxs-lookup"><span data-stu-id="03e7a-283">Int32</span></span>|<span data-ttu-id="03e7a-284">Especifique o período para notificações de aviso iminente de reinicialização automática.</span><span class="sxs-lookup"><span data-stu-id="03e7a-284">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="03e7a-285">Valores suportados: 15, 30 ou 60 (minutos).</span><span class="sxs-lookup"><span data-stu-id="03e7a-285">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="03e7a-286">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="03e7a-286">userPauseAccess</span></span>|[<span data-ttu-id="03e7a-287">enablement</span><span class="sxs-lookup"><span data-stu-id="03e7a-287">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="03e7a-288">Especifica se é possível habilitar o acesso do usuário final a pausar atualizações de software.</span><span class="sxs-lookup"><span data-stu-id="03e7a-288">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="03e7a-289">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="03e7a-290">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="03e7a-290">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="03e7a-291">enablement</span><span class="sxs-lookup"><span data-stu-id="03e7a-291">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="03e7a-292">Especifica se o acesso do usuário deve ser desabilitado para verificar o Windows Update.</span><span class="sxs-lookup"><span data-stu-id="03e7a-292">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="03e7a-293">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-293">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="03e7a-294">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="03e7a-294">updateNotificationLevel</span></span>|[<span data-ttu-id="03e7a-295">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="03e7a-295">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="03e7a-296">Especifica o que os usuários de notificações do Windows Update veem.</span><span class="sxs-lookup"><span data-stu-id="03e7a-296">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="03e7a-297">Os valores possíveis são: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="03e7a-297">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="03e7a-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e7a-298">Response</span></span>
<span data-ttu-id="03e7a-299">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e7a-299">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e7a-300">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03e7a-300">Example</span></span>

### <a name="request"></a><span data-ttu-id="03e7a-301">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03e7a-301">Request</span></span>
<span data-ttu-id="03e7a-302">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03e7a-302">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2794

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
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
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

### <a name="response"></a><span data-ttu-id="03e7a-303">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e7a-303">Response</span></span>
<span data-ttu-id="03e7a-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03e7a-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2966

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
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
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




