---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49201207237b8482aadf4ec417f1d1b7254ae212
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278482"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="474f0-103">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="474f0-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="474f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="474f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="474f0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="474f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="474f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="474f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474f0-107">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474f0-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="474f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="474f0-108">Prerequisites</span></span>
<span data-ttu-id="474f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="474f0-111">Permission type</span></span>|<span data-ttu-id="474f0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="474f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="474f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="474f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="474f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="474f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="474f0-116">Not supported.</span></span>|
|<span data-ttu-id="474f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="474f0-117">Application</span></span>|<span data-ttu-id="474f0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474f0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="474f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="474f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="474f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="474f0-120">Request headers</span></span>
|<span data-ttu-id="474f0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="474f0-121">Header</span></span>|<span data-ttu-id="474f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="474f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="474f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="474f0-123">Authorization</span></span>|<span data-ttu-id="474f0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="474f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="474f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="474f0-125">Accept</span></span>|<span data-ttu-id="474f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="474f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="474f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="474f0-127">Request body</span></span>
<span data-ttu-id="474f0-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="474f0-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="474f0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="474f0-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="474f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="474f0-130">Property</span></span>|<span data-ttu-id="474f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="474f0-131">Type</span></span>|<span data-ttu-id="474f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="474f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="474f0-133">id</span><span class="sxs-lookup"><span data-stu-id="474f0-133">id</span></span>|<span data-ttu-id="474f0-134">String</span><span class="sxs-lookup"><span data-stu-id="474f0-134">String</span></span>|<span data-ttu-id="474f0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="474f0-135">Key of the entity.</span></span> <span data-ttu-id="474f0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="474f0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-138">DateTimeOffset</span></span>|<span data-ttu-id="474f0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="474f0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="474f0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="474f0-141">roleScopeTagIds</span></span>|<span data-ttu-id="474f0-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="474f0-142">String collection</span></span>|<span data-ttu-id="474f0-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="474f0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="474f0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="474f0-145">supportsScopeTags</span></span>|<span data-ttu-id="474f0-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="474f0-146">Boolean</span></span>|<span data-ttu-id="474f0-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="474f0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="474f0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="474f0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="474f0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="474f0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="474f0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="474f0-150">This property is read-only.</span></span> <span data-ttu-id="474f0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="474f0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="474f0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="474f0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="474f0-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="474f0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="474f0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="474f0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="474f0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="474f0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="474f0-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="474f0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="474f0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="474f0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="474f0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="474f0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="474f0-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="474f0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="474f0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-164">createdDateTime</span></span>|<span data-ttu-id="474f0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-165">DateTimeOffset</span></span>|<span data-ttu-id="474f0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="474f0-166">DateTime the object was created.</span></span> <span data-ttu-id="474f0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-168">description</span><span class="sxs-lookup"><span data-stu-id="474f0-168">description</span></span>|<span data-ttu-id="474f0-169">String</span><span class="sxs-lookup"><span data-stu-id="474f0-169">String</span></span>|<span data-ttu-id="474f0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="474f0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="474f0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="474f0-172">displayName</span></span>|<span data-ttu-id="474f0-173">String</span><span class="sxs-lookup"><span data-stu-id="474f0-173">String</span></span>|<span data-ttu-id="474f0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="474f0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="474f0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-176">versão</span><span class="sxs-lookup"><span data-stu-id="474f0-176">version</span></span>|<span data-ttu-id="474f0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-177">Int32</span></span>|<span data-ttu-id="474f0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="474f0-178">Version of the device configuration.</span></span> <span data-ttu-id="474f0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="474f0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474f0-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="474f0-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="474f0-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="474f0-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="474f0-182">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="474f0-182">Delivery Optimization Mode.</span></span> <span data-ttu-id="474f0-183">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="474f0-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="474f0-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="474f0-184">prereleaseFeatures</span></span>|[<span data-ttu-id="474f0-185">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="474f0-185">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="474f0-186">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="474f0-186">The pre-release features.</span></span> <span data-ttu-id="474f0-187">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="474f0-187">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="474f0-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="474f0-188">automaticUpdateMode</span></span>|[<span data-ttu-id="474f0-189">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="474f0-189">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="474f0-190">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="474f0-190">Automatic update mode.</span></span> <span data-ttu-id="474f0-191">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="474f0-191">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="474f0-192">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="474f0-192">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="474f0-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="474f0-193">Boolean</span></span>|<span data-ttu-id="474f0-194">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="474f0-194">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="474f0-195">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="474f0-195">driversExcluded</span></span>|<span data-ttu-id="474f0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="474f0-196">Boolean</span></span>|<span data-ttu-id="474f0-197">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="474f0-197">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="474f0-198">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="474f0-198">installationSchedule</span></span>|[<span data-ttu-id="474f0-199">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="474f0-199">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="474f0-200">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="474f0-200">Installation schedule</span></span>|
|<span data-ttu-id="474f0-201">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-201">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="474f0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-202">Int32</span></span>|<span data-ttu-id="474f0-203">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="474f0-203">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="474f0-204">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-204">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="474f0-205">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-205">Int32</span></span>|<span data-ttu-id="474f0-206">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="474f0-206">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="474f0-207">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="474f0-207">qualityUpdatesPaused</span></span>|<span data-ttu-id="474f0-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="474f0-208">Boolean</span></span>|<span data-ttu-id="474f0-209">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="474f0-209">Pause Quality Updates</span></span>|
|<span data-ttu-id="474f0-210">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="474f0-210">featureUpdatesPaused</span></span>|<span data-ttu-id="474f0-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="474f0-211">Boolean</span></span>|<span data-ttu-id="474f0-212">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="474f0-212">Pause Feature Updates</span></span>|
|<span data-ttu-id="474f0-213">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-213">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="474f0-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-214">DateTimeOffset</span></span>|<span data-ttu-id="474f0-215">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="474f0-215">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="474f0-216">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-216">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="474f0-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-217">DateTimeOffset</span></span>|<span data-ttu-id="474f0-218">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="474f0-218">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="474f0-219">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="474f0-219">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="474f0-220">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="474f0-220">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="474f0-221">Determina quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="474f0-221">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="474f0-222">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="474f0-222">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="474f0-223">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="474f0-223">skipChecksBeforeRestart</span></span>|<span data-ttu-id="474f0-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="474f0-224">Boolean</span></span>|<span data-ttu-id="474f0-225">Definido como ignorar todas as verificação antes de reiniciar: nível da bateria = 40%, presença do usuário, exibição necessária, modo de apresentação, modo de tela cheia, estado de chamada telefônica, modo de jogo, etc.</span><span class="sxs-lookup"><span data-stu-id="474f0-225">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="474f0-226">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="474f0-226">updateWeeks</span></span>|[<span data-ttu-id="474f0-227">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="474f0-227">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="474f0-228">Agendou a instalação da atualização nas semanas do mês.</span><span class="sxs-lookup"><span data-stu-id="474f0-228">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="474f0-229">Os possíveis valores são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="474f0-229">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="474f0-230">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="474f0-230">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="474f0-231">Data</span><span class="sxs-lookup"><span data-stu-id="474f0-231">Date</span></span>|<span data-ttu-id="474f0-232">Atualização de qualidade pausar data de início.</span><span class="sxs-lookup"><span data-stu-id="474f0-232">Quality Updates Pause start date.</span></span> <span data-ttu-id="474f0-233">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="474f0-233">This property is read-only.</span></span>|
|<span data-ttu-id="474f0-234">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="474f0-234">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="474f0-235">Data</span><span class="sxs-lookup"><span data-stu-id="474f0-235">Date</span></span>|<span data-ttu-id="474f0-236">Atualização de recursos pausar data de início.</span><span class="sxs-lookup"><span data-stu-id="474f0-236">Feature Updates Pause start date.</span></span> <span data-ttu-id="474f0-237">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="474f0-237">This property is read-only.</span></span>|
|<span data-ttu-id="474f0-238">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-238">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="474f0-239">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-239">Int32</span></span>|<span data-ttu-id="474f0-240">O número de dias após uma atualização de recurso para a qual uma reversão é válida</span><span class="sxs-lookup"><span data-stu-id="474f0-240">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="474f0-241">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="474f0-241">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="474f0-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="474f0-242">Boolean</span></span>|<span data-ttu-id="474f0-243">Especifica se é para reverter as atualizações de qualidade no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="474f0-243">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="474f0-244">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="474f0-244">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="474f0-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="474f0-245">Boolean</span></span>|<span data-ttu-id="474f0-246">Especifica se as atualizações de recursos devem ser revertidas no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="474f0-246">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="474f0-247">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-247">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="474f0-248">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-248">DateTimeOffset</span></span>|<span data-ttu-id="474f0-249">Data de início da reversão de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="474f0-249">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="474f0-250">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="474f0-250">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="474f0-251">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474f0-251">DateTimeOffset</span></span>|<span data-ttu-id="474f0-252">Atualização de recursos data de início da reversão</span><span class="sxs-lookup"><span data-stu-id="474f0-252">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="474f0-253">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-253">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="474f0-254">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-254">Int32</span></span>|<span data-ttu-id="474f0-255">Prazo em dias antes de agendar automaticamente e executar uma reinicialização pendente fora do horário ativo, com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-255">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="474f0-256">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-256">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="474f0-257">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-257">Int32</span></span>|<span data-ttu-id="474f0-258">Número de dias durante os quais um usuário pode adiar notificações de lembrete de reinício envolvidos com um intervalo válido de 1 a 3 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-258">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="474f0-259">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-259">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="474f0-260">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-260">Int32</span></span>|<span data-ttu-id="474f0-261">Número de dias antes da transição de reinícios automáticos agendados fora do horário ativo para o reinício envolvido, o que requer que o usuário agende, com o intervalo válido de 0 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-261">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="474f0-262">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-262">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="474f0-263">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-263">Int32</span></span>|<span data-ttu-id="474f0-264">Número de dias antes que as atualizações de recursos sejam instaladas automaticamente com um intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-264">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="474f0-265">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-265">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="474f0-266">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-266">Int32</span></span>|<span data-ttu-id="474f0-267">Número de dias antes de as atualizações de qualidade serem instaladas automaticamente com um intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-267">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="474f0-268">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="474f0-268">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="474f0-269">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-269">Int32</span></span>|<span data-ttu-id="474f0-270">Número de dias após o prazo até que as reinicializações ocorram automaticamente com um intervalo válido de 0 a 7 dias</span><span class="sxs-lookup"><span data-stu-id="474f0-270">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="474f0-271">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="474f0-271">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="474f0-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="474f0-272">Boolean</span></span>|<span data-ttu-id="474f0-273">Especifica se o dispositivo deve aguardar até o prazo final para reinicialização fora do horário ativo</span><span class="sxs-lookup"><span data-stu-id="474f0-273">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="474f0-274">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="474f0-274">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="474f0-275">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="474f0-275">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="474f0-276">Especifique o método pelo qual a notificação de reinício automático necessário é ignorada.</span><span class="sxs-lookup"><span data-stu-id="474f0-276">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="474f0-277">Os valores possíveis são: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="474f0-277">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="474f0-278">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="474f0-278">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="474f0-279">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-279">Int32</span></span>|<span data-ttu-id="474f0-280">Especifique o período para notificações de lembrete de aviso de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="474f0-280">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="474f0-281">Valores com suporte: 2, 4, 8, 12 ou 24 (horas).</span><span class="sxs-lookup"><span data-stu-id="474f0-281">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="474f0-282">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="474f0-282">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="474f0-283">Int32</span><span class="sxs-lookup"><span data-stu-id="474f0-283">Int32</span></span>|<span data-ttu-id="474f0-284">Especifique o período para notificações de aviso iminentes de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="474f0-284">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="474f0-285">Valores com suporte: 15, 30 ou 60 (minutos).</span><span class="sxs-lookup"><span data-stu-id="474f0-285">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="474f0-286">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="474f0-286">userPauseAccess</span></span>|[<span data-ttu-id="474f0-287">habilitação</span><span class="sxs-lookup"><span data-stu-id="474f0-287">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="474f0-288">Especifica se o acesso do usuário final deve ser habilitado para pausar as atualizações de software.</span><span class="sxs-lookup"><span data-stu-id="474f0-288">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="474f0-289">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="474f0-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="474f0-290">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="474f0-290">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="474f0-291">habilitação</span><span class="sxs-lookup"><span data-stu-id="474f0-291">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="474f0-292">Especifica se é para desabilitar o acesso do usuário para verificar o Windows Update.</span><span class="sxs-lookup"><span data-stu-id="474f0-292">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="474f0-293">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="474f0-293">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="474f0-294">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="474f0-294">updateNotificationLevel</span></span>|[<span data-ttu-id="474f0-295">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="474f0-295">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="474f0-296">Especifica quais usuários de notificações do Windows Update são exibidos.</span><span class="sxs-lookup"><span data-stu-id="474f0-296">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="474f0-297">Os valores possíveis são: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="474f0-297">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="474f0-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="474f0-298">Response</span></span>
<span data-ttu-id="474f0-299">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="474f0-299">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="474f0-300">Exemplo</span><span class="sxs-lookup"><span data-stu-id="474f0-300">Example</span></span>

### <a name="request"></a><span data-ttu-id="474f0-301">Solicitação</span><span class="sxs-lookup"><span data-stu-id="474f0-301">Request</span></span>
<span data-ttu-id="474f0-302">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="474f0-302">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="474f0-303">Resposta</span><span class="sxs-lookup"><span data-stu-id="474f0-303">Response</span></span>
<span data-ttu-id="474f0-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="474f0-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




