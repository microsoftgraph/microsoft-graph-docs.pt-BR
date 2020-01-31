---
title: Atualizar iosUpdateConfiguration
description: Atualizar as propriedades de um objeto iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 847190c77e408fb08204ca4cd3f5101efaf360e7
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635864"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="d013f-103">Atualizar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="d013f-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="d013f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d013f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d013f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d013f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d013f-106">Atualizar as propriedades de um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d013f-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d013f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d013f-107">Prerequisites</span></span>
<span data-ttu-id="d013f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d013f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d013f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d013f-110">Permission type</span></span>|<span data-ttu-id="d013f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d013f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d013f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d013f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d013f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d013f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d013f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d013f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d013f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d013f-115">Not supported.</span></span>|
|<span data-ttu-id="d013f-116">Application</span><span class="sxs-lookup"><span data-stu-id="d013f-116">Application</span></span>|<span data-ttu-id="d013f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d013f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d013f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d013f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d013f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d013f-119">Request headers</span></span>
|<span data-ttu-id="d013f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d013f-120">Header</span></span>|<span data-ttu-id="d013f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d013f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d013f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d013f-122">Authorization</span></span>|<span data-ttu-id="d013f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d013f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d013f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d013f-124">Accept</span></span>|<span data-ttu-id="d013f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d013f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d013f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d013f-126">Request body</span></span>
<span data-ttu-id="d013f-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d013f-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="d013f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d013f-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="d013f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d013f-129">Property</span></span>|<span data-ttu-id="d013f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d013f-130">Type</span></span>|<span data-ttu-id="d013f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d013f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d013f-132">id</span><span class="sxs-lookup"><span data-stu-id="d013f-132">id</span></span>|<span data-ttu-id="d013f-133">String</span><span class="sxs-lookup"><span data-stu-id="d013f-133">String</span></span>|<span data-ttu-id="d013f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d013f-134">Key of the entity.</span></span> <span data-ttu-id="d013f-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d013f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d013f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d013f-137">DateTimeOffset</span></span>|<span data-ttu-id="d013f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d013f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d013f-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d013f-140">roleScopeTagIds</span></span>|<span data-ttu-id="d013f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d013f-141">String collection</span></span>|<span data-ttu-id="d013f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d013f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d013f-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d013f-144">supportsScopeTags</span></span>|<span data-ttu-id="d013f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d013f-145">Boolean</span></span>|<span data-ttu-id="d013f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d013f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d013f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d013f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d013f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d013f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d013f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d013f-149">This property is read-only.</span></span> <span data-ttu-id="d013f-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d013f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d013f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d013f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d013f-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d013f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d013f-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d013f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d013f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d013f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d013f-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d013f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d013f-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d013f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d013f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d013f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d013f-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d013f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d013f-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d013f-163">createdDateTime</span></span>|<span data-ttu-id="d013f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d013f-164">DateTimeOffset</span></span>|<span data-ttu-id="d013f-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d013f-165">DateTime the object was created.</span></span> <span data-ttu-id="d013f-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-167">description</span><span class="sxs-lookup"><span data-stu-id="d013f-167">description</span></span>|<span data-ttu-id="d013f-168">String</span><span class="sxs-lookup"><span data-stu-id="d013f-168">String</span></span>|<span data-ttu-id="d013f-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d013f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d013f-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d013f-171">displayName</span></span>|<span data-ttu-id="d013f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d013f-172">String</span></span>|<span data-ttu-id="d013f-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d013f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d013f-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-175">versão</span><span class="sxs-lookup"><span data-stu-id="d013f-175">version</span></span>|<span data-ttu-id="d013f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d013f-176">Int32</span></span>|<span data-ttu-id="d013f-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d013f-177">Version of the device configuration.</span></span> <span data-ttu-id="d013f-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d013f-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d013f-179">isEnabled</span></span>|<span data-ttu-id="d013f-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d013f-180">Boolean</span></span>|<span data-ttu-id="d013f-181">A configuração está habilitada na IU</span><span class="sxs-lookup"><span data-stu-id="d013f-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="d013f-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d013f-182">activeHoursStart</span></span>|<span data-ttu-id="d013f-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d013f-183">TimeOfDay</span></span>|<span data-ttu-id="d013f-184">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="d013f-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d013f-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d013f-185">activeHoursEnd</span></span>|<span data-ttu-id="d013f-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d013f-186">TimeOfDay</span></span>|<span data-ttu-id="d013f-187">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="d013f-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d013f-188">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="d013f-188">desiredOsVersion</span></span>|<span data-ttu-id="d013f-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d013f-189">String</span></span>|<span data-ttu-id="d013f-190">Se deixado não especificado, os dispositivos serão atualizados para a versão mais recente do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="d013f-190">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="d013f-191">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="d013f-191">scheduledInstallDays</span></span>|<span data-ttu-id="d013f-192">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="d013f-192">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="d013f-193">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="d013f-193">Days in week for which active hours are configured.</span></span> <span data-ttu-id="d013f-194">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="d013f-194">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="d013f-195">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d013f-195">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d013f-196">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="d013f-196">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="d013f-197">Int32</span><span class="sxs-lookup"><span data-stu-id="d013f-197">Int32</span></span>|<span data-ttu-id="d013f-198">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="d013f-198">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="d013f-199">Propriedadeenforcedsoftwareupdatedelayindays</span><span class="sxs-lookup"><span data-stu-id="d013f-199">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="d013f-200">Int32</span><span class="sxs-lookup"><span data-stu-id="d013f-200">Int32</span></span>|<span data-ttu-id="d013f-201">Dias antes que as atualizações de software fiquem visíveis para dispositivos iOS variando de 0 a 90, inclusive</span><span class="sxs-lookup"><span data-stu-id="d013f-201">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="d013f-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="d013f-202">Response</span></span>
<span data-ttu-id="d013f-203">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d013f-203">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d013f-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d013f-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="d013f-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d013f-205">Request</span></span>
<span data-ttu-id="d013f-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d013f-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="d013f-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="d013f-207">Response</span></span>
<span data-ttu-id="d013f-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d013f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1478

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





