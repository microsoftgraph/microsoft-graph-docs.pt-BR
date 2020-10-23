---
title: Atualizar androidOmaCpConfiguration
description: Atualiza as propriedades de um objeto androidOmaCpConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17a17a2fada5745273f95ef759378a8c85b605f8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692174"
---
# <a name="update-androidomacpconfiguration"></a><span data-ttu-id="e2d30-103">Atualizar androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2d30-103">Update androidOmaCpConfiguration</span></span>

<span data-ttu-id="e2d30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2d30-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2d30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2d30-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2d30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2d30-107">Atualiza as propriedades de um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2d30-107">Update the properties of a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2d30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2d30-108">Prerequisites</span></span>
<span data-ttu-id="e2d30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2d30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2d30-111">Permission type</span></span>|<span data-ttu-id="e2d30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2d30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2d30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2d30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2d30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2d30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2d30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2d30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2d30-116">Not supported.</span></span>|
|<span data-ttu-id="e2d30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2d30-117">Application</span></span>|<span data-ttu-id="e2d30-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d30-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2d30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2d30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e2d30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d30-120">Request headers</span></span>
|<span data-ttu-id="e2d30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2d30-121">Header</span></span>|<span data-ttu-id="e2d30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2d30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2d30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2d30-123">Authorization</span></span>|<span data-ttu-id="e2d30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2d30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2d30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2d30-125">Accept</span></span>|<span data-ttu-id="e2d30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2d30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2d30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d30-127">Request body</span></span>
<span data-ttu-id="e2d30-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2d30-128">In the request body, supply a JSON representation for the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

<span data-ttu-id="e2d30-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2d30-129">The following table shows the properties that are required when you create the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span></span>

|<span data-ttu-id="e2d30-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d30-130">Property</span></span>|<span data-ttu-id="e2d30-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d30-131">Type</span></span>|<span data-ttu-id="e2d30-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d30-133">id</span><span class="sxs-lookup"><span data-stu-id="e2d30-133">id</span></span>|<span data-ttu-id="e2d30-134">String</span><span class="sxs-lookup"><span data-stu-id="e2d30-134">String</span></span>|<span data-ttu-id="e2d30-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2d30-135">Key of the entity.</span></span> <span data-ttu-id="e2d30-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2d30-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2d30-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2d30-138">DateTimeOffset</span></span>|<span data-ttu-id="e2d30-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e2d30-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2d30-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2d30-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2d30-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2d30-142">String collection</span></span>|<span data-ttu-id="e2d30-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e2d30-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2d30-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e2d30-145">supportsScopeTags</span></span>|<span data-ttu-id="e2d30-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2d30-146">Boolean</span></span>|<span data-ttu-id="e2d30-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2d30-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2d30-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e2d30-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2d30-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2d30-150">This property is read-only.</span></span> <span data-ttu-id="e2d30-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2d30-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2d30-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2d30-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2d30-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="e2d30-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2d30-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2d30-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2d30-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2d30-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2d30-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="e2d30-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2d30-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2d30-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2d30-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2d30-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2d30-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="e2d30-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2d30-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2d30-164">createdDateTime</span></span>|<span data-ttu-id="e2d30-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2d30-165">DateTimeOffset</span></span>|<span data-ttu-id="e2d30-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e2d30-166">DateTime the object was created.</span></span> <span data-ttu-id="e2d30-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-168">description</span><span class="sxs-lookup"><span data-stu-id="e2d30-168">description</span></span>|<span data-ttu-id="e2d30-169">String</span><span class="sxs-lookup"><span data-stu-id="e2d30-169">String</span></span>|<span data-ttu-id="e2d30-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2d30-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e2d30-172">displayName</span></span>|<span data-ttu-id="e2d30-173">String</span><span class="sxs-lookup"><span data-stu-id="e2d30-173">String</span></span>|<span data-ttu-id="e2d30-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2d30-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-176">versão</span><span class="sxs-lookup"><span data-stu-id="e2d30-176">version</span></span>|<span data-ttu-id="e2d30-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2d30-177">Int32</span></span>|<span data-ttu-id="e2d30-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-178">Version of the device configuration.</span></span> <span data-ttu-id="e2d30-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d30-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2d30-180">configurationXml</span><span class="sxs-lookup"><span data-stu-id="e2d30-180">configurationXml</span></span>|<span data-ttu-id="e2d30-181">Binária</span><span class="sxs-lookup"><span data-stu-id="e2d30-181">Binary</span></span>|<span data-ttu-id="e2d30-182">XML de configuração que será aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2d30-182">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="e2d30-183">Quando ele é lido, ele só fornece uma cadeia de caracteres de espaço reservado, pois os dados originais são criptografados e armazenados.</span><span class="sxs-lookup"><span data-stu-id="e2d30-183">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="e2d30-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2d30-184">Response</span></span>
<span data-ttu-id="e2d30-185">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2d30-185">If successful, this method returns a `200 OK` response code and an updated [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2d30-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2d30-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2d30-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d30-187">Request</span></span>
<span data-ttu-id="e2d30-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2d30-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="e2d30-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2d30-189">Response</span></span>
<span data-ttu-id="e2d30-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2d30-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





