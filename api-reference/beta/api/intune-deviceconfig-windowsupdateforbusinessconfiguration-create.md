---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
ms.openlocfilehash: 83213279b959b927be5a6e4b99f92036c83a99b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036100"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="346ee-103">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="346ee-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="346ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="346ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="346ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="346ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="346ee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="346ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="346ee-107">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346ee-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="346ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="346ee-108">Prerequisites</span></span>
<span data-ttu-id="346ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="346ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="346ee-111">Permission type</span></span>|<span data-ttu-id="346ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="346ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="346ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="346ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="346ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="346ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="346ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="346ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="346ee-116">Not supported.</span></span>|
|<span data-ttu-id="346ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="346ee-117">Application</span></span>|<span data-ttu-id="346ee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="346ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="346ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="346ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="346ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="346ee-120">Request headers</span></span>
|<span data-ttu-id="346ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="346ee-121">Header</span></span>|<span data-ttu-id="346ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="346ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="346ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="346ee-123">Authorization</span></span>|<span data-ttu-id="346ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="346ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="346ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="346ee-125">Accept</span></span>|<span data-ttu-id="346ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="346ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="346ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="346ee-127">Request body</span></span>
<span data-ttu-id="346ee-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="346ee-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="346ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="346ee-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="346ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="346ee-130">Property</span></span>|<span data-ttu-id="346ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="346ee-131">Type</span></span>|<span data-ttu-id="346ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="346ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346ee-133">id</span><span class="sxs-lookup"><span data-stu-id="346ee-133">id</span></span>|<span data-ttu-id="346ee-134">String</span><span class="sxs-lookup"><span data-stu-id="346ee-134">String</span></span>|<span data-ttu-id="346ee-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="346ee-135">Key of the entity.</span></span> <span data-ttu-id="346ee-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="346ee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-138">DateTimeOffset</span></span>|<span data-ttu-id="346ee-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="346ee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="346ee-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="346ee-141">roleScopeTagIds</span></span>|<span data-ttu-id="346ee-142">String collection</span><span class="sxs-lookup"><span data-stu-id="346ee-142">String collection</span></span>|<span data-ttu-id="346ee-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="346ee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="346ee-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="346ee-145">supportsScopeTags</span></span>|<span data-ttu-id="346ee-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-146">Boolean</span></span>|<span data-ttu-id="346ee-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="346ee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="346ee-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="346ee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="346ee-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="346ee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="346ee-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="346ee-150">This property is read-only.</span></span> <span data-ttu-id="346ee-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-152">createdDateTime</span></span>|<span data-ttu-id="346ee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-153">DateTimeOffset</span></span>|<span data-ttu-id="346ee-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="346ee-154">DateTime the object was created.</span></span> <span data-ttu-id="346ee-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-156">description</span><span class="sxs-lookup"><span data-stu-id="346ee-156">description</span></span>|<span data-ttu-id="346ee-157">String</span><span class="sxs-lookup"><span data-stu-id="346ee-157">String</span></span>|<span data-ttu-id="346ee-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="346ee-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="346ee-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-160">displayName</span><span class="sxs-lookup"><span data-stu-id="346ee-160">displayName</span></span>|<span data-ttu-id="346ee-161">String</span><span class="sxs-lookup"><span data-stu-id="346ee-161">String</span></span>|<span data-ttu-id="346ee-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="346ee-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="346ee-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-164">version</span><span class="sxs-lookup"><span data-stu-id="346ee-164">version</span></span>|<span data-ttu-id="346ee-165">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-165">Int32</span></span>|<span data-ttu-id="346ee-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="346ee-166">Version of the device configuration.</span></span> <span data-ttu-id="346ee-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346ee-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346ee-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="346ee-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="346ee-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="346ee-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="346ee-170">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="346ee-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="346ee-171">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="346ee-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="346ee-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="346ee-172">prereleaseFeatures</span></span>|[<span data-ttu-id="346ee-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="346ee-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="346ee-174">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="346ee-174">The pre-release features.</span></span> <span data-ttu-id="346ee-175">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="346ee-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="346ee-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="346ee-176">automaticUpdateMode</span></span>|[<span data-ttu-id="346ee-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="346ee-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="346ee-178">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="346ee-178">Automatic update mode.</span></span> <span data-ttu-id="346ee-179">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="346ee-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="346ee-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="346ee-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="346ee-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-181">Boolean</span></span>|<span data-ttu-id="346ee-182">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="346ee-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="346ee-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="346ee-183">driversExcluded</span></span>|<span data-ttu-id="346ee-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-184">Boolean</span></span>|<span data-ttu-id="346ee-185">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="346ee-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="346ee-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="346ee-186">installationSchedule</span></span>|[<span data-ttu-id="346ee-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="346ee-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="346ee-188">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="346ee-188">Installation schedule</span></span>|
|<span data-ttu-id="346ee-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="346ee-190">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-190">Int32</span></span>|<span data-ttu-id="346ee-191">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="346ee-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="346ee-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="346ee-193">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-193">Int32</span></span>|<span data-ttu-id="346ee-194">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="346ee-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="346ee-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="346ee-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="346ee-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-196">Boolean</span></span>|<span data-ttu-id="346ee-197">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="346ee-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="346ee-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="346ee-198">featureUpdatesPaused</span></span>|<span data-ttu-id="346ee-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-199">Boolean</span></span>|<span data-ttu-id="346ee-200">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="346ee-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="346ee-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="346ee-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-202">DateTimeOffset</span></span>|<span data-ttu-id="346ee-203">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="346ee-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="346ee-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="346ee-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-205">DateTimeOffset</span></span>|<span data-ttu-id="346ee-206">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="346ee-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="346ee-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="346ee-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="346ee-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="346ee-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="346ee-209">Determina quais dispositivos de filial receberão suas atualizações de.</span><span class="sxs-lookup"><span data-stu-id="346ee-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="346ee-210">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="346ee-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="346ee-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="346ee-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="346ee-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-212">Boolean</span></span>|<span data-ttu-id="346ee-213">Defina ignorar a verificação de todos os antes da reinicialização: nível de bateria = 40%, a presença do usuário, exibição necessários, o modo de apresentação, o modo de tela inteira, o estado de chamada telefônica, modo jogo etc.</span><span class="sxs-lookup"><span data-stu-id="346ee-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="346ee-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="346ee-214">updateWeeks</span></span>|[<span data-ttu-id="346ee-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="346ee-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="346ee-216">Agendada a instalação da atualização as semanas do mês.</span><span class="sxs-lookup"><span data-stu-id="346ee-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="346ee-217">Os possíveis valores são: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="346ee-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="346ee-218">qualityUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-218">qualityUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="346ee-219">String</span><span class="sxs-lookup"><span data-stu-id="346ee-219">String</span></span>|<span data-ttu-id="346ee-220">Qualidade pausa de atualizações iniciar datetime</span><span class="sxs-lookup"><span data-stu-id="346ee-220">Quality Updates Pause Start datetime</span></span>|
|<span data-ttu-id="346ee-221">featureUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-221">featureUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="346ee-222">String</span><span class="sxs-lookup"><span data-stu-id="346ee-222">String</span></span>|<span data-ttu-id="346ee-223">Recurso Iniciar de pausar atualizações datetime</span><span class="sxs-lookup"><span data-stu-id="346ee-223">Feature Updates Pause Start datetime</span></span>|
|<span data-ttu-id="346ee-224">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-224">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="346ee-225">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-225">Int32</span></span>|<span data-ttu-id="346ee-226">O número de dias após uma atualização de recurso para o qual uma reversão é válida</span><span class="sxs-lookup"><span data-stu-id="346ee-226">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="346ee-227">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="346ee-227">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="346ee-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-228">Boolean</span></span>|<span data-ttu-id="346ee-229">Especifica se a reversão de atualizações de qualidade do dispositivo próximo check-in</span><span class="sxs-lookup"><span data-stu-id="346ee-229">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="346ee-230">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="346ee-230">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="346ee-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="346ee-231">Boolean</span></span>|<span data-ttu-id="346ee-232">Especifica se a reversão de atualizações de recurso no dispositivo próximo check-in</span><span class="sxs-lookup"><span data-stu-id="346ee-232">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="346ee-233">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-233">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="346ee-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-234">DateTimeOffset</span></span>|<span data-ttu-id="346ee-235">Datetime Iniciar de reversão de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="346ee-235">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="346ee-236">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="346ee-236">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="346ee-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346ee-237">DateTimeOffset</span></span>|<span data-ttu-id="346ee-238">Datetime Iniciar de reversão de atualizações do recurso</span><span class="sxs-lookup"><span data-stu-id="346ee-238">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="346ee-239">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-239">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="346ee-240">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-240">Int32</span></span>|<span data-ttu-id="346ee-241">Prazo final em dias antes de agendar automaticamente e executá-lo uma reinicialização pendente fora do horário ativo, com o intervalo válido de 2 a 30 dias</span><span class="sxs-lookup"><span data-stu-id="346ee-241">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="346ee-242">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-242">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="346ee-243">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-243">Int32</span></span>|<span data-ttu-id="346ee-244">Número de dias que um usuário pode snooze notificações de lembrete reiniciar envolvidos com válidos variam de 1 a 3 dias</span><span class="sxs-lookup"><span data-stu-id="346ee-244">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="346ee-245">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="346ee-245">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="346ee-246">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-246">Int32</span></span>|<span data-ttu-id="346ee-247">Número de dias antes da transição do automático reinicia agendada fora do horário ativo participa reiniciar, que requer que o usuário agendar, com o intervalo válido entre 0 e 30 dias</span><span class="sxs-lookup"><span data-stu-id="346ee-247">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="346ee-248">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="346ee-248">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="346ee-249">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="346ee-249">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="346ee-250">Especifique o método pelo qual a reinicialização automática necessário notificação é liberada.</span><span class="sxs-lookup"><span data-stu-id="346ee-250">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="346ee-251">Os valores possíveis são: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="346ee-251">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="346ee-252">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="346ee-252">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="346ee-253">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-253">Int32</span></span>|<span data-ttu-id="346ee-254">Especifique o período para notificações de lembrete de aviso de reinicialização automática.</span><span class="sxs-lookup"><span data-stu-id="346ee-254">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="346ee-255">Valores compatíveis: 2, 4, 8, 12 ou 24 (horas).</span><span class="sxs-lookup"><span data-stu-id="346ee-255">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="346ee-256">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="346ee-256">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="346ee-257">Int32</span><span class="sxs-lookup"><span data-stu-id="346ee-257">Int32</span></span>|<span data-ttu-id="346ee-258">Especifique o período para notificações de aviso iminente da reinicialização automática.</span><span class="sxs-lookup"><span data-stu-id="346ee-258">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="346ee-259">Suporte para valores: 15, 30 ou 60 (minutos).</span><span class="sxs-lookup"><span data-stu-id="346ee-259">Supported values: 15, 30 or 60 (minutes).</span></span>|



## <a name="response"></a><span data-ttu-id="346ee-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="346ee-260">Response</span></span>
<span data-ttu-id="346ee-261">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="346ee-261">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="346ee-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="346ee-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="346ee-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="346ee-263">Request</span></span>
<span data-ttu-id="346ee-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="346ee-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1863

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```

### <a name="response"></a><span data-ttu-id="346ee-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="346ee-265">Response</span></span>
<span data-ttu-id="346ee-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="346ee-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1971

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
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
  "scheduleImminentRestartWarningInMinutes": 7
}
```





