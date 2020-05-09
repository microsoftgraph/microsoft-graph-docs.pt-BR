---
title: Atualizar androidWorkProfileCustomConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7cc14b90daa0b3ea2aa8d220c2859567822bbb3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178868"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="17076-103">Atualizar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="17076-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="17076-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17076-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17076-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17076-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17076-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17076-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17076-107">Atualiza as propriedades de um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="17076-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17076-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17076-108">Prerequisites</span></span>
<span data-ttu-id="17076-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17076-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17076-111">Permission type</span></span>|<span data-ttu-id="17076-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17076-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17076-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17076-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17076-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17076-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17076-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17076-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17076-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17076-116">Not supported.</span></span>|
|<span data-ttu-id="17076-117">Application</span><span class="sxs-lookup"><span data-stu-id="17076-117">Application</span></span>|<span data-ttu-id="17076-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17076-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17076-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17076-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="17076-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17076-120">Request headers</span></span>
|<span data-ttu-id="17076-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17076-121">Header</span></span>|<span data-ttu-id="17076-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17076-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17076-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17076-123">Authorization</span></span>|<span data-ttu-id="17076-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17076-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17076-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17076-125">Accept</span></span>|<span data-ttu-id="17076-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17076-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17076-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17076-127">Request body</span></span>
<span data-ttu-id="17076-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="17076-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="17076-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17076-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="17076-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17076-130">Property</span></span>|<span data-ttu-id="17076-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17076-131">Type</span></span>|<span data-ttu-id="17076-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17076-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17076-133">id</span><span class="sxs-lookup"><span data-stu-id="17076-133">id</span></span>|<span data-ttu-id="17076-134">String</span><span class="sxs-lookup"><span data-stu-id="17076-134">String</span></span>|<span data-ttu-id="17076-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17076-135">Key of the entity.</span></span> <span data-ttu-id="17076-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17076-137">lastModifiedDateTime</span></span>|<span data-ttu-id="17076-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17076-138">DateTimeOffset</span></span>|<span data-ttu-id="17076-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="17076-139">DateTime the object was last modified.</span></span> <span data-ttu-id="17076-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17076-141">roleScopeTagIds</span></span>|<span data-ttu-id="17076-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="17076-142">String collection</span></span>|<span data-ttu-id="17076-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="17076-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17076-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17076-145">supportsScopeTags</span></span>|<span data-ttu-id="17076-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="17076-146">Boolean</span></span>|<span data-ttu-id="17076-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="17076-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17076-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="17076-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17076-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="17076-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17076-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17076-150">This property is read-only.</span></span> <span data-ttu-id="17076-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17076-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="17076-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17076-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="17076-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="17076-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="17076-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17076-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="17076-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17076-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="17076-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="17076-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="17076-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17076-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="17076-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17076-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="17076-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="17076-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="17076-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17076-164">createdDateTime</span></span>|<span data-ttu-id="17076-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17076-165">DateTimeOffset</span></span>|<span data-ttu-id="17076-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="17076-166">DateTime the object was created.</span></span> <span data-ttu-id="17076-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-168">description</span><span class="sxs-lookup"><span data-stu-id="17076-168">description</span></span>|<span data-ttu-id="17076-169">String</span><span class="sxs-lookup"><span data-stu-id="17076-169">String</span></span>|<span data-ttu-id="17076-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17076-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17076-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-172">displayName</span><span class="sxs-lookup"><span data-stu-id="17076-172">displayName</span></span>|<span data-ttu-id="17076-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17076-173">String</span></span>|<span data-ttu-id="17076-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17076-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17076-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-176">versão</span><span class="sxs-lookup"><span data-stu-id="17076-176">version</span></span>|<span data-ttu-id="17076-177">Int32</span><span class="sxs-lookup"><span data-stu-id="17076-177">Int32</span></span>|<span data-ttu-id="17076-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17076-178">Version of the device configuration.</span></span> <span data-ttu-id="17076-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17076-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17076-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="17076-180">omaSettings</span></span>|<span data-ttu-id="17076-181">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="17076-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="17076-182">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="17076-182">OMA settings.</span></span> <span data-ttu-id="17076-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="17076-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="17076-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="17076-184">Response</span></span>
<span data-ttu-id="17076-185">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17076-185">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17076-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17076-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="17076-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17076-187">Request</span></span>
<span data-ttu-id="17076-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17076-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17076-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="17076-189">Response</span></span>
<span data-ttu-id="17076-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17076-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



