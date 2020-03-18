---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d1fd44a5d247610529abfa977d8bacdbfcf51cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42737916"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="1746a-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="1746a-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="1746a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1746a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1746a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1746a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1746a-106">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1746a-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1746a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1746a-107">Prerequisites</span></span>
<span data-ttu-id="1746a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1746a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1746a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1746a-110">Permission type</span></span>|<span data-ttu-id="1746a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1746a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1746a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1746a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1746a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1746a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1746a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1746a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1746a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1746a-115">Not supported.</span></span>|
|<span data-ttu-id="1746a-116">Application</span><span class="sxs-lookup"><span data-stu-id="1746a-116">Application</span></span>|<span data-ttu-id="1746a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1746a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1746a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1746a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1746a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1746a-119">Request headers</span></span>
|<span data-ttu-id="1746a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1746a-120">Header</span></span>|<span data-ttu-id="1746a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1746a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1746a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1746a-122">Authorization</span></span>|<span data-ttu-id="1746a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1746a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1746a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1746a-124">Accept</span></span>|<span data-ttu-id="1746a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1746a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1746a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1746a-126">Request body</span></span>
<span data-ttu-id="1746a-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1746a-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="1746a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1746a-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="1746a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1746a-129">Property</span></span>|<span data-ttu-id="1746a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1746a-130">Type</span></span>|<span data-ttu-id="1746a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1746a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1746a-132">id</span><span class="sxs-lookup"><span data-stu-id="1746a-132">id</span></span>|<span data-ttu-id="1746a-133">String</span><span class="sxs-lookup"><span data-stu-id="1746a-133">String</span></span>|<span data-ttu-id="1746a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1746a-134">Key of the entity.</span></span> <span data-ttu-id="1746a-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1746a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1746a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1746a-137">DateTimeOffset</span></span>|<span data-ttu-id="1746a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1746a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1746a-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1746a-140">roleScopeTagIds</span></span>|<span data-ttu-id="1746a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1746a-141">String collection</span></span>|<span data-ttu-id="1746a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1746a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1746a-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1746a-144">supportsScopeTags</span></span>|<span data-ttu-id="1746a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-145">Boolean</span></span>|<span data-ttu-id="1746a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1746a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1746a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1746a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1746a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1746a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1746a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1746a-149">This property is read-only.</span></span> <span data-ttu-id="1746a-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1746a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1746a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1746a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1746a-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="1746a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1746a-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1746a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1746a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1746a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1746a-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="1746a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1746a-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1746a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1746a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1746a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1746a-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="1746a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1746a-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1746a-163">createdDateTime</span></span>|<span data-ttu-id="1746a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1746a-164">DateTimeOffset</span></span>|<span data-ttu-id="1746a-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1746a-165">DateTime the object was created.</span></span> <span data-ttu-id="1746a-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-167">description</span><span class="sxs-lookup"><span data-stu-id="1746a-167">description</span></span>|<span data-ttu-id="1746a-168">String</span><span class="sxs-lookup"><span data-stu-id="1746a-168">String</span></span>|<span data-ttu-id="1746a-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1746a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1746a-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1746a-171">displayName</span></span>|<span data-ttu-id="1746a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1746a-172">String</span></span>|<span data-ttu-id="1746a-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1746a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1746a-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-175">versão</span><span class="sxs-lookup"><span data-stu-id="1746a-175">version</span></span>|<span data-ttu-id="1746a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-176">Int32</span></span>|<span data-ttu-id="1746a-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1746a-177">Version of the device configuration.</span></span> <span data-ttu-id="1746a-178">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1746a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1746a-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="1746a-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="1746a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-180">Boolean</span></span>|<span data-ttu-id="1746a-181">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1746a-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="1746a-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="1746a-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="1746a-183">String</span><span class="sxs-lookup"><span data-stu-id="1746a-183">String</span></span>|<span data-ttu-id="1746a-184">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="1746a-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="1746a-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="1746a-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="1746a-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1746a-186">String</span></span>|<span data-ttu-id="1746a-187">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="1746a-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="1746a-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="1746a-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="1746a-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-189">Boolean</span></span>|<span data-ttu-id="1746a-190">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="1746a-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="1746a-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="1746a-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="1746a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-192">Boolean</span></span>|<span data-ttu-id="1746a-193">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1746a-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="1746a-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="1746a-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="1746a-195">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-195">Int32</span></span>|<span data-ttu-id="1746a-196">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1746a-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="1746a-197">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="1746a-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="1746a-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="1746a-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="1746a-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1746a-199">TimeOfDay</span></span>|<span data-ttu-id="1746a-200">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1746a-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="1746a-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="1746a-201">miracastChannel</span></span>|[<span data-ttu-id="1746a-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="1746a-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="1746a-203">O canal.</span><span class="sxs-lookup"><span data-stu-id="1746a-203">The channel.</span></span> <span data-ttu-id="1746a-204">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="1746a-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="1746a-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="1746a-205">miracastBlocked</span></span>|<span data-ttu-id="1746a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-206">Boolean</span></span>|<span data-ttu-id="1746a-207">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1746a-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="1746a-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="1746a-208">miracastRequirePin</span></span>|<span data-ttu-id="1746a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-209">Boolean</span></span>|<span data-ttu-id="1746a-210">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="1746a-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="1746a-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="1746a-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="1746a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-212">Boolean</span></span>|<span data-ttu-id="1746a-213">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="1746a-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="1746a-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="1746a-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="1746a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-215">Boolean</span></span>|<span data-ttu-id="1746a-216">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="1746a-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="1746a-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="1746a-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="1746a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-218">Boolean</span></span>|<span data-ttu-id="1746a-219">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="1746a-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="1746a-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="1746a-220">settingsDefaultVolume</span></span>|<span data-ttu-id="1746a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-221">Int32</span></span>|<span data-ttu-id="1746a-222">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="1746a-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="1746a-223">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="1746a-223">Permitted values are 0-100.</span></span> <span data-ttu-id="1746a-224">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="1746a-224">The default is 45.</span></span> <span data-ttu-id="1746a-225">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="1746a-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1746a-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1746a-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="1746a-227">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-227">Int32</span></span>|<span data-ttu-id="1746a-228">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="1746a-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="1746a-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1746a-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="1746a-230">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-230">Int32</span></span>|<span data-ttu-id="1746a-231">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1746a-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="1746a-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1746a-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="1746a-233">Int32</span><span class="sxs-lookup"><span data-stu-id="1746a-233">Int32</span></span>|<span data-ttu-id="1746a-234">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="1746a-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="1746a-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="1746a-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="1746a-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="1746a-236">Boolean</span></span>|<span data-ttu-id="1746a-237">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="1746a-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="1746a-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="1746a-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="1746a-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1746a-239">String</span></span>|<span data-ttu-id="1746a-240">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="1746a-240">The welcome screen background image URL.</span></span> <span data-ttu-id="1746a-241">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="1746a-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="1746a-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="1746a-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="1746a-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="1746a-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="1746a-244">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="1746a-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="1746a-245">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="1746a-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="1746a-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="1746a-246">Response</span></span>
<span data-ttu-id="1746a-247">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1746a-247">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1746a-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1746a-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="1746a-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1746a-249">Request</span></span>
<span data-ttu-id="1746a-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1746a-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1746a-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="1746a-251">Response</span></span>
<span data-ttu-id="1746a-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1746a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




