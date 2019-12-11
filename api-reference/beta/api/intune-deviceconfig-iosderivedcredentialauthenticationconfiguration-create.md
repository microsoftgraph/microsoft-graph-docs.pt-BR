---
title: Criar iosDerivedCredentialAuthenticationConfiguration
description: Criar um novo objeto iosDerivedCredentialAuthenticationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c6ae79ffdbda8b1cbd96bcd57f940c1e15ee252
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949100"
---
# <a name="create-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="73317-103">Criar iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="73317-103">Create iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="73317-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73317-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73317-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73317-106">Criar um novo objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73317-106">Create a new [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73317-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73317-107">Prerequisites</span></span>
<span data-ttu-id="73317-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73317-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73317-110">Permission type</span></span>|<span data-ttu-id="73317-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73317-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73317-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73317-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73317-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73317-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73317-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73317-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73317-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73317-115">Not supported.</span></span>|
|<span data-ttu-id="73317-116">Application</span><span class="sxs-lookup"><span data-stu-id="73317-116">Application</span></span>|<span data-ttu-id="73317-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73317-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73317-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73317-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73317-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73317-119">Request headers</span></span>
|<span data-ttu-id="73317-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73317-120">Header</span></span>|<span data-ttu-id="73317-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73317-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73317-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73317-122">Authorization</span></span>|<span data-ttu-id="73317-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73317-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73317-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73317-124">Accept</span></span>|<span data-ttu-id="73317-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73317-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73317-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73317-126">Request body</span></span>
<span data-ttu-id="73317-127">No corpo da solicitação, forneça uma representação JSON do objeto iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73317-127">In the request body, supply a JSON representation for the iosDerivedCredentialAuthenticationConfiguration object.</span></span>

<span data-ttu-id="73317-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73317-128">The following table shows the properties that are required when you create the iosDerivedCredentialAuthenticationConfiguration.</span></span>

|<span data-ttu-id="73317-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73317-129">Property</span></span>|<span data-ttu-id="73317-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73317-130">Type</span></span>|<span data-ttu-id="73317-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73317-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73317-132">id</span><span class="sxs-lookup"><span data-stu-id="73317-132">id</span></span>|<span data-ttu-id="73317-133">String</span><span class="sxs-lookup"><span data-stu-id="73317-133">String</span></span>|<span data-ttu-id="73317-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73317-134">Key of the entity.</span></span> <span data-ttu-id="73317-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73317-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73317-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73317-137">DateTimeOffset</span></span>|<span data-ttu-id="73317-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="73317-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73317-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73317-140">roleScopeTagIds</span></span>|<span data-ttu-id="73317-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73317-141">String collection</span></span>|<span data-ttu-id="73317-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73317-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73317-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73317-144">supportsScopeTags</span></span>|<span data-ttu-id="73317-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="73317-145">Boolean</span></span>|<span data-ttu-id="73317-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="73317-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73317-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="73317-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73317-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="73317-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73317-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73317-149">This property is read-only.</span></span> <span data-ttu-id="73317-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73317-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="73317-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73317-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="73317-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="73317-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="73317-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73317-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="73317-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73317-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="73317-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="73317-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="73317-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73317-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="73317-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73317-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="73317-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="73317-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="73317-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73317-163">createdDateTime</span></span>|<span data-ttu-id="73317-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73317-164">DateTimeOffset</span></span>|<span data-ttu-id="73317-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="73317-165">DateTime the object was created.</span></span> <span data-ttu-id="73317-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-167">description</span><span class="sxs-lookup"><span data-stu-id="73317-167">description</span></span>|<span data-ttu-id="73317-168">String</span><span class="sxs-lookup"><span data-stu-id="73317-168">String</span></span>|<span data-ttu-id="73317-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73317-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73317-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-171">displayName</span><span class="sxs-lookup"><span data-stu-id="73317-171">displayName</span></span>|<span data-ttu-id="73317-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73317-172">String</span></span>|<span data-ttu-id="73317-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73317-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73317-174">Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73317-175">versão</span><span class="sxs-lookup"><span data-stu-id="73317-175">version</span></span>|<span data-ttu-id="73317-176">Int32</span><span class="sxs-lookup"><span data-stu-id="73317-176">Int32</span></span>|<span data-ttu-id="73317-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73317-177">Version of the device configuration.</span></span> <span data-ttu-id="73317-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73317-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="73317-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="73317-179">Response</span></span>
<span data-ttu-id="73317-180">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73317-180">If successful, this method returns a `201 Created` response code and a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73317-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73317-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="73317-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73317-182">Request</span></span>
<span data-ttu-id="73317-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73317-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="73317-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="73317-184">Response</span></span>
<span data-ttu-id="73317-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73317-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1222

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
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
  "version": 7
}
```





