---
title: Criar windows10TeamGeneralConfiguration
description: Criar um novo objeto windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f977f1a644d4de74a833c3c0ed03f1a52cb4f89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127428"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="beed7-103">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="beed7-103">Create windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="beed7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beed7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="beed7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="beed7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beed7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="beed7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beed7-107">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beed7-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beed7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="beed7-108">Prerequisites</span></span>
<span data-ttu-id="beed7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beed7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beed7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beed7-111">Permission type</span></span>|<span data-ttu-id="beed7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="beed7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beed7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beed7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beed7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beed7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="beed7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beed7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beed7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beed7-116">Not supported.</span></span>|
|<span data-ttu-id="beed7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beed7-117">Application</span></span>|<span data-ttu-id="beed7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beed7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="beed7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beed7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="beed7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beed7-120">Request headers</span></span>
|<span data-ttu-id="beed7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="beed7-121">Header</span></span>|<span data-ttu-id="beed7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="beed7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beed7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="beed7-123">Authorization</span></span>|<span data-ttu-id="beed7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beed7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beed7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="beed7-125">Accept</span></span>|<span data-ttu-id="beed7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="beed7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beed7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beed7-127">Request body</span></span>
<span data-ttu-id="beed7-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="beed7-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="beed7-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="beed7-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="beed7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="beed7-130">Property</span></span>|<span data-ttu-id="beed7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="beed7-131">Type</span></span>|<span data-ttu-id="beed7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="beed7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beed7-133">id</span><span class="sxs-lookup"><span data-stu-id="beed7-133">id</span></span>|<span data-ttu-id="beed7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-134">String</span></span>|<span data-ttu-id="beed7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="beed7-135">Key of the entity.</span></span> <span data-ttu-id="beed7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="beed7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="beed7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beed7-138">DateTimeOffset</span></span>|<span data-ttu-id="beed7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="beed7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="beed7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="beed7-141">roleScopeTagIds</span></span>|<span data-ttu-id="beed7-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-142">String collection</span></span>|<span data-ttu-id="beed7-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="beed7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="beed7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="beed7-145">supportsScopeTags</span></span>|<span data-ttu-id="beed7-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="beed7-146">Boolean</span></span>|<span data-ttu-id="beed7-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="beed7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="beed7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="beed7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="beed7-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="beed7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="beed7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="beed7-150">This property is read-only.</span></span> <span data-ttu-id="beed7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="beed7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="beed7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="beed7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="beed7-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="beed7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="beed7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="beed7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="beed7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="beed7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="beed7-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="beed7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="beed7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="beed7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="beed7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="beed7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="beed7-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="beed7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="beed7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="beed7-164">createdDateTime</span></span>|<span data-ttu-id="beed7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beed7-165">DateTimeOffset</span></span>|<span data-ttu-id="beed7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="beed7-166">DateTime the object was created.</span></span> <span data-ttu-id="beed7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-168">descrição</span><span class="sxs-lookup"><span data-stu-id="beed7-168">description</span></span>|<span data-ttu-id="beed7-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-169">String</span></span>|<span data-ttu-id="beed7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="beed7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="beed7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="beed7-172">displayName</span></span>|<span data-ttu-id="beed7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-173">String</span></span>|<span data-ttu-id="beed7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="beed7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="beed7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-176">versão</span><span class="sxs-lookup"><span data-stu-id="beed7-176">version</span></span>|<span data-ttu-id="beed7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-177">Int32</span></span>|<span data-ttu-id="beed7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="beed7-178">Version of the device configuration.</span></span> <span data-ttu-id="beed7-179">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="beed7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="beed7-180">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="beed7-180">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="beed7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-181">Boolean</span></span>|<span data-ttu-id="beed7-182">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="beed7-182">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="beed7-183">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="beed7-183">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="beed7-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-184">String</span></span>|<span data-ttu-id="beed7-185">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="beed7-185">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="beed7-186">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="beed7-186">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="beed7-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-187">String</span></span>|<span data-ttu-id="beed7-188">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="beed7-188">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="beed7-189">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="beed7-189">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="beed7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-190">Boolean</span></span>|<span data-ttu-id="beed7-191">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="beed7-191">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="beed7-192">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="beed7-192">maintenanceWindowBlocked</span></span>|<span data-ttu-id="beed7-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-193">Boolean</span></span>|<span data-ttu-id="beed7-194">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="beed7-194">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="beed7-195">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="beed7-195">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="beed7-196">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-196">Int32</span></span>|<span data-ttu-id="beed7-197">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="beed7-197">Maintenance window duration for device updates.</span></span> <span data-ttu-id="beed7-198">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="beed7-198">Valid values 0 to 5</span></span>|
|<span data-ttu-id="beed7-199">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="beed7-199">maintenanceWindowStartTime</span></span>|<span data-ttu-id="beed7-200">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="beed7-200">TimeOfDay</span></span>|<span data-ttu-id="beed7-201">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="beed7-201">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="beed7-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="beed7-202">miracastChannel</span></span>|[<span data-ttu-id="beed7-203">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="beed7-203">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="beed7-204">O canal.</span><span class="sxs-lookup"><span data-stu-id="beed7-204">The channel.</span></span> <span data-ttu-id="beed7-205">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="beed7-205">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="beed7-206">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="beed7-206">miracastBlocked</span></span>|<span data-ttu-id="beed7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-207">Boolean</span></span>|<span data-ttu-id="beed7-208">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="beed7-208">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="beed7-209">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="beed7-209">miracastRequirePin</span></span>|<span data-ttu-id="beed7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-210">Boolean</span></span>|<span data-ttu-id="beed7-211">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="beed7-211">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="beed7-212">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="beed7-212">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="beed7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-213">Boolean</span></span>|<span data-ttu-id="beed7-214">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="beed7-214">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="beed7-215">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="beed7-215">settingsBlockSessionResume</span></span>|<span data-ttu-id="beed7-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-216">Boolean</span></span>|<span data-ttu-id="beed7-217">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="beed7-217">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="beed7-218">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="beed7-218">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="beed7-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-219">Boolean</span></span>|<span data-ttu-id="beed7-220">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="beed7-220">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="beed7-221">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="beed7-221">settingsDefaultVolume</span></span>|<span data-ttu-id="beed7-222">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-222">Int32</span></span>|<span data-ttu-id="beed7-223">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="beed7-223">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="beed7-224">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="beed7-224">Permitted values are 0-100.</span></span> <span data-ttu-id="beed7-225">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="beed7-225">The default is 45.</span></span> <span data-ttu-id="beed7-226">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="beed7-226">Valid values 0 to 100</span></span>|
|<span data-ttu-id="beed7-227">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="beed7-227">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="beed7-228">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-228">Int32</span></span>|<span data-ttu-id="beed7-229">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="beed7-229">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="beed7-230">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="beed7-230">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="beed7-231">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-231">Int32</span></span>|<span data-ttu-id="beed7-232">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="beed7-232">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="beed7-233">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="beed7-233">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="beed7-234">Int32</span><span class="sxs-lookup"><span data-stu-id="beed7-234">Int32</span></span>|<span data-ttu-id="beed7-235">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="beed7-235">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="beed7-236">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="beed7-236">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="beed7-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="beed7-237">Boolean</span></span>|<span data-ttu-id="beed7-238">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="beed7-238">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="beed7-239">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="beed7-239">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="beed7-240">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beed7-240">String</span></span>|<span data-ttu-id="beed7-241">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="beed7-241">The welcome screen background image URL.</span></span> <span data-ttu-id="beed7-242">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="beed7-242">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="beed7-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="beed7-243">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="beed7-244">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="beed7-244">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="beed7-245">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="beed7-245">The welcome screen meeting information shown.</span></span> <span data-ttu-id="beed7-246">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="beed7-246">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="beed7-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="beed7-247">Response</span></span>
<span data-ttu-id="beed7-248">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="beed7-248">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beed7-249">Exemplo</span><span class="sxs-lookup"><span data-stu-id="beed7-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="beed7-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beed7-250">Request</span></span>
<span data-ttu-id="beed7-251">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="beed7-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="beed7-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="beed7-252">Response</span></span>
<span data-ttu-id="beed7-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="beed7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




