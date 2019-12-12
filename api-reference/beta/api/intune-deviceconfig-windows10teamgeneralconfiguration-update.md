---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 556945d1b73d852b42a7555893b7bbd1c8227cb7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947173"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="d9749-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9749-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="d9749-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9749-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9749-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9749-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9749-106">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9749-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9749-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9749-107">Prerequisites</span></span>
<span data-ttu-id="d9749-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9749-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9749-110">Permission type</span></span>|<span data-ttu-id="d9749-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9749-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9749-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9749-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9749-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9749-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9749-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9749-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9749-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9749-115">Not supported.</span></span>|
|<span data-ttu-id="d9749-116">Application</span><span class="sxs-lookup"><span data-stu-id="d9749-116">Application</span></span>|<span data-ttu-id="d9749-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9749-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9749-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9749-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d9749-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9749-119">Request headers</span></span>
|<span data-ttu-id="d9749-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9749-120">Header</span></span>|<span data-ttu-id="d9749-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9749-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9749-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9749-122">Authorization</span></span>|<span data-ttu-id="d9749-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9749-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9749-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9749-124">Accept</span></span>|<span data-ttu-id="d9749-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9749-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9749-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9749-126">Request body</span></span>
<span data-ttu-id="d9749-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9749-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="d9749-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9749-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="d9749-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9749-129">Property</span></span>|<span data-ttu-id="d9749-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9749-130">Type</span></span>|<span data-ttu-id="d9749-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9749-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9749-132">id</span><span class="sxs-lookup"><span data-stu-id="d9749-132">id</span></span>|<span data-ttu-id="d9749-133">String</span><span class="sxs-lookup"><span data-stu-id="d9749-133">String</span></span>|<span data-ttu-id="d9749-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9749-134">Key of the entity.</span></span> <span data-ttu-id="d9749-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9749-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9749-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9749-137">DateTimeOffset</span></span>|<span data-ttu-id="d9749-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d9749-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d9749-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9749-140">roleScopeTagIds</span></span>|<span data-ttu-id="d9749-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9749-141">String collection</span></span>|<span data-ttu-id="d9749-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d9749-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9749-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d9749-144">supportsScopeTags</span></span>|<span data-ttu-id="d9749-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-145">Boolean</span></span>|<span data-ttu-id="d9749-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d9749-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9749-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d9749-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9749-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d9749-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9749-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9749-149">This property is read-only.</span></span> <span data-ttu-id="d9749-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9749-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d9749-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9749-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d9749-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d9749-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d9749-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9749-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d9749-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9749-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d9749-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d9749-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d9749-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9749-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d9749-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9749-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d9749-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d9749-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d9749-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9749-163">createdDateTime</span></span>|<span data-ttu-id="d9749-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9749-164">DateTimeOffset</span></span>|<span data-ttu-id="d9749-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d9749-165">DateTime the object was created.</span></span> <span data-ttu-id="d9749-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-167">description</span><span class="sxs-lookup"><span data-stu-id="d9749-167">description</span></span>|<span data-ttu-id="d9749-168">String</span><span class="sxs-lookup"><span data-stu-id="d9749-168">String</span></span>|<span data-ttu-id="d9749-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9749-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9749-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d9749-171">displayName</span></span>|<span data-ttu-id="d9749-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9749-172">String</span></span>|<span data-ttu-id="d9749-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9749-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9749-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-175">versão</span><span class="sxs-lookup"><span data-stu-id="d9749-175">version</span></span>|<span data-ttu-id="d9749-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-176">Int32</span></span>|<span data-ttu-id="d9749-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9749-177">Version of the device configuration.</span></span> <span data-ttu-id="d9749-178">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9749-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9749-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="d9749-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="d9749-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-180">Boolean</span></span>|<span data-ttu-id="d9749-181">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d9749-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="d9749-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="d9749-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="d9749-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d9749-183">String</span></span>|<span data-ttu-id="d9749-184">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="d9749-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="d9749-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="d9749-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="d9749-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9749-186">String</span></span>|<span data-ttu-id="d9749-187">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="d9749-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="d9749-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="d9749-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="d9749-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-189">Boolean</span></span>|<span data-ttu-id="d9749-190">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="d9749-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="d9749-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="d9749-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="d9749-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-192">Boolean</span></span>|<span data-ttu-id="d9749-193">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d9749-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="d9749-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="d9749-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="d9749-195">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-195">Int32</span></span>|<span data-ttu-id="d9749-196">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9749-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="d9749-197">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="d9749-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="d9749-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="d9749-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="d9749-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d9749-199">TimeOfDay</span></span>|<span data-ttu-id="d9749-200">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9749-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="d9749-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d9749-201">miracastChannel</span></span>|[<span data-ttu-id="d9749-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d9749-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="d9749-203">O canal.</span><span class="sxs-lookup"><span data-stu-id="d9749-203">The channel.</span></span> <span data-ttu-id="d9749-204">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="d9749-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="d9749-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="d9749-205">miracastBlocked</span></span>|<span data-ttu-id="d9749-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-206">Boolean</span></span>|<span data-ttu-id="d9749-207">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d9749-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="d9749-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="d9749-208">miracastRequirePin</span></span>|<span data-ttu-id="d9749-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-209">Boolean</span></span>|<span data-ttu-id="d9749-210">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="d9749-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="d9749-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="d9749-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="d9749-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-212">Boolean</span></span>|<span data-ttu-id="d9749-213">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="d9749-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="d9749-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="d9749-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="d9749-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-215">Boolean</span></span>|<span data-ttu-id="d9749-216">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="d9749-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="d9749-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="d9749-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="d9749-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-218">Boolean</span></span>|<span data-ttu-id="d9749-219">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="d9749-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="d9749-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="d9749-220">settingsDefaultVolume</span></span>|<span data-ttu-id="d9749-221">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-221">Int32</span></span>|<span data-ttu-id="d9749-222">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="d9749-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="d9749-223">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="d9749-223">Permitted values are 0-100.</span></span> <span data-ttu-id="d9749-224">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="d9749-224">The default is 45.</span></span> <span data-ttu-id="d9749-225">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="d9749-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d9749-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d9749-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="d9749-227">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-227">Int32</span></span>|<span data-ttu-id="d9749-228">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="d9749-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="d9749-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d9749-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="d9749-230">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-230">Int32</span></span>|<span data-ttu-id="d9749-231">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d9749-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="d9749-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d9749-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="d9749-233">Int32</span><span class="sxs-lookup"><span data-stu-id="d9749-233">Int32</span></span>|<span data-ttu-id="d9749-234">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="d9749-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="d9749-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="d9749-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="d9749-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9749-236">Boolean</span></span>|<span data-ttu-id="d9749-237">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="d9749-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="d9749-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="d9749-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="d9749-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9749-239">String</span></span>|<span data-ttu-id="d9749-240">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="d9749-240">The welcome screen background image URL.</span></span> <span data-ttu-id="d9749-241">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="d9749-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="d9749-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d9749-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="d9749-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d9749-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="d9749-244">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="d9749-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="d9749-245">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="d9749-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9749-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9749-246">Response</span></span>
<span data-ttu-id="d9749-247">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9749-247">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9749-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9749-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9749-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9749-249">Request</span></span>
<span data-ttu-id="d9749-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9749-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2015

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="d9749-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9749-251">Response</span></span>
<span data-ttu-id="d9749-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9749-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2187

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```





