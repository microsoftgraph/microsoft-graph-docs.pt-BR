---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 807a49ba69e3fa034f564bf68e5eab6678e08100
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962642"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="e6168-103">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6168-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="e6168-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6168-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6168-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6168-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6168-106">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6168-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6168-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6168-107">Prerequisites</span></span>
<span data-ttu-id="e6168-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6168-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6168-110">Permission type</span></span>|<span data-ttu-id="e6168-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6168-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6168-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6168-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6168-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6168-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6168-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6168-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6168-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6168-115">Not supported.</span></span>|
|<span data-ttu-id="e6168-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6168-116">Application</span></span>|<span data-ttu-id="e6168-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6168-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6168-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6168-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e6168-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6168-119">Request headers</span></span>
|<span data-ttu-id="e6168-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6168-120">Header</span></span>|<span data-ttu-id="e6168-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e6168-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6168-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6168-122">Authorization</span></span>|<span data-ttu-id="e6168-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6168-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6168-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6168-124">Accept</span></span>|<span data-ttu-id="e6168-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6168-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6168-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6168-126">Request body</span></span>
<span data-ttu-id="e6168-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e6168-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="e6168-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e6168-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="e6168-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6168-129">Property</span></span>|<span data-ttu-id="e6168-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6168-130">Type</span></span>|<span data-ttu-id="e6168-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6168-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6168-132">id</span><span class="sxs-lookup"><span data-stu-id="e6168-132">id</span></span>|<span data-ttu-id="e6168-133">String</span><span class="sxs-lookup"><span data-stu-id="e6168-133">String</span></span>|<span data-ttu-id="e6168-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6168-134">Key of the entity.</span></span> <span data-ttu-id="e6168-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e6168-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-137">DateTimeOffset</span></span>|<span data-ttu-id="e6168-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e6168-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e6168-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6168-140">roleScopeTagIds</span></span>|<span data-ttu-id="e6168-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e6168-141">String collection</span></span>|<span data-ttu-id="e6168-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e6168-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6168-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e6168-144">supportsScopeTags</span></span>|<span data-ttu-id="e6168-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-145">Boolean</span></span>|<span data-ttu-id="e6168-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e6168-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e6168-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e6168-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e6168-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e6168-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e6168-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6168-149">This property is read-only.</span></span> <span data-ttu-id="e6168-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-151">createdDateTime</span></span>|<span data-ttu-id="e6168-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-152">DateTimeOffset</span></span>|<span data-ttu-id="e6168-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e6168-153">DateTime the object was created.</span></span> <span data-ttu-id="e6168-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-155">descrição</span><span class="sxs-lookup"><span data-stu-id="e6168-155">description</span></span>|<span data-ttu-id="e6168-156">String</span><span class="sxs-lookup"><span data-stu-id="e6168-156">String</span></span>|<span data-ttu-id="e6168-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6168-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6168-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e6168-159">displayName</span></span>|<span data-ttu-id="e6168-160">String</span><span class="sxs-lookup"><span data-stu-id="e6168-160">String</span></span>|<span data-ttu-id="e6168-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6168-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6168-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-163">versão</span><span class="sxs-lookup"><span data-stu-id="e6168-163">version</span></span>|<span data-ttu-id="e6168-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-164">Int32</span></span>|<span data-ttu-id="e6168-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6168-165">Version of the device configuration.</span></span> <span data-ttu-id="e6168-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6168-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6168-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e6168-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="e6168-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e6168-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="e6168-169">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="e6168-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="e6168-170">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="e6168-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="e6168-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e6168-171">prereleaseFeatures</span></span>|[<span data-ttu-id="e6168-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e6168-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="e6168-173">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="e6168-173">The pre-release features.</span></span> <span data-ttu-id="e6168-174">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="e6168-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="e6168-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e6168-175">automaticUpdateMode</span></span>|[<span data-ttu-id="e6168-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e6168-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="e6168-177">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="e6168-177">Automatic update mode.</span></span> <span data-ttu-id="e6168-178">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="e6168-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="e6168-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="e6168-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="e6168-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-180">Boolean</span></span>|<span data-ttu-id="e6168-181">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="e6168-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="e6168-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="e6168-182">driversExcluded</span></span>|<span data-ttu-id="e6168-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-183">Boolean</span></span>|<span data-ttu-id="e6168-184">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="e6168-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="e6168-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="e6168-185">installationSchedule</span></span>|[<span data-ttu-id="e6168-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="e6168-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="e6168-187">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="e6168-187">Installation schedule</span></span>|
|<span data-ttu-id="e6168-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e6168-189">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-189">Int32</span></span>|<span data-ttu-id="e6168-190">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="e6168-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="e6168-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e6168-192">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-192">Int32</span></span>|<span data-ttu-id="e6168-193">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="e6168-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="e6168-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e6168-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="e6168-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-195">Boolean</span></span>|<span data-ttu-id="e6168-196">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="e6168-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="e6168-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e6168-197">featureUpdatesPaused</span></span>|<span data-ttu-id="e6168-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-198">Boolean</span></span>|<span data-ttu-id="e6168-199">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="e6168-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="e6168-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e6168-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-201">DateTimeOffset</span></span>|<span data-ttu-id="e6168-202">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="e6168-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e6168-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e6168-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-204">DateTimeOffset</span></span>|<span data-ttu-id="e6168-205">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="e6168-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e6168-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="e6168-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="e6168-207">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="e6168-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="e6168-208">Determina quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="e6168-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="e6168-209">Os valores possíveis são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="e6168-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="e6168-210">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="e6168-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="e6168-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-211">Boolean</span></span>|<span data-ttu-id="e6168-212">Definido como ignorar todas as verificação antes de reiniciar: nível da bateria = 40%, presença do usuário, exibição necessária, modo de apresentação, modo de tela cheia, estado de chamada telefônica, modo de jogo, etc.</span><span class="sxs-lookup"><span data-stu-id="e6168-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="e6168-213">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="e6168-213">updateWeeks</span></span>|[<span data-ttu-id="e6168-214">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="e6168-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="e6168-215">Agendou a instalação da atualização nas semanas do mês.</span><span class="sxs-lookup"><span data-stu-id="e6168-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="e6168-216">Os valores possíveis são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="e6168-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="e6168-217">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="e6168-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="e6168-218">Data</span><span class="sxs-lookup"><span data-stu-id="e6168-218">Date</span></span>|<span data-ttu-id="e6168-219">Atualização de qualidade paUsar data de início.</span><span class="sxs-lookup"><span data-stu-id="e6168-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="e6168-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6168-220">This property is read-only.</span></span>|
|<span data-ttu-id="e6168-221">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="e6168-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="e6168-222">Data</span><span class="sxs-lookup"><span data-stu-id="e6168-222">Date</span></span>|<span data-ttu-id="e6168-223">Atualização de recursos paUsar data de início.</span><span class="sxs-lookup"><span data-stu-id="e6168-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="e6168-224">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6168-224">This property is read-only.</span></span>|
|<span data-ttu-id="e6168-225">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="e6168-226">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-226">Int32</span></span>|<span data-ttu-id="e6168-227">O número de dias após uma atualização de recurso para a qual uma reversão é válida</span><span class="sxs-lookup"><span data-stu-id="e6168-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="e6168-228">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="e6168-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="e6168-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-229">Boolean</span></span>|<span data-ttu-id="e6168-230">Especifica se é para reverter as atualizações de qualidade no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e6168-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="e6168-231">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="e6168-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="e6168-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6168-232">Boolean</span></span>|<span data-ttu-id="e6168-233">Especifica se as atualizações de recursos devem ser revertidas no próximo check-in de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e6168-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="e6168-234">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="e6168-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-235">DateTimeOffset</span></span>|<span data-ttu-id="e6168-236">Data de início da reVersão de atualização de qualidade</span><span class="sxs-lookup"><span data-stu-id="e6168-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="e6168-237">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="e6168-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="e6168-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6168-238">DateTimeOffset</span></span>|<span data-ttu-id="e6168-239">Atualização de recursos data de início da reVersão</span><span class="sxs-lookup"><span data-stu-id="e6168-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="e6168-240">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="e6168-241">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-241">Int32</span></span>|<span data-ttu-id="e6168-242">Prazo em dias antes de agendar automaticamente e executar uma reinicialização pendente fora do horário ativo, com intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="e6168-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="e6168-243">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="e6168-244">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-244">Int32</span></span>|<span data-ttu-id="e6168-245">Número de dias durante os quais um usuário pode adiar notificações de lembrete de reInício envolvidos com um intervalo válido de 1 a 3 dias</span><span class="sxs-lookup"><span data-stu-id="e6168-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="e6168-246">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="e6168-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="e6168-247">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-247">Int32</span></span>|<span data-ttu-id="e6168-248">Número de dias antes da transição de reinícios automáticos agendados fora do horário ativo para o reinício envolvido, o que requer que o usuário agende, com o intervalo válido de 0 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="e6168-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="e6168-249">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="e6168-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="e6168-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="e6168-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="e6168-251">Especifique o método pelo qual a notificação de reinício automático necessário é ignorada.</span><span class="sxs-lookup"><span data-stu-id="e6168-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="e6168-252">Os valores possíveis são: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e6168-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="e6168-253">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="e6168-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="e6168-254">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-254">Int32</span></span>|<span data-ttu-id="e6168-255">Especifique o período para notificações de lembrete de aviso de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="e6168-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="e6168-256">Valores com suporte: 2, 4, 8, 12 ou 24 (horas).</span><span class="sxs-lookup"><span data-stu-id="e6168-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="e6168-257">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="e6168-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="e6168-258">Int32</span><span class="sxs-lookup"><span data-stu-id="e6168-258">Int32</span></span>|<span data-ttu-id="e6168-259">Especifique o período para notificações de aviso iminentes de reinício automático.</span><span class="sxs-lookup"><span data-stu-id="e6168-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="e6168-260">Valores com suporte: 15, 30 ou 60 (minutos).</span><span class="sxs-lookup"><span data-stu-id="e6168-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="e6168-261">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="e6168-261">userPauseAccess</span></span>|[<span data-ttu-id="e6168-262">habilitação</span><span class="sxs-lookup"><span data-stu-id="e6168-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e6168-263">Especifica se o acesso do usuário final deve ser habilitado para pausar as atualizações de software.</span><span class="sxs-lookup"><span data-stu-id="e6168-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="e6168-264">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e6168-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e6168-265">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="e6168-265">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="e6168-266">habilitação</span><span class="sxs-lookup"><span data-stu-id="e6168-266">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e6168-267">Especifica se é para desabilitar o acesso do usuário para verificar o Windows Update.</span><span class="sxs-lookup"><span data-stu-id="e6168-267">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="e6168-268">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e6168-268">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e6168-269">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="e6168-269">updateNotificationLevel</span></span>|[<span data-ttu-id="e6168-270">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="e6168-270">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="e6168-271">Especifica quais usuários de notificações do Windows Update são exibidos.</span><span class="sxs-lookup"><span data-stu-id="e6168-271">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="e6168-272">Os valores possíveis são: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="e6168-272">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="e6168-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6168-273">Response</span></span>
<span data-ttu-id="e6168-274">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6168-274">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6168-275">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6168-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6168-276">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6168-276">Request</span></span>
<span data-ttu-id="e6168-277">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6168-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1903

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="e6168-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6168-278">Response</span></span>
<span data-ttu-id="e6168-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6168-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2075

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```




