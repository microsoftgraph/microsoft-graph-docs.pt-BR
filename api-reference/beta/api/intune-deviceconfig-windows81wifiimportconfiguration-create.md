---
title: Criar windows81WifiImportConfiguration
description: Criar um novo objeto windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2577bc39e1c276b5c2ae9bb3c5955471505e0d0d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946942"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="679d2-103">Criar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="679d2-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="679d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="679d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="679d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="679d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="679d2-106">Criar um novo objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="679d2-106">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="679d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="679d2-107">Prerequisites</span></span>
<span data-ttu-id="679d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="679d2-110">Permission type</span></span>|<span data-ttu-id="679d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="679d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="679d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="679d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="679d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="679d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="679d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="679d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679d2-115">Not supported.</span></span>|
|<span data-ttu-id="679d2-116">Application</span><span class="sxs-lookup"><span data-stu-id="679d2-116">Application</span></span>|<span data-ttu-id="679d2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679d2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="679d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="679d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="679d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="679d2-119">Request headers</span></span>
|<span data-ttu-id="679d2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="679d2-120">Header</span></span>|<span data-ttu-id="679d2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="679d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="679d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="679d2-122">Authorization</span></span>|<span data-ttu-id="679d2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="679d2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="679d2-124">Accept</span></span>|<span data-ttu-id="679d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="679d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="679d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="679d2-126">Request body</span></span>
<span data-ttu-id="679d2-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="679d2-127">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="679d2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="679d2-128">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="679d2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="679d2-129">Property</span></span>|<span data-ttu-id="679d2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="679d2-130">Type</span></span>|<span data-ttu-id="679d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="679d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="679d2-132">id</span><span class="sxs-lookup"><span data-stu-id="679d2-132">id</span></span>|<span data-ttu-id="679d2-133">String</span><span class="sxs-lookup"><span data-stu-id="679d2-133">String</span></span>|<span data-ttu-id="679d2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="679d2-134">Key of the entity.</span></span> <span data-ttu-id="679d2-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="679d2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="679d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679d2-137">DateTimeOffset</span></span>|<span data-ttu-id="679d2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="679d2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="679d2-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="679d2-140">roleScopeTagIds</span></span>|<span data-ttu-id="679d2-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="679d2-141">String collection</span></span>|<span data-ttu-id="679d2-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="679d2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="679d2-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="679d2-144">supportsScopeTags</span></span>|<span data-ttu-id="679d2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="679d2-145">Boolean</span></span>|<span data-ttu-id="679d2-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="679d2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="679d2-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="679d2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="679d2-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="679d2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="679d2-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="679d2-149">This property is read-only.</span></span> <span data-ttu-id="679d2-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="679d2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="679d2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="679d2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="679d2-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="679d2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="679d2-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="679d2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="679d2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="679d2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="679d2-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="679d2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="679d2-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="679d2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="679d2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="679d2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="679d2-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="679d2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="679d2-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="679d2-163">createdDateTime</span></span>|<span data-ttu-id="679d2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679d2-164">DateTimeOffset</span></span>|<span data-ttu-id="679d2-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="679d2-165">DateTime the object was created.</span></span> <span data-ttu-id="679d2-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-167">description</span><span class="sxs-lookup"><span data-stu-id="679d2-167">description</span></span>|<span data-ttu-id="679d2-168">String</span><span class="sxs-lookup"><span data-stu-id="679d2-168">String</span></span>|<span data-ttu-id="679d2-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="679d2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="679d2-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="679d2-171">displayName</span></span>|<span data-ttu-id="679d2-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679d2-172">String</span></span>|<span data-ttu-id="679d2-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="679d2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="679d2-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-175">versão</span><span class="sxs-lookup"><span data-stu-id="679d2-175">version</span></span>|<span data-ttu-id="679d2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="679d2-176">Int32</span></span>|<span data-ttu-id="679d2-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="679d2-177">Version of the device configuration.</span></span> <span data-ttu-id="679d2-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="679d2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="679d2-179">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="679d2-179">payloadFileName</span></span>|<span data-ttu-id="679d2-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679d2-180">String</span></span>|<span data-ttu-id="679d2-181">Nome do arquivo de carga (\*. xml).</span><span class="sxs-lookup"><span data-stu-id="679d2-181">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="679d2-182">ProfileName</span><span class="sxs-lookup"><span data-stu-id="679d2-182">profileName</span></span>|<span data-ttu-id="679d2-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="679d2-183">String</span></span>|<span data-ttu-id="679d2-184">Nome do perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="679d2-184">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="679d2-185">payload</span><span class="sxs-lookup"><span data-stu-id="679d2-185">payload</span></span>|<span data-ttu-id="679d2-186">Binária</span><span class="sxs-lookup"><span data-stu-id="679d2-186">Binary</span></span>|<span data-ttu-id="679d2-187">Carga.</span><span class="sxs-lookup"><span data-stu-id="679d2-187">Payload.</span></span> <span data-ttu-id="679d2-188">(Matriz de bytes codificados por UTF8).</span><span class="sxs-lookup"><span data-stu-id="679d2-188">(UTF8 encoded byte array).</span></span> <span data-ttu-id="679d2-189">Este é o arquivo XML salvo no dispositivo que você usou para se conectar ao ponto de extremidade Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="679d2-189">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="679d2-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="679d2-190">Response</span></span>
<span data-ttu-id="679d2-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="679d2-191">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679d2-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="679d2-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="679d2-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679d2-193">Request</span></span>
<span data-ttu-id="679d2-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="679d2-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="679d2-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="679d2-195">Response</span></span>
<span data-ttu-id="679d2-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="679d2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





