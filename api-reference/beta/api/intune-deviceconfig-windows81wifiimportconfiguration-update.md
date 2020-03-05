---
title: Atualizar windows81WifiImportConfiguration
description: Atualiza as propriedades de um objeto windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e012d64f819a2ad84689abceefde1190da7e0f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476416"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="95b46-103">Atualizar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="95b46-103">Update windows81WifiImportConfiguration</span></span>

<span data-ttu-id="95b46-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95b46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95b46-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95b46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95b46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95b46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b46-107">Atualiza as propriedades de um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95b46-107">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95b46-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95b46-108">Prerequisites</span></span>
<span data-ttu-id="95b46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95b46-111">Permission type</span></span>|<span data-ttu-id="95b46-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95b46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95b46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95b46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95b46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95b46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95b46-116">Not supported.</span></span>|
|<span data-ttu-id="95b46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95b46-117">Application</span></span>|<span data-ttu-id="95b46-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b46-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95b46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95b46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95b46-120">Request headers</span></span>
|<span data-ttu-id="95b46-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95b46-121">Header</span></span>|<span data-ttu-id="95b46-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95b46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95b46-123">Authorization</span></span>|<span data-ttu-id="95b46-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95b46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b46-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95b46-125">Accept</span></span>|<span data-ttu-id="95b46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95b46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95b46-127">Request body</span></span>
<span data-ttu-id="95b46-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95b46-128">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="95b46-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95b46-129">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="95b46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95b46-130">Property</span></span>|<span data-ttu-id="95b46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95b46-131">Type</span></span>|<span data-ttu-id="95b46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b46-133">id</span><span class="sxs-lookup"><span data-stu-id="95b46-133">id</span></span>|<span data-ttu-id="95b46-134">String</span><span class="sxs-lookup"><span data-stu-id="95b46-134">String</span></span>|<span data-ttu-id="95b46-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95b46-135">Key of the entity.</span></span> <span data-ttu-id="95b46-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95b46-137">lastModifiedDateTime</span></span>|<span data-ttu-id="95b46-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b46-138">DateTimeOffset</span></span>|<span data-ttu-id="95b46-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95b46-139">DateTime the object was last modified.</span></span> <span data-ttu-id="95b46-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95b46-141">roleScopeTagIds</span></span>|<span data-ttu-id="95b46-142">String collection</span><span class="sxs-lookup"><span data-stu-id="95b46-142">String collection</span></span>|<span data-ttu-id="95b46-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="95b46-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95b46-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95b46-145">supportsScopeTags</span></span>|<span data-ttu-id="95b46-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b46-146">Boolean</span></span>|<span data-ttu-id="95b46-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="95b46-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95b46-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="95b46-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95b46-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="95b46-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95b46-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95b46-150">This property is read-only.</span></span> <span data-ttu-id="95b46-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95b46-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="95b46-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95b46-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="95b46-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="95b46-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="95b46-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95b46-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="95b46-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95b46-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="95b46-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="95b46-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="95b46-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95b46-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="95b46-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95b46-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="95b46-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="95b46-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="95b46-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95b46-164">createdDateTime</span></span>|<span data-ttu-id="95b46-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b46-165">DateTimeOffset</span></span>|<span data-ttu-id="95b46-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95b46-166">DateTime the object was created.</span></span> <span data-ttu-id="95b46-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-168">description</span><span class="sxs-lookup"><span data-stu-id="95b46-168">description</span></span>|<span data-ttu-id="95b46-169">String</span><span class="sxs-lookup"><span data-stu-id="95b46-169">String</span></span>|<span data-ttu-id="95b46-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95b46-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95b46-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-172">displayName</span><span class="sxs-lookup"><span data-stu-id="95b46-172">displayName</span></span>|<span data-ttu-id="95b46-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b46-173">String</span></span>|<span data-ttu-id="95b46-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95b46-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95b46-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-176">versão</span><span class="sxs-lookup"><span data-stu-id="95b46-176">version</span></span>|<span data-ttu-id="95b46-177">Int32</span><span class="sxs-lookup"><span data-stu-id="95b46-177">Int32</span></span>|<span data-ttu-id="95b46-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95b46-178">Version of the device configuration.</span></span> <span data-ttu-id="95b46-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95b46-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95b46-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="95b46-180">payloadFileName</span></span>|<span data-ttu-id="95b46-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b46-181">String</span></span>|<span data-ttu-id="95b46-182">Nome do arquivo de carga (\*. xml).</span><span class="sxs-lookup"><span data-stu-id="95b46-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="95b46-183">ProfileName</span><span class="sxs-lookup"><span data-stu-id="95b46-183">profileName</span></span>|<span data-ttu-id="95b46-184">String</span><span class="sxs-lookup"><span data-stu-id="95b46-184">String</span></span>|<span data-ttu-id="95b46-185">Nome do perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="95b46-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="95b46-186">payload</span><span class="sxs-lookup"><span data-stu-id="95b46-186">payload</span></span>|<span data-ttu-id="95b46-187">Binária</span><span class="sxs-lookup"><span data-stu-id="95b46-187">Binary</span></span>|<span data-ttu-id="95b46-188">Carga.</span><span class="sxs-lookup"><span data-stu-id="95b46-188">Payload.</span></span> <span data-ttu-id="95b46-189">(Matriz de bytes codificados por UTF8).</span><span class="sxs-lookup"><span data-stu-id="95b46-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="95b46-190">Este é o arquivo XML salvo no dispositivo que você usou para se conectar ao ponto de extremidade Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="95b46-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="95b46-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="95b46-191">Response</span></span>
<span data-ttu-id="95b46-192">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95b46-192">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b46-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95b46-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="95b46-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95b46-194">Request</span></span>
<span data-ttu-id="95b46-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95b46-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1154

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="95b46-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="95b46-196">Response</span></span>
<span data-ttu-id="95b46-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95b46-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1326

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





