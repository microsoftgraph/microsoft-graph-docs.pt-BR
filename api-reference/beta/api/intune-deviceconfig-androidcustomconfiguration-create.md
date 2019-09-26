---
title: Criar androidCustomConfiguration
description: Criar um novo objeto androidCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad8ea5e9ccc1e1f81b45694163ba06be88739875
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170163"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="31516-103">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="31516-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="31516-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31516-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31516-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31516-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31516-106">Criar um novo objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31516-106">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31516-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31516-107">Prerequisites</span></span>
<span data-ttu-id="31516-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31516-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31516-110">Permission type</span></span>|<span data-ttu-id="31516-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31516-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31516-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31516-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31516-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31516-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31516-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31516-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31516-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31516-115">Not supported.</span></span>|
|<span data-ttu-id="31516-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31516-116">Application</span></span>|<span data-ttu-id="31516-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31516-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31516-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31516-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31516-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31516-119">Request headers</span></span>
|<span data-ttu-id="31516-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31516-120">Header</span></span>|<span data-ttu-id="31516-121">Valor</span><span class="sxs-lookup"><span data-stu-id="31516-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31516-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31516-122">Authorization</span></span>|<span data-ttu-id="31516-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31516-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31516-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31516-124">Accept</span></span>|<span data-ttu-id="31516-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31516-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31516-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31516-126">Request body</span></span>
<span data-ttu-id="31516-127">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="31516-127">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="31516-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="31516-128">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="31516-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31516-129">Property</span></span>|<span data-ttu-id="31516-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="31516-130">Type</span></span>|<span data-ttu-id="31516-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="31516-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31516-132">id</span><span class="sxs-lookup"><span data-stu-id="31516-132">id</span></span>|<span data-ttu-id="31516-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31516-133">String</span></span>|<span data-ttu-id="31516-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="31516-134">Key of the entity.</span></span> <span data-ttu-id="31516-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31516-136">lastModifiedDateTime</span></span>|<span data-ttu-id="31516-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31516-137">DateTimeOffset</span></span>|<span data-ttu-id="31516-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="31516-138">DateTime the object was last modified.</span></span> <span data-ttu-id="31516-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31516-140">roleScopeTagIds</span></span>|<span data-ttu-id="31516-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="31516-141">String collection</span></span>|<span data-ttu-id="31516-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="31516-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31516-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="31516-144">supportsScopeTags</span></span>|<span data-ttu-id="31516-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="31516-145">Boolean</span></span>|<span data-ttu-id="31516-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="31516-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31516-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="31516-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31516-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="31516-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31516-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31516-149">This property is read-only.</span></span> <span data-ttu-id="31516-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31516-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="31516-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31516-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="31516-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="31516-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="31516-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31516-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="31516-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31516-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="31516-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="31516-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="31516-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31516-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="31516-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31516-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="31516-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="31516-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="31516-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31516-163">createdDateTime</span></span>|<span data-ttu-id="31516-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31516-164">DateTimeOffset</span></span>|<span data-ttu-id="31516-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="31516-165">DateTime the object was created.</span></span> <span data-ttu-id="31516-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-167">descrição</span><span class="sxs-lookup"><span data-stu-id="31516-167">description</span></span>|<span data-ttu-id="31516-168">String</span><span class="sxs-lookup"><span data-stu-id="31516-168">String</span></span>|<span data-ttu-id="31516-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31516-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31516-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-171">displayName</span><span class="sxs-lookup"><span data-stu-id="31516-171">displayName</span></span>|<span data-ttu-id="31516-172">String</span><span class="sxs-lookup"><span data-stu-id="31516-172">String</span></span>|<span data-ttu-id="31516-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31516-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31516-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-175">versão</span><span class="sxs-lookup"><span data-stu-id="31516-175">version</span></span>|<span data-ttu-id="31516-176">Int32</span><span class="sxs-lookup"><span data-stu-id="31516-176">Int32</span></span>|<span data-ttu-id="31516-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31516-177">Version of the device configuration.</span></span> <span data-ttu-id="31516-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31516-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31516-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="31516-179">omaSettings</span></span>|<span data-ttu-id="31516-180">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31516-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="31516-181">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="31516-181">OMA settings.</span></span> <span data-ttu-id="31516-182">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="31516-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="31516-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="31516-183">Response</span></span>
<span data-ttu-id="31516-184">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31516-184">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31516-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31516-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="31516-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31516-186">Request</span></span>
<span data-ttu-id="31516-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31516-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1294

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="31516-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="31516-188">Response</span></span>
<span data-ttu-id="31516-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31516-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```




