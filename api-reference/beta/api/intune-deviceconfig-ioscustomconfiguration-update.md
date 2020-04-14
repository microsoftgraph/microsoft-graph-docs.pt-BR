---
title: Atualizar iosCustomConfiguration
description: Atualizar as propriedades de um objeto iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b9ccc85482bbf32ea8ba403e81f7ccadce0e353
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432864"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="87340-103">Atualizar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="87340-103">Update iosCustomConfiguration</span></span>

<span data-ttu-id="87340-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87340-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87340-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87340-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87340-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87340-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87340-107">Atualizar as propriedades de um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87340-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87340-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87340-108">Prerequisites</span></span>
<span data-ttu-id="87340-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87340-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87340-111">Permission type</span></span>|<span data-ttu-id="87340-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87340-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87340-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87340-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87340-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87340-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87340-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87340-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87340-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87340-116">Not supported.</span></span>|
|<span data-ttu-id="87340-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87340-117">Application</span></span>|<span data-ttu-id="87340-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87340-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87340-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87340-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="87340-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87340-120">Request headers</span></span>
|<span data-ttu-id="87340-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87340-121">Header</span></span>|<span data-ttu-id="87340-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87340-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87340-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87340-123">Authorization</span></span>|<span data-ttu-id="87340-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87340-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87340-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87340-125">Accept</span></span>|<span data-ttu-id="87340-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87340-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87340-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87340-127">Request body</span></span>
<span data-ttu-id="87340-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87340-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="87340-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87340-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="87340-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87340-130">Property</span></span>|<span data-ttu-id="87340-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="87340-131">Type</span></span>|<span data-ttu-id="87340-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="87340-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87340-133">id</span><span class="sxs-lookup"><span data-stu-id="87340-133">id</span></span>|<span data-ttu-id="87340-134">String</span><span class="sxs-lookup"><span data-stu-id="87340-134">String</span></span>|<span data-ttu-id="87340-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87340-135">Key of the entity.</span></span> <span data-ttu-id="87340-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87340-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87340-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87340-138">DateTimeOffset</span></span>|<span data-ttu-id="87340-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="87340-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87340-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87340-141">roleScopeTagIds</span></span>|<span data-ttu-id="87340-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="87340-142">String collection</span></span>|<span data-ttu-id="87340-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="87340-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87340-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87340-145">supportsScopeTags</span></span>|<span data-ttu-id="87340-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="87340-146">Boolean</span></span>|<span data-ttu-id="87340-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="87340-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87340-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="87340-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87340-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="87340-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87340-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87340-150">This property is read-only.</span></span> <span data-ttu-id="87340-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87340-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="87340-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87340-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="87340-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="87340-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="87340-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87340-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="87340-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87340-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="87340-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="87340-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="87340-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87340-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="87340-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87340-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="87340-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="87340-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="87340-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87340-164">createdDateTime</span></span>|<span data-ttu-id="87340-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87340-165">DateTimeOffset</span></span>|<span data-ttu-id="87340-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="87340-166">DateTime the object was created.</span></span> <span data-ttu-id="87340-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-168">description</span><span class="sxs-lookup"><span data-stu-id="87340-168">description</span></span>|<span data-ttu-id="87340-169">String</span><span class="sxs-lookup"><span data-stu-id="87340-169">String</span></span>|<span data-ttu-id="87340-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87340-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87340-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-172">displayName</span><span class="sxs-lookup"><span data-stu-id="87340-172">displayName</span></span>|<span data-ttu-id="87340-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87340-173">String</span></span>|<span data-ttu-id="87340-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87340-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87340-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-176">versão</span><span class="sxs-lookup"><span data-stu-id="87340-176">version</span></span>|<span data-ttu-id="87340-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87340-177">Int32</span></span>|<span data-ttu-id="87340-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87340-178">Version of the device configuration.</span></span> <span data-ttu-id="87340-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87340-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87340-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="87340-180">payloadName</span></span>|<span data-ttu-id="87340-181">String</span><span class="sxs-lookup"><span data-stu-id="87340-181">String</span></span>|<span data-ttu-id="87340-182">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="87340-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="87340-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="87340-183">payloadFileName</span></span>|<span data-ttu-id="87340-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87340-184">String</span></span>|<span data-ttu-id="87340-185">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="87340-185">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="87340-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="87340-186">\*.xml).</span></span>|
|<span data-ttu-id="87340-187">payload</span><span class="sxs-lookup"><span data-stu-id="87340-187">payload</span></span>|<span data-ttu-id="87340-188">Binária</span><span class="sxs-lookup"><span data-stu-id="87340-188">Binary</span></span>|<span data-ttu-id="87340-189">Carga.</span><span class="sxs-lookup"><span data-stu-id="87340-189">Payload.</span></span> <span data-ttu-id="87340-190">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="87340-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="87340-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="87340-191">Response</span></span>
<span data-ttu-id="87340-192">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87340-192">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87340-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87340-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="87340-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87340-194">Request</span></span>
<span data-ttu-id="87340-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87340-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1144

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="87340-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="87340-196">Response</span></span>
<span data-ttu-id="87340-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87340-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1316

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



