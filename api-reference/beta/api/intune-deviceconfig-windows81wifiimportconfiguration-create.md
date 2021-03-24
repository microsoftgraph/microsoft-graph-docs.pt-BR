---
title: Criar windows81WifiImportConfiguration
description: Crie um novo objeto windows81WifiImportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3d79634df501a9f9976d76c0ecaf6621b3d834
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136969"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="83fb8-103">Criar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="83fb8-103">Create windows81WifiImportConfiguration</span></span>

<span data-ttu-id="83fb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83fb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83fb8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83fb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83fb8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83fb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83fb8-107">Crie um novo [objeto windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83fb8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83fb8-108">Prerequisites</span></span>
<span data-ttu-id="83fb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83fb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83fb8-111">Permission type</span></span>|<span data-ttu-id="83fb8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83fb8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83fb8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83fb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83fb8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83fb8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83fb8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83fb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83fb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83fb8-116">Not supported.</span></span>|
|<span data-ttu-id="83fb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83fb8-117">Application</span></span>|<span data-ttu-id="83fb8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83fb8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83fb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83fb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83fb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83fb8-120">Request headers</span></span>
|<span data-ttu-id="83fb8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83fb8-121">Header</span></span>|<span data-ttu-id="83fb8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83fb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83fb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83fb8-123">Authorization</span></span>|<span data-ttu-id="83fb8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83fb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83fb8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83fb8-125">Accept</span></span>|<span data-ttu-id="83fb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83fb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83fb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83fb8-127">Request body</span></span>
<span data-ttu-id="83fb8-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="83fb8-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="83fb8-129">A tabela a seguir mostra as propriedades necessárias ao criar o windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="83fb8-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="83fb8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83fb8-130">Property</span></span>|<span data-ttu-id="83fb8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83fb8-131">Type</span></span>|<span data-ttu-id="83fb8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83fb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83fb8-133">id</span><span class="sxs-lookup"><span data-stu-id="83fb8-133">id</span></span>|<span data-ttu-id="83fb8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-134">String</span></span>|<span data-ttu-id="83fb8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83fb8-135">Key of the entity.</span></span> <span data-ttu-id="83fb8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83fb8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83fb8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83fb8-138">DateTimeOffset</span></span>|<span data-ttu-id="83fb8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="83fb8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83fb8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83fb8-141">roleScopeTagIds</span></span>|<span data-ttu-id="83fb8-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-142">String collection</span></span>|<span data-ttu-id="83fb8-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="83fb8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83fb8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83fb8-145">supportsScopeTags</span></span>|<span data-ttu-id="83fb8-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="83fb8-146">Boolean</span></span>|<span data-ttu-id="83fb8-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="83fb8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83fb8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="83fb8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83fb8-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="83fb8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83fb8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83fb8-150">This property is read-only.</span></span> <span data-ttu-id="83fb8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83fb8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83fb8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83fb8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83fb8-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="83fb8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83fb8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83fb8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83fb8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83fb8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83fb8-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="83fb8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83fb8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83fb8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83fb8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83fb8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83fb8-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="83fb8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83fb8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83fb8-164">createdDateTime</span></span>|<span data-ttu-id="83fb8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83fb8-165">DateTimeOffset</span></span>|<span data-ttu-id="83fb8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="83fb8-166">DateTime the object was created.</span></span> <span data-ttu-id="83fb8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-168">descrição</span><span class="sxs-lookup"><span data-stu-id="83fb8-168">description</span></span>|<span data-ttu-id="83fb8-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-169">String</span></span>|<span data-ttu-id="83fb8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83fb8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83fb8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="83fb8-172">displayName</span></span>|<span data-ttu-id="83fb8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-173">String</span></span>|<span data-ttu-id="83fb8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83fb8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83fb8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-176">versão</span><span class="sxs-lookup"><span data-stu-id="83fb8-176">version</span></span>|<span data-ttu-id="83fb8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="83fb8-177">Int32</span></span>|<span data-ttu-id="83fb8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83fb8-178">Version of the device configuration.</span></span> <span data-ttu-id="83fb8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83fb8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83fb8-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="83fb8-180">payloadFileName</span></span>|<span data-ttu-id="83fb8-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-181">String</span></span>|<span data-ttu-id="83fb8-182">Nome do arquivo de carga (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="83fb8-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="83fb8-183">profileName</span><span class="sxs-lookup"><span data-stu-id="83fb8-183">profileName</span></span>|<span data-ttu-id="83fb8-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83fb8-184">String</span></span>|<span data-ttu-id="83fb8-185">Nome de perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="83fb8-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="83fb8-186">payload</span><span class="sxs-lookup"><span data-stu-id="83fb8-186">payload</span></span>|<span data-ttu-id="83fb8-187">Binária</span><span class="sxs-lookup"><span data-stu-id="83fb8-187">Binary</span></span>|<span data-ttu-id="83fb8-188">Carga.</span><span class="sxs-lookup"><span data-stu-id="83fb8-188">Payload.</span></span> <span data-ttu-id="83fb8-189">(matriz de byte codificado UTF8).</span><span class="sxs-lookup"><span data-stu-id="83fb8-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="83fb8-190">Este é o arquivo XML salvo no dispositivo que você usou para se conectar ao Wi-Fi ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="83fb8-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="83fb8-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="83fb8-191">Response</span></span>
<span data-ttu-id="83fb8-192">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83fb8-192">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83fb8-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83fb8-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="83fb8-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83fb8-194">Request</span></span>
<span data-ttu-id="83fb8-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83fb8-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83fb8-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="83fb8-196">Response</span></span>
<span data-ttu-id="83fb8-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83fb8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




