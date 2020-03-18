---
title: Atualizar iosUpdateConfiguration
description: Atualizar as propriedades de um objeto iosUpdateConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4515cee39f8b037e34599c92ab3f56ba0c111efb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42748980"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="26aef-103">Atualizar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="26aef-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="26aef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26aef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26aef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26aef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26aef-106">Atualizar as propriedades de um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26aef-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26aef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26aef-107">Prerequisites</span></span>
<span data-ttu-id="26aef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26aef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26aef-110">Permission type</span></span>|<span data-ttu-id="26aef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26aef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26aef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26aef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26aef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26aef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26aef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26aef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26aef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26aef-115">Not supported.</span></span>|
|<span data-ttu-id="26aef-116">Application</span><span class="sxs-lookup"><span data-stu-id="26aef-116">Application</span></span>|<span data-ttu-id="26aef-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26aef-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26aef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26aef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="26aef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26aef-119">Request headers</span></span>
|<span data-ttu-id="26aef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26aef-120">Header</span></span>|<span data-ttu-id="26aef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26aef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26aef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26aef-122">Authorization</span></span>|<span data-ttu-id="26aef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26aef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26aef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26aef-124">Accept</span></span>|<span data-ttu-id="26aef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26aef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26aef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26aef-126">Request body</span></span>
<span data-ttu-id="26aef-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26aef-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="26aef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26aef-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="26aef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26aef-129">Property</span></span>|<span data-ttu-id="26aef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26aef-130">Type</span></span>|<span data-ttu-id="26aef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26aef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26aef-132">id</span><span class="sxs-lookup"><span data-stu-id="26aef-132">id</span></span>|<span data-ttu-id="26aef-133">String</span><span class="sxs-lookup"><span data-stu-id="26aef-133">String</span></span>|<span data-ttu-id="26aef-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26aef-134">Key of the entity.</span></span> <span data-ttu-id="26aef-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26aef-136">lastModifiedDateTime</span></span>|<span data-ttu-id="26aef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26aef-137">DateTimeOffset</span></span>|<span data-ttu-id="26aef-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="26aef-138">DateTime the object was last modified.</span></span> <span data-ttu-id="26aef-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26aef-140">roleScopeTagIds</span></span>|<span data-ttu-id="26aef-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26aef-141">String collection</span></span>|<span data-ttu-id="26aef-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="26aef-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26aef-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26aef-144">supportsScopeTags</span></span>|<span data-ttu-id="26aef-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="26aef-145">Boolean</span></span>|<span data-ttu-id="26aef-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="26aef-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26aef-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="26aef-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26aef-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="26aef-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26aef-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26aef-149">This property is read-only.</span></span> <span data-ttu-id="26aef-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26aef-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="26aef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26aef-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="26aef-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="26aef-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="26aef-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26aef-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="26aef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26aef-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="26aef-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="26aef-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="26aef-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26aef-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="26aef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26aef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="26aef-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="26aef-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="26aef-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26aef-163">createdDateTime</span></span>|<span data-ttu-id="26aef-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26aef-164">DateTimeOffset</span></span>|<span data-ttu-id="26aef-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="26aef-165">DateTime the object was created.</span></span> <span data-ttu-id="26aef-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-167">description</span><span class="sxs-lookup"><span data-stu-id="26aef-167">description</span></span>|<span data-ttu-id="26aef-168">String</span><span class="sxs-lookup"><span data-stu-id="26aef-168">String</span></span>|<span data-ttu-id="26aef-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26aef-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26aef-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-171">displayName</span><span class="sxs-lookup"><span data-stu-id="26aef-171">displayName</span></span>|<span data-ttu-id="26aef-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26aef-172">String</span></span>|<span data-ttu-id="26aef-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26aef-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26aef-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-175">versão</span><span class="sxs-lookup"><span data-stu-id="26aef-175">version</span></span>|<span data-ttu-id="26aef-176">Int32</span><span class="sxs-lookup"><span data-stu-id="26aef-176">Int32</span></span>|<span data-ttu-id="26aef-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26aef-177">Version of the device configuration.</span></span> <span data-ttu-id="26aef-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26aef-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="26aef-179">isEnabled</span></span>|<span data-ttu-id="26aef-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="26aef-180">Boolean</span></span>|<span data-ttu-id="26aef-181">A configuração está habilitada na IU</span><span class="sxs-lookup"><span data-stu-id="26aef-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="26aef-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="26aef-182">activeHoursStart</span></span>|<span data-ttu-id="26aef-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26aef-183">TimeOfDay</span></span>|<span data-ttu-id="26aef-184">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="26aef-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="26aef-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="26aef-185">activeHoursEnd</span></span>|<span data-ttu-id="26aef-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26aef-186">TimeOfDay</span></span>|<span data-ttu-id="26aef-187">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="26aef-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="26aef-188">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="26aef-188">desiredOsVersion</span></span>|<span data-ttu-id="26aef-189">String</span><span class="sxs-lookup"><span data-stu-id="26aef-189">String</span></span>|<span data-ttu-id="26aef-190">Se deixado não especificado, os dispositivos serão atualizados para a versão mais recente do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="26aef-190">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="26aef-191">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="26aef-191">scheduledInstallDays</span></span>|<span data-ttu-id="26aef-192">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-192">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="26aef-193">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="26aef-193">Days in week for which active hours are configured.</span></span> <span data-ttu-id="26aef-194">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="26aef-194">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="26aef-195">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="26aef-195">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="26aef-196">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="26aef-196">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="26aef-197">Int32</span><span class="sxs-lookup"><span data-stu-id="26aef-197">Int32</span></span>|<span data-ttu-id="26aef-198">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="26aef-198">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="26aef-199">Propriedadeenforcedsoftwareupdatedelayindays</span><span class="sxs-lookup"><span data-stu-id="26aef-199">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="26aef-200">Int32</span><span class="sxs-lookup"><span data-stu-id="26aef-200">Int32</span></span>|<span data-ttu-id="26aef-201">Dias antes que as atualizações de software fiquem visíveis para dispositivos iOS variando de 0 a 90, inclusive</span><span class="sxs-lookup"><span data-stu-id="26aef-201">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="26aef-202">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="26aef-202">updateScheduleType</span></span>|[<span data-ttu-id="26aef-203">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="26aef-203">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="26aef-204">Atualizar tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="26aef-204">Update schedule type.</span></span> <span data-ttu-id="26aef-205">Os valores possíveis são: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="26aef-205">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="26aef-206">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="26aef-206">customUpdateTimeWindows</span></span>|<span data-ttu-id="26aef-207">coleção [customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="26aef-207">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="26aef-208">Se atualizar o tipo de agendamento estiver definido para usar agendamento de janela de tempo, as janelas de tempo personalizadas quando as atualizações serão agendadas.</span><span class="sxs-lookup"><span data-stu-id="26aef-208">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="26aef-209">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="26aef-209">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="26aef-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="26aef-210">Response</span></span>
<span data-ttu-id="26aef-211">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26aef-211">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26aef-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26aef-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="26aef-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26aef-213">Request</span></span>
<span data-ttu-id="26aef-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26aef-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1596

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
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="26aef-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="26aef-215">Response</span></span>
<span data-ttu-id="26aef-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26aef-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1768

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
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```




