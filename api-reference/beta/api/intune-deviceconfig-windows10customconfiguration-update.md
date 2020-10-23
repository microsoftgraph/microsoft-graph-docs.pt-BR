---
title: Atualizar windows10CustomConfiguration
description: Atualizar as propriedades de um objeto windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d53bb018599e8c326e223c1fd2565e2777cec7b9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727826"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="6b9d4-103">Atualizar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b9d4-103">Update windows10CustomConfiguration</span></span>

<span data-ttu-id="6b9d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b9d4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b9d4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9d4-107">Atualizar as propriedades de um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b9d4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b9d4-108">Prerequisites</span></span>
<span data-ttu-id="6b9d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b9d4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b9d4-111">Permission type</span></span>|<span data-ttu-id="6b9d4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b9d4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b9d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b9d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b9d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b9d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-116">Not supported.</span></span>|
|<span data-ttu-id="6b9d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b9d4-117">Application</span></span>|<span data-ttu-id="6b9d4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b9d4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b9d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b9d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6b9d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9d4-120">Request headers</span></span>
|<span data-ttu-id="6b9d4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b9d4-121">Header</span></span>|<span data-ttu-id="6b9d4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b9d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b9d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b9d4-123">Authorization</span></span>|<span data-ttu-id="6b9d4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b9d4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b9d4-125">Accept</span></span>|<span data-ttu-id="6b9d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b9d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b9d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9d4-127">Request body</span></span>
<span data-ttu-id="6b9d4-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="6b9d4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b9d4-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="6b9d4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b9d4-130">Property</span></span>|<span data-ttu-id="6b9d4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b9d4-131">Type</span></span>|<span data-ttu-id="6b9d4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b9d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9d4-133">id</span><span class="sxs-lookup"><span data-stu-id="6b9d4-133">id</span></span>|<span data-ttu-id="6b9d4-134">String</span><span class="sxs-lookup"><span data-stu-id="6b9d4-134">String</span></span>|<span data-ttu-id="6b9d4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-135">Key of the entity.</span></span> <span data-ttu-id="6b9d4-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b9d4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b9d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b9d4-138">DateTimeOffset</span></span>|<span data-ttu-id="6b9d4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6b9d4-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b9d4-141">roleScopeTagIds</span></span>|<span data-ttu-id="6b9d4-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b9d4-142">String collection</span></span>|<span data-ttu-id="6b9d4-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b9d4-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b9d4-145">supportsScopeTags</span></span>|<span data-ttu-id="6b9d4-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b9d4-146">Boolean</span></span>|<span data-ttu-id="6b9d4-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b9d4-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b9d4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b9d4-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-150">This property is read-only.</span></span> <span data-ttu-id="6b9d4-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6b9d4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6b9d4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6b9d4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6b9d4-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6b9d4-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6b9d4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6b9d4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6b9d4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6b9d4-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6b9d4-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6b9d4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6b9d4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6b9d4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6b9d4-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6b9d4-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b9d4-164">createdDateTime</span></span>|<span data-ttu-id="6b9d4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b9d4-165">DateTimeOffset</span></span>|<span data-ttu-id="6b9d4-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-166">DateTime the object was created.</span></span> <span data-ttu-id="6b9d4-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-168">description</span><span class="sxs-lookup"><span data-stu-id="6b9d4-168">description</span></span>|<span data-ttu-id="6b9d4-169">String</span><span class="sxs-lookup"><span data-stu-id="6b9d4-169">String</span></span>|<span data-ttu-id="6b9d4-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b9d4-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6b9d4-172">displayName</span></span>|<span data-ttu-id="6b9d4-173">String</span><span class="sxs-lookup"><span data-stu-id="6b9d4-173">String</span></span>|<span data-ttu-id="6b9d4-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b9d4-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-176">versão</span><span class="sxs-lookup"><span data-stu-id="6b9d4-176">version</span></span>|<span data-ttu-id="6b9d4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6b9d4-177">Int32</span></span>|<span data-ttu-id="6b9d4-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-178">Version of the device configuration.</span></span> <span data-ttu-id="6b9d4-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b9d4-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="6b9d4-180">omaSettings</span></span>|<span data-ttu-id="6b9d4-181">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d4-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="6b9d4-182">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-182">OMA settings.</span></span> <span data-ttu-id="6b9d4-183">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6b9d4-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9d4-184">Response</span></span>
<span data-ttu-id="6b9d4-185">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-185">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b9d4-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b9d4-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b9d4-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9d4-187">Request</span></span>
<span data-ttu-id="6b9d4-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1243

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
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6b9d4-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9d4-189">Response</span></span>
<span data-ttu-id="6b9d4-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b9d4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1415

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
      "omaUri": "Oma Uri value"
    }
  ]
}
```





