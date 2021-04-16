---
title: Atualizar windows10CustomConfiguration
description: Atualizar as propriedades de um objeto windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84a014bbd73a67414eb987bd34ff989276140fce
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866472"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="5e92f-103">Atualizar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e92f-103">Update windows10CustomConfiguration</span></span>

<span data-ttu-id="5e92f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e92f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e92f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e92f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e92f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e92f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e92f-107">Atualizar as propriedades de um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e92f-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e92f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e92f-108">Prerequisites</span></span>
<span data-ttu-id="5e92f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e92f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e92f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e92f-111">Permission type</span></span>|<span data-ttu-id="5e92f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e92f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e92f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e92f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e92f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e92f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e92f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e92f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e92f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e92f-116">Not supported.</span></span>|
|<span data-ttu-id="5e92f-117">Application</span><span class="sxs-lookup"><span data-stu-id="5e92f-117">Application</span></span>|<span data-ttu-id="5e92f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e92f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e92f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e92f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5e92f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e92f-120">Request headers</span></span>
|<span data-ttu-id="5e92f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e92f-121">Header</span></span>|<span data-ttu-id="5e92f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e92f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e92f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e92f-123">Authorization</span></span>|<span data-ttu-id="5e92f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e92f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e92f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e92f-125">Accept</span></span>|<span data-ttu-id="5e92f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e92f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e92f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e92f-127">Request body</span></span>
<span data-ttu-id="5e92f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e92f-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="5e92f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e92f-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="5e92f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e92f-130">Property</span></span>|<span data-ttu-id="5e92f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e92f-131">Type</span></span>|<span data-ttu-id="5e92f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e92f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e92f-133">id</span><span class="sxs-lookup"><span data-stu-id="5e92f-133">id</span></span>|<span data-ttu-id="5e92f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e92f-134">String</span></span>|<span data-ttu-id="5e92f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e92f-135">Key of the entity.</span></span> <span data-ttu-id="5e92f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e92f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5e92f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e92f-138">DateTimeOffset</span></span>|<span data-ttu-id="5e92f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5e92f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5e92f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e92f-141">roleScopeTagIds</span></span>|<span data-ttu-id="5e92f-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5e92f-142">String collection</span></span>|<span data-ttu-id="5e92f-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="5e92f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5e92f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5e92f-145">supportsScopeTags</span></span>|<span data-ttu-id="5e92f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e92f-146">Boolean</span></span>|<span data-ttu-id="5e92f-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5e92f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5e92f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5e92f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5e92f-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5e92f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5e92f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e92f-150">This property is read-only.</span></span> <span data-ttu-id="5e92f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5e92f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5e92f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5e92f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5e92f-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="5e92f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5e92f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5e92f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5e92f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5e92f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5e92f-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="5e92f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5e92f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5e92f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5e92f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5e92f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5e92f-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="5e92f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5e92f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e92f-164">createdDateTime</span></span>|<span data-ttu-id="5e92f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e92f-165">DateTimeOffset</span></span>|<span data-ttu-id="5e92f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5e92f-166">DateTime the object was created.</span></span> <span data-ttu-id="5e92f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-168">description</span><span class="sxs-lookup"><span data-stu-id="5e92f-168">description</span></span>|<span data-ttu-id="5e92f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e92f-169">String</span></span>|<span data-ttu-id="5e92f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e92f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5e92f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5e92f-172">displayName</span></span>|<span data-ttu-id="5e92f-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e92f-173">String</span></span>|<span data-ttu-id="5e92f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e92f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5e92f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-176">versão</span><span class="sxs-lookup"><span data-stu-id="5e92f-176">version</span></span>|<span data-ttu-id="5e92f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5e92f-177">Int32</span></span>|<span data-ttu-id="5e92f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e92f-178">Version of the device configuration.</span></span> <span data-ttu-id="5e92f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e92f-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="5e92f-180">omaSettings</span></span>|<span data-ttu-id="5e92f-181">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5e92f-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="5e92f-182">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="5e92f-182">OMA settings.</span></span> <span data-ttu-id="5e92f-183">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="5e92f-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5e92f-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e92f-184">Response</span></span>
<span data-ttu-id="5e92f-185">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e92f-185">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e92f-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e92f-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e92f-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e92f-187">Request</span></span>
<span data-ttu-id="5e92f-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e92f-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "secretReferenceValueId": "Secret Reference Value Id value",
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5e92f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e92f-189">Response</span></span>
<span data-ttu-id="5e92f-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e92f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "secretReferenceValueId": "Secret Reference Value Id value",
      "isEncrypted": true
    }
  ]
}
```




