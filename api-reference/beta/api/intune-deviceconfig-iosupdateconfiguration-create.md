---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0548cb809f0eb5013a393c36b2ab73cdffa53cc4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977286"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="b9fad-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9fad-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="b9fad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9fad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9fad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9fad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9fad-106">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9fad-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9fad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9fad-107">Prerequisites</span></span>
<span data-ttu-id="b9fad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9fad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9fad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9fad-110">Permission type</span></span>|<span data-ttu-id="b9fad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9fad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9fad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9fad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9fad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9fad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9fad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9fad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9fad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9fad-115">Not supported.</span></span>|
|<span data-ttu-id="b9fad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9fad-116">Application</span></span>|<span data-ttu-id="b9fad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9fad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9fad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9fad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b9fad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fad-119">Request headers</span></span>
|<span data-ttu-id="b9fad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9fad-120">Header</span></span>|<span data-ttu-id="b9fad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9fad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9fad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9fad-122">Authorization</span></span>|<span data-ttu-id="b9fad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9fad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9fad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9fad-124">Accept</span></span>|<span data-ttu-id="b9fad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9fad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9fad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fad-126">Request body</span></span>
<span data-ttu-id="b9fad-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b9fad-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="b9fad-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b9fad-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="b9fad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9fad-129">Property</span></span>|<span data-ttu-id="b9fad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9fad-130">Type</span></span>|<span data-ttu-id="b9fad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9fad-132">id</span><span class="sxs-lookup"><span data-stu-id="b9fad-132">id</span></span>|<span data-ttu-id="b9fad-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9fad-133">String</span></span>|<span data-ttu-id="b9fad-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b9fad-134">Key of the entity.</span></span> <span data-ttu-id="b9fad-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b9fad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fad-137">DateTimeOffset</span></span>|<span data-ttu-id="b9fad-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b9fad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b9fad-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9fad-140">roleScopeTagIds</span></span>|<span data-ttu-id="b9fad-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9fad-141">String collection</span></span>|<span data-ttu-id="b9fad-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b9fad-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9fad-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9fad-144">supportsScopeTags</span></span>|<span data-ttu-id="b9fad-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9fad-145">Boolean</span></span>|<span data-ttu-id="b9fad-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b9fad-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9fad-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b9fad-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9fad-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b9fad-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9fad-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9fad-149">This property is read-only.</span></span> <span data-ttu-id="b9fad-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9fad-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b9fad-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9fad-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b9fad-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b9fad-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b9fad-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9fad-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b9fad-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9fad-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b9fad-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b9fad-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b9fad-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9fad-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b9fad-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9fad-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b9fad-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b9fad-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b9fad-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fad-163">createdDateTime</span></span>|<span data-ttu-id="b9fad-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fad-164">DateTimeOffset</span></span>|<span data-ttu-id="b9fad-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b9fad-165">DateTime the object was created.</span></span> <span data-ttu-id="b9fad-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b9fad-167">description</span></span>|<span data-ttu-id="b9fad-168">String</span><span class="sxs-lookup"><span data-stu-id="b9fad-168">String</span></span>|<span data-ttu-id="b9fad-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9fad-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9fad-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b9fad-171">displayName</span></span>|<span data-ttu-id="b9fad-172">String</span><span class="sxs-lookup"><span data-stu-id="b9fad-172">String</span></span>|<span data-ttu-id="b9fad-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9fad-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9fad-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-175">versão</span><span class="sxs-lookup"><span data-stu-id="b9fad-175">version</span></span>|<span data-ttu-id="b9fad-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b9fad-176">Int32</span></span>|<span data-ttu-id="b9fad-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9fad-177">Version of the device configuration.</span></span> <span data-ttu-id="b9fad-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9fad-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b9fad-179">isEnabled</span></span>|<span data-ttu-id="b9fad-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9fad-180">Boolean</span></span>|<span data-ttu-id="b9fad-181">A configuração está habilitada na IU</span><span class="sxs-lookup"><span data-stu-id="b9fad-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="b9fad-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b9fad-182">activeHoursStart</span></span>|<span data-ttu-id="b9fad-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9fad-183">TimeOfDay</span></span>|<span data-ttu-id="b9fad-184">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="b9fad-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="b9fad-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b9fad-185">activeHoursEnd</span></span>|<span data-ttu-id="b9fad-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9fad-186">TimeOfDay</span></span>|<span data-ttu-id="b9fad-187">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="b9fad-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="b9fad-188">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="b9fad-188">scheduledInstallDays</span></span>|<span data-ttu-id="b9fad-189">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="b9fad-189">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="b9fad-190">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="b9fad-190">Days in week for which active hours are configured.</span></span> <span data-ttu-id="b9fad-191">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="b9fad-191">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="b9fad-192">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="b9fad-192">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b9fad-193">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="b9fad-193">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="b9fad-194">Int32</span><span class="sxs-lookup"><span data-stu-id="b9fad-194">Int32</span></span>|<span data-ttu-id="b9fad-195">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="b9fad-195">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="b9fad-196">Propriedadeenforcedsoftwareupdatedelayindays</span><span class="sxs-lookup"><span data-stu-id="b9fad-196">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="b9fad-197">Int32</span><span class="sxs-lookup"><span data-stu-id="b9fad-197">Int32</span></span>|<span data-ttu-id="b9fad-198">Dias antes que as atualizações de software fiquem visíveis para dispositivos iOS variando de 0 a 90, inclusive</span><span class="sxs-lookup"><span data-stu-id="b9fad-198">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="b9fad-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fad-199">Response</span></span>
<span data-ttu-id="b9fad-200">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9fad-200">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9fad-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9fad-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9fad-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fad-202">Request</span></span>
<span data-ttu-id="b9fad-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9fad-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1255

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
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="b9fad-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fad-204">Response</span></span>
<span data-ttu-id="b9fad-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9fad-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1427

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
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





