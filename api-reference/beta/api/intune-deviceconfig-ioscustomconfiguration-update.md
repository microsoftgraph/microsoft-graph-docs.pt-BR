---
title: Atualizar iosCustomConfiguration
description: Atualizar as propriedades de um objeto iosCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c3d9fd1076373eff4549826d18f018d84ac0e1c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949107"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="76592-103">Atualizar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="76592-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="76592-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76592-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76592-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76592-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76592-106">Atualizar as propriedades de um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76592-106">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76592-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76592-107">Prerequisites</span></span>
<span data-ttu-id="76592-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76592-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76592-110">Permission type</span></span>|<span data-ttu-id="76592-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76592-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76592-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76592-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76592-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76592-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76592-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76592-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76592-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76592-115">Not supported.</span></span>|
|<span data-ttu-id="76592-116">Application</span><span class="sxs-lookup"><span data-stu-id="76592-116">Application</span></span>|<span data-ttu-id="76592-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76592-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76592-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76592-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="76592-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76592-119">Request headers</span></span>
|<span data-ttu-id="76592-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76592-120">Header</span></span>|<span data-ttu-id="76592-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76592-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76592-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76592-122">Authorization</span></span>|<span data-ttu-id="76592-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76592-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76592-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76592-124">Accept</span></span>|<span data-ttu-id="76592-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76592-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76592-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76592-126">Request body</span></span>
<span data-ttu-id="76592-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76592-127">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="76592-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76592-128">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="76592-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76592-129">Property</span></span>|<span data-ttu-id="76592-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="76592-130">Type</span></span>|<span data-ttu-id="76592-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="76592-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76592-132">id</span><span class="sxs-lookup"><span data-stu-id="76592-132">id</span></span>|<span data-ttu-id="76592-133">String</span><span class="sxs-lookup"><span data-stu-id="76592-133">String</span></span>|<span data-ttu-id="76592-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76592-134">Key of the entity.</span></span> <span data-ttu-id="76592-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76592-136">lastModifiedDateTime</span></span>|<span data-ttu-id="76592-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76592-137">DateTimeOffset</span></span>|<span data-ttu-id="76592-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76592-138">DateTime the object was last modified.</span></span> <span data-ttu-id="76592-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76592-140">roleScopeTagIds</span></span>|<span data-ttu-id="76592-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76592-141">String collection</span></span>|<span data-ttu-id="76592-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="76592-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76592-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76592-144">supportsScopeTags</span></span>|<span data-ttu-id="76592-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="76592-145">Boolean</span></span>|<span data-ttu-id="76592-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="76592-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76592-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="76592-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76592-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="76592-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76592-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76592-149">This property is read-only.</span></span> <span data-ttu-id="76592-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76592-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76592-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76592-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76592-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="76592-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76592-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76592-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76592-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76592-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76592-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="76592-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76592-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76592-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76592-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76592-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76592-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="76592-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76592-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76592-163">createdDateTime</span></span>|<span data-ttu-id="76592-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76592-164">DateTimeOffset</span></span>|<span data-ttu-id="76592-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76592-165">DateTime the object was created.</span></span> <span data-ttu-id="76592-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-167">description</span><span class="sxs-lookup"><span data-stu-id="76592-167">description</span></span>|<span data-ttu-id="76592-168">String</span><span class="sxs-lookup"><span data-stu-id="76592-168">String</span></span>|<span data-ttu-id="76592-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76592-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76592-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-171">displayName</span><span class="sxs-lookup"><span data-stu-id="76592-171">displayName</span></span>|<span data-ttu-id="76592-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76592-172">String</span></span>|<span data-ttu-id="76592-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76592-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76592-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-175">versão</span><span class="sxs-lookup"><span data-stu-id="76592-175">version</span></span>|<span data-ttu-id="76592-176">Int32</span><span class="sxs-lookup"><span data-stu-id="76592-176">Int32</span></span>|<span data-ttu-id="76592-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76592-177">Version of the device configuration.</span></span> <span data-ttu-id="76592-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76592-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76592-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="76592-179">payloadName</span></span>|<span data-ttu-id="76592-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="76592-180">String</span></span>|<span data-ttu-id="76592-181">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76592-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="76592-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="76592-182">payloadFileName</span></span>|<span data-ttu-id="76592-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76592-183">String</span></span>|<span data-ttu-id="76592-184">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="76592-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="76592-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="76592-185">\*.xml).</span></span>|
|<span data-ttu-id="76592-186">payload</span><span class="sxs-lookup"><span data-stu-id="76592-186">payload</span></span>|<span data-ttu-id="76592-187">Binária</span><span class="sxs-lookup"><span data-stu-id="76592-187">Binary</span></span>|<span data-ttu-id="76592-188">Carga.</span><span class="sxs-lookup"><span data-stu-id="76592-188">Payload.</span></span> <span data-ttu-id="76592-189">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="76592-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="76592-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="76592-190">Response</span></span>
<span data-ttu-id="76592-191">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76592-191">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76592-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76592-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="76592-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76592-193">Request</span></span>
<span data-ttu-id="76592-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76592-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76592-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="76592-195">Response</span></span>
<span data-ttu-id="76592-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76592-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





