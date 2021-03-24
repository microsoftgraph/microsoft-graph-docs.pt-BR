---
title: Criar macOSSoftwareUpdateConfiguration
description: Crie um novo objeto macOSSoftwareUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e7d58e0543daaefe92d21e5081332d12391b41c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132643"
---
# <a name="create-macossoftwareupdateconfiguration"></a><span data-ttu-id="c4273-103">Criar macOSSoftwareUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4273-103">Create macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="c4273-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4273-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4273-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4273-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4273-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4273-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4273-107">Crie um novo [objeto macOSSoftwareUpdateConfiguration.](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-107">Create a new [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4273-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4273-108">Prerequisites</span></span>
<span data-ttu-id="c4273-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4273-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4273-111">Permission type</span></span>|<span data-ttu-id="c4273-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4273-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4273-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4273-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4273-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4273-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4273-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4273-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4273-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4273-116">Not supported.</span></span>|
|<span data-ttu-id="c4273-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4273-117">Application</span></span>|<span data-ttu-id="c4273-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4273-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4273-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4273-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c4273-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4273-120">Request headers</span></span>
|<span data-ttu-id="c4273-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4273-121">Header</span></span>|<span data-ttu-id="c4273-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4273-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4273-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4273-123">Authorization</span></span>|<span data-ttu-id="c4273-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4273-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4273-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4273-125">Accept</span></span>|<span data-ttu-id="c4273-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4273-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4273-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4273-127">Request body</span></span>
<span data-ttu-id="c4273-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSSoftwareUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c4273-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateConfiguration object.</span></span>

<span data-ttu-id="c4273-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSSoftwareUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c4273-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateConfiguration.</span></span>

|<span data-ttu-id="c4273-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4273-130">Property</span></span>|<span data-ttu-id="c4273-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4273-131">Type</span></span>|<span data-ttu-id="c4273-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4273-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4273-133">id</span><span class="sxs-lookup"><span data-stu-id="c4273-133">id</span></span>|<span data-ttu-id="c4273-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4273-134">String</span></span>|<span data-ttu-id="c4273-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4273-135">Key of the entity.</span></span> <span data-ttu-id="c4273-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4273-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c4273-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4273-138">DateTimeOffset</span></span>|<span data-ttu-id="c4273-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c4273-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c4273-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4273-141">roleScopeTagIds</span></span>|<span data-ttu-id="c4273-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4273-142">String collection</span></span>|<span data-ttu-id="c4273-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="c4273-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4273-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4273-145">supportsScopeTags</span></span>|<span data-ttu-id="c4273-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="c4273-146">Boolean</span></span>|<span data-ttu-id="c4273-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c4273-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4273-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c4273-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4273-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4273-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4273-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4273-150">This property is read-only.</span></span> <span data-ttu-id="c4273-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4273-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4273-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4273-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4273-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="c4273-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4273-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4273-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4273-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4273-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4273-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="c4273-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4273-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4273-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4273-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4273-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4273-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="c4273-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4273-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4273-164">createdDateTime</span></span>|<span data-ttu-id="c4273-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4273-165">DateTimeOffset</span></span>|<span data-ttu-id="c4273-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c4273-166">DateTime the object was created.</span></span> <span data-ttu-id="c4273-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-168">descrição</span><span class="sxs-lookup"><span data-stu-id="c4273-168">description</span></span>|<span data-ttu-id="c4273-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4273-169">String</span></span>|<span data-ttu-id="c4273-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4273-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4273-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c4273-172">displayName</span></span>|<span data-ttu-id="c4273-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4273-173">String</span></span>|<span data-ttu-id="c4273-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4273-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4273-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-176">versão</span><span class="sxs-lookup"><span data-stu-id="c4273-176">version</span></span>|<span data-ttu-id="c4273-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c4273-177">Int32</span></span>|<span data-ttu-id="c4273-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4273-178">Version of the device configuration.</span></span> <span data-ttu-id="c4273-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4273-180">criticalUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="c4273-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="c4273-182">Atualize o comportamento para atualizações críticas.</span><span class="sxs-lookup"><span data-stu-id="c4273-182">Update behavior for critical updates.</span></span> <span data-ttu-id="c4273-183">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="c4273-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="c4273-184">configDataUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="c4273-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="c4273-186">Atualizar comportamento para atualizações de arquivo de dados de configuração.</span><span class="sxs-lookup"><span data-stu-id="c4273-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="c4273-187">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="c4273-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="c4273-188">firmwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="c4273-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="c4273-190">Comportamento de atualização para atualizações de firmware.</span><span class="sxs-lookup"><span data-stu-id="c4273-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="c4273-191">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="c4273-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="c4273-192">allOtherUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="c4273-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="c4273-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="c4273-194">Atualize o comportamento de todas as outras atualizações.</span><span class="sxs-lookup"><span data-stu-id="c4273-194">Update behavior for all other updates.</span></span> <span data-ttu-id="c4273-195">Os valores possíveis são: `notConfigured` e `default`.</span><span class="sxs-lookup"><span data-stu-id="c4273-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="c4273-196">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="c4273-196">updateScheduleType</span></span>|[<span data-ttu-id="c4273-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="c4273-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="c4273-198">Atualizar tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="c4273-198">Update schedule type.</span></span> <span data-ttu-id="c4273-199">Os valores possíveis são: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="c4273-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="c4273-200">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="c4273-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="c4273-201">[Coleção customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="c4273-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="c4273-202">Janelas de tempo personalizadas quando as atualizações serão permitidas ou bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="c4273-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="c4273-203">Essa coleção pode conter no máximo 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="c4273-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="c4273-204">updateTimeWindowUtcOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="c4273-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="c4273-205">Int32</span><span class="sxs-lookup"><span data-stu-id="c4273-205">Int32</span></span>|<span data-ttu-id="c4273-206">Minutos indicando deslocamento UTC para cada janela de tempo de atualização</span><span class="sxs-lookup"><span data-stu-id="c4273-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="c4273-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4273-207">Response</span></span>
<span data-ttu-id="c4273-208">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4273-208">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4273-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4273-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4273-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4273-210">Request</span></span>
<span data-ttu-id="c4273-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4273-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c4273-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4273-212">Response</span></span>
<span data-ttu-id="c4273-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4273-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




