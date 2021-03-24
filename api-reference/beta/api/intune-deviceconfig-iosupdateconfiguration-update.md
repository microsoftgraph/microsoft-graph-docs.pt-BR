---
title: Atualizar iosUpdateConfiguration
description: Atualizar as propriedades de um objeto iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c0009cc5a5d127ee9abbdbfe97f56591e2ba1a1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137396"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="aea0c-103">Atualizar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="aea0c-103">Update iosUpdateConfiguration</span></span>

<span data-ttu-id="aea0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aea0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aea0c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aea0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aea0c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aea0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea0c-107">Atualizar as propriedades de um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aea0c-107">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aea0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aea0c-108">Prerequisites</span></span>
<span data-ttu-id="aea0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aea0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aea0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aea0c-111">Permission type</span></span>|<span data-ttu-id="aea0c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aea0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aea0c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aea0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aea0c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea0c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aea0c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aea0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aea0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aea0c-116">Not supported.</span></span>|
|<span data-ttu-id="aea0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aea0c-117">Application</span></span>|<span data-ttu-id="aea0c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea0c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aea0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aea0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aea0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aea0c-120">Request headers</span></span>
|<span data-ttu-id="aea0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aea0c-121">Header</span></span>|<span data-ttu-id="aea0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aea0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aea0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aea0c-123">Authorization</span></span>|<span data-ttu-id="aea0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aea0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aea0c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aea0c-125">Accept</span></span>|<span data-ttu-id="aea0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aea0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aea0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aea0c-127">Request body</span></span>
<span data-ttu-id="aea0c-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aea0c-128">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="aea0c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aea0c-129">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="aea0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aea0c-130">Property</span></span>|<span data-ttu-id="aea0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aea0c-131">Type</span></span>|<span data-ttu-id="aea0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aea0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea0c-133">id</span><span class="sxs-lookup"><span data-stu-id="aea0c-133">id</span></span>|<span data-ttu-id="aea0c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aea0c-134">String</span></span>|<span data-ttu-id="aea0c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aea0c-135">Key of the entity.</span></span> <span data-ttu-id="aea0c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aea0c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aea0c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea0c-138">DateTimeOffset</span></span>|<span data-ttu-id="aea0c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aea0c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aea0c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aea0c-141">roleScopeTagIds</span></span>|<span data-ttu-id="aea0c-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aea0c-142">String collection</span></span>|<span data-ttu-id="aea0c-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="aea0c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aea0c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aea0c-145">supportsScopeTags</span></span>|<span data-ttu-id="aea0c-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="aea0c-146">Boolean</span></span>|<span data-ttu-id="aea0c-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="aea0c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aea0c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="aea0c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aea0c-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="aea0c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aea0c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aea0c-150">This property is read-only.</span></span> <span data-ttu-id="aea0c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aea0c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aea0c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aea0c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aea0c-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="aea0c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aea0c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aea0c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aea0c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aea0c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aea0c-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="aea0c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aea0c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aea0c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aea0c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aea0c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aea0c-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="aea0c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aea0c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aea0c-164">createdDateTime</span></span>|<span data-ttu-id="aea0c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea0c-165">DateTimeOffset</span></span>|<span data-ttu-id="aea0c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aea0c-166">DateTime the object was created.</span></span> <span data-ttu-id="aea0c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-168">descrição</span><span class="sxs-lookup"><span data-stu-id="aea0c-168">description</span></span>|<span data-ttu-id="aea0c-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aea0c-169">String</span></span>|<span data-ttu-id="aea0c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aea0c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aea0c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="aea0c-172">displayName</span></span>|<span data-ttu-id="aea0c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aea0c-173">String</span></span>|<span data-ttu-id="aea0c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aea0c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aea0c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-176">versão</span><span class="sxs-lookup"><span data-stu-id="aea0c-176">version</span></span>|<span data-ttu-id="aea0c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aea0c-177">Int32</span></span>|<span data-ttu-id="aea0c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aea0c-178">Version of the device configuration.</span></span> <span data-ttu-id="aea0c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aea0c-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="aea0c-180">isEnabled</span></span>|<span data-ttu-id="aea0c-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="aea0c-181">Boolean</span></span>|<span data-ttu-id="aea0c-182">A configuração está habilitada na interface do usuário</span><span class="sxs-lookup"><span data-stu-id="aea0c-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="aea0c-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="aea0c-183">activeHoursStart</span></span>|<span data-ttu-id="aea0c-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="aea0c-184">TimeOfDay</span></span>|<span data-ttu-id="aea0c-185">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="aea0c-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="aea0c-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="aea0c-186">activeHoursEnd</span></span>|<span data-ttu-id="aea0c-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="aea0c-187">TimeOfDay</span></span>|<span data-ttu-id="aea0c-188">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="aea0c-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="aea0c-189">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="aea0c-189">desiredOsVersion</span></span>|<span data-ttu-id="aea0c-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aea0c-190">String</span></span>|<span data-ttu-id="aea0c-191">Se não especificado, os dispositivos serão atualizados para a versão mais recente do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="aea0c-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="aea0c-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="aea0c-192">scheduledInstallDays</span></span>|<span data-ttu-id="aea0c-193">[Coleção dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="aea0c-194">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="aea0c-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="aea0c-195">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="aea0c-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="aea0c-196">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="aea0c-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="aea0c-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="aea0c-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="aea0c-198">Int32</span><span class="sxs-lookup"><span data-stu-id="aea0c-198">Int32</span></span>|<span data-ttu-id="aea0c-199">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="aea0c-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="aea0c-200">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="aea0c-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="aea0c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="aea0c-201">Int32</span></span>|<span data-ttu-id="aea0c-202">Dias antes que as atualizações de software sejam visíveis para dispositivos iOS que variam de 0 a 90 inclusive</span><span class="sxs-lookup"><span data-stu-id="aea0c-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="aea0c-203">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="aea0c-203">updateScheduleType</span></span>|[<span data-ttu-id="aea0c-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="aea0c-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="aea0c-205">Atualizar tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="aea0c-205">Update schedule type.</span></span> <span data-ttu-id="aea0c-206">Os valores possíveis são: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="aea0c-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="aea0c-207">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="aea0c-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="aea0c-208">[Coleção customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="aea0c-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="aea0c-209">Se o tipo de agendamento de atualização estiver definido para usar o agendamento de janelas de tempo, janelas de tempo personalizadas quando as atualizações serão agendadas.</span><span class="sxs-lookup"><span data-stu-id="aea0c-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="aea0c-210">Essa coleção pode conter no máximo 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="aea0c-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="aea0c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="aea0c-211">Response</span></span>
<span data-ttu-id="aea0c-212">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aea0c-212">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aea0c-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aea0c-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="aea0c-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aea0c-214">Request</span></span>
<span data-ttu-id="aea0c-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aea0c-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aea0c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="aea0c-216">Response</span></span>
<span data-ttu-id="aea0c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aea0c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




