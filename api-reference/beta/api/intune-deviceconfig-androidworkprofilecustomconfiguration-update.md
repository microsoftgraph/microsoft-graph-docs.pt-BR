---
title: Atualizar androidWorkProfileCustomConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8910af93e9431768935ee3a5505f1d62707a854a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059030"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="aad74-103">Atualizar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="aad74-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="aad74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aad74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aad74-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aad74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aad74-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aad74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aad74-107">Atualiza as propriedades de um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aad74-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aad74-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aad74-108">Prerequisites</span></span>
<span data-ttu-id="aad74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aad74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aad74-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aad74-111">Permission type</span></span>|<span data-ttu-id="aad74-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aad74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aad74-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aad74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aad74-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aad74-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aad74-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aad74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aad74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aad74-116">Not supported.</span></span>|
|<span data-ttu-id="aad74-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aad74-117">Application</span></span>|<span data-ttu-id="aad74-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aad74-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aad74-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aad74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aad74-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aad74-120">Request headers</span></span>
|<span data-ttu-id="aad74-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aad74-121">Header</span></span>|<span data-ttu-id="aad74-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aad74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aad74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aad74-123">Authorization</span></span>|<span data-ttu-id="aad74-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aad74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aad74-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aad74-125">Accept</span></span>|<span data-ttu-id="aad74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aad74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aad74-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aad74-127">Request body</span></span>
<span data-ttu-id="aad74-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aad74-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="aad74-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aad74-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="aad74-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aad74-130">Property</span></span>|<span data-ttu-id="aad74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aad74-131">Type</span></span>|<span data-ttu-id="aad74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aad74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aad74-133">id</span><span class="sxs-lookup"><span data-stu-id="aad74-133">id</span></span>|<span data-ttu-id="aad74-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad74-134">String</span></span>|<span data-ttu-id="aad74-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aad74-135">Key of the entity.</span></span> <span data-ttu-id="aad74-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aad74-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aad74-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad74-138">DateTimeOffset</span></span>|<span data-ttu-id="aad74-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aad74-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aad74-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aad74-141">roleScopeTagIds</span></span>|<span data-ttu-id="aad74-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad74-142">String collection</span></span>|<span data-ttu-id="aad74-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aad74-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aad74-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aad74-145">supportsScopeTags</span></span>|<span data-ttu-id="aad74-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="aad74-146">Boolean</span></span>|<span data-ttu-id="aad74-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="aad74-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aad74-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="aad74-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aad74-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="aad74-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aad74-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad74-150">This property is read-only.</span></span> <span data-ttu-id="aad74-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aad74-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aad74-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aad74-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aad74-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="aad74-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aad74-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aad74-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aad74-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aad74-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aad74-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="aad74-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aad74-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aad74-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aad74-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aad74-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aad74-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="aad74-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aad74-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aad74-164">createdDateTime</span></span>|<span data-ttu-id="aad74-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad74-165">DateTimeOffset</span></span>|<span data-ttu-id="aad74-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aad74-166">DateTime the object was created.</span></span> <span data-ttu-id="aad74-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-168">description</span><span class="sxs-lookup"><span data-stu-id="aad74-168">description</span></span>|<span data-ttu-id="aad74-169">String</span><span class="sxs-lookup"><span data-stu-id="aad74-169">String</span></span>|<span data-ttu-id="aad74-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad74-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aad74-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-172">displayName</span><span class="sxs-lookup"><span data-stu-id="aad74-172">displayName</span></span>|<span data-ttu-id="aad74-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad74-173">String</span></span>|<span data-ttu-id="aad74-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad74-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aad74-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-176">versão</span><span class="sxs-lookup"><span data-stu-id="aad74-176">version</span></span>|<span data-ttu-id="aad74-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aad74-177">Int32</span></span>|<span data-ttu-id="aad74-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad74-178">Version of the device configuration.</span></span> <span data-ttu-id="aad74-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aad74-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="aad74-180">omaSettings</span></span>|<span data-ttu-id="aad74-181">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aad74-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="aad74-182">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="aad74-182">OMA settings.</span></span> <span data-ttu-id="aad74-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="aad74-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="aad74-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="aad74-184">Response</span></span>
<span data-ttu-id="aad74-185">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aad74-185">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aad74-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aad74-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="aad74-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aad74-187">Request</span></span>
<span data-ttu-id="aad74-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aad74-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1252

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="aad74-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="aad74-189">Response</span></span>
<span data-ttu-id="aad74-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aad74-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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






