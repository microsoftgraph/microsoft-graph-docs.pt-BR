---
title: Atualizar macOSSoftwareUpdateConfiguration
description: Atualiza as propriedades de um objeto macOSSoftwareUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c1e87c2ff6aa528ef76b8a89239c36fb6b17ac4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704885"
---
# <a name="update-macossoftwareupdateconfiguration"></a><span data-ttu-id="79257-103">Atualizar macOSSoftwareUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="79257-103">Update macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="79257-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79257-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79257-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79257-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79257-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79257-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79257-107">Atualiza as propriedades de um objeto [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79257-107">Update the properties of a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79257-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79257-108">Prerequisites</span></span>
<span data-ttu-id="79257-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79257-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79257-111">Permission type</span></span>|<span data-ttu-id="79257-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79257-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79257-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79257-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79257-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79257-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79257-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79257-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79257-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79257-116">Not supported.</span></span>|
|<span data-ttu-id="79257-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79257-117">Application</span></span>|<span data-ttu-id="79257-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79257-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79257-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79257-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="79257-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-120">Request headers</span></span>
|<span data-ttu-id="79257-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79257-121">Header</span></span>|<span data-ttu-id="79257-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79257-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79257-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79257-123">Authorization</span></span>|<span data-ttu-id="79257-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79257-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79257-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79257-125">Accept</span></span>|<span data-ttu-id="79257-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79257-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79257-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-127">Request body</span></span>
<span data-ttu-id="79257-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79257-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

<span data-ttu-id="79257-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79257-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md).</span></span>

|<span data-ttu-id="79257-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79257-130">Property</span></span>|<span data-ttu-id="79257-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79257-131">Type</span></span>|<span data-ttu-id="79257-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79257-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79257-133">id</span><span class="sxs-lookup"><span data-stu-id="79257-133">id</span></span>|<span data-ttu-id="79257-134">String</span><span class="sxs-lookup"><span data-stu-id="79257-134">String</span></span>|<span data-ttu-id="79257-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="79257-135">Key of the entity.</span></span> <span data-ttu-id="79257-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79257-137">lastModifiedDateTime</span></span>|<span data-ttu-id="79257-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79257-138">DateTimeOffset</span></span>|<span data-ttu-id="79257-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="79257-139">DateTime the object was last modified.</span></span> <span data-ttu-id="79257-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79257-141">roleScopeTagIds</span></span>|<span data-ttu-id="79257-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79257-142">String collection</span></span>|<span data-ttu-id="79257-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="79257-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79257-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="79257-145">supportsScopeTags</span></span>|<span data-ttu-id="79257-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="79257-146">Boolean</span></span>|<span data-ttu-id="79257-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="79257-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79257-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="79257-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79257-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="79257-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79257-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79257-150">This property is read-only.</span></span> <span data-ttu-id="79257-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79257-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="79257-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79257-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="79257-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="79257-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="79257-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79257-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="79257-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79257-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="79257-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="79257-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="79257-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="79257-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="79257-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="79257-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="79257-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="79257-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="79257-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79257-164">createdDateTime</span></span>|<span data-ttu-id="79257-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79257-165">DateTimeOffset</span></span>|<span data-ttu-id="79257-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="79257-166">DateTime the object was created.</span></span> <span data-ttu-id="79257-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-168">description</span><span class="sxs-lookup"><span data-stu-id="79257-168">description</span></span>|<span data-ttu-id="79257-169">String</span><span class="sxs-lookup"><span data-stu-id="79257-169">String</span></span>|<span data-ttu-id="79257-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79257-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79257-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-172">displayName</span><span class="sxs-lookup"><span data-stu-id="79257-172">displayName</span></span>|<span data-ttu-id="79257-173">String</span><span class="sxs-lookup"><span data-stu-id="79257-173">String</span></span>|<span data-ttu-id="79257-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79257-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79257-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-176">versão</span><span class="sxs-lookup"><span data-stu-id="79257-176">version</span></span>|<span data-ttu-id="79257-177">Int32</span><span class="sxs-lookup"><span data-stu-id="79257-177">Int32</span></span>|<span data-ttu-id="79257-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79257-178">Version of the device configuration.</span></span> <span data-ttu-id="79257-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79257-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79257-180">criticalUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="79257-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="79257-182">Comportamento de atualização para atualizações críticas.</span><span class="sxs-lookup"><span data-stu-id="79257-182">Update behavior for critical updates.</span></span> <span data-ttu-id="79257-183">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="79257-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="79257-184">configDataUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="79257-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="79257-186">Comportamento de atualização para atualizações de arquivo de dados de configuração.</span><span class="sxs-lookup"><span data-stu-id="79257-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="79257-187">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="79257-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="79257-188">firmwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="79257-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="79257-190">Comportamento de atualização para atualizações de firmware.</span><span class="sxs-lookup"><span data-stu-id="79257-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="79257-191">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="79257-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="79257-192">allOtherUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="79257-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="79257-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="79257-194">Atualize o comportamento de todas as outras atualizações.</span><span class="sxs-lookup"><span data-stu-id="79257-194">Update behavior for all other updates.</span></span> <span data-ttu-id="79257-195">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="79257-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="79257-196">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="79257-196">updateScheduleType</span></span>|[<span data-ttu-id="79257-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="79257-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="79257-198">Atualizar tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="79257-198">Update schedule type.</span></span> <span data-ttu-id="79257-199">Os valores possíveis são: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="79257-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="79257-200">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="79257-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="79257-201">coleção [customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="79257-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="79257-202">Janelas de tempo personalizadas quando as atualizações serão permitidas ou bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="79257-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="79257-203">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="79257-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="79257-204">updateTimeWindowUtcOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="79257-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="79257-205">Int32</span><span class="sxs-lookup"><span data-stu-id="79257-205">Int32</span></span>|<span data-ttu-id="79257-206">Minutos que indica o deslocamento UTC para cada janela de tempo de atualização</span><span class="sxs-lookup"><span data-stu-id="79257-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="79257-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="79257-207">Response</span></span>
<span data-ttu-id="79257-208">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79257-208">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79257-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79257-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="79257-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-210">Request</span></span>
<span data-ttu-id="79257-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79257-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1542

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```

### <a name="response"></a><span data-ttu-id="79257-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="79257-212">Response</span></span>
<span data-ttu-id="79257-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79257-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1714

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "b8e467ac-67ac-b8e4-ac67-e4b8ac67e4b8",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```





