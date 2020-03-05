---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60a29103f588950bd1f468681a512b71bda82057
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442429"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="13e09-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="13e09-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="13e09-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13e09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13e09-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13e09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13e09-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13e09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13e09-107">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e09-107">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13e09-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13e09-108">Prerequisites</span></span>
<span data-ttu-id="13e09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13e09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13e09-111">Permission type</span></span>|<span data-ttu-id="13e09-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13e09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13e09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13e09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13e09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13e09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13e09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13e09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13e09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13e09-116">Not supported.</span></span>|
|<span data-ttu-id="13e09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13e09-117">Application</span></span>|<span data-ttu-id="13e09-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13e09-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13e09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13e09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13e09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13e09-120">Request headers</span></span>
|<span data-ttu-id="13e09-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13e09-121">Header</span></span>|<span data-ttu-id="13e09-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13e09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13e09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13e09-123">Authorization</span></span>|<span data-ttu-id="13e09-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13e09-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13e09-125">Accept</span></span>|<span data-ttu-id="13e09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13e09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13e09-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13e09-127">Request body</span></span>
<span data-ttu-id="13e09-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="13e09-128">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="13e09-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="13e09-129">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="13e09-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13e09-130">Property</span></span>|<span data-ttu-id="13e09-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13e09-131">Type</span></span>|<span data-ttu-id="13e09-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13e09-133">id</span><span class="sxs-lookup"><span data-stu-id="13e09-133">id</span></span>|<span data-ttu-id="13e09-134">String</span><span class="sxs-lookup"><span data-stu-id="13e09-134">String</span></span>|<span data-ttu-id="13e09-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="13e09-135">Key of the entity.</span></span> <span data-ttu-id="13e09-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e09-137">lastModifiedDateTime</span></span>|<span data-ttu-id="13e09-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e09-138">DateTimeOffset</span></span>|<span data-ttu-id="13e09-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="13e09-139">DateTime the object was last modified.</span></span> <span data-ttu-id="13e09-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13e09-141">roleScopeTagIds</span></span>|<span data-ttu-id="13e09-142">String collection</span><span class="sxs-lookup"><span data-stu-id="13e09-142">String collection</span></span>|<span data-ttu-id="13e09-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="13e09-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13e09-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13e09-145">supportsScopeTags</span></span>|<span data-ttu-id="13e09-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="13e09-146">Boolean</span></span>|<span data-ttu-id="13e09-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="13e09-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13e09-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="13e09-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13e09-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="13e09-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13e09-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13e09-150">This property is read-only.</span></span> <span data-ttu-id="13e09-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13e09-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="13e09-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13e09-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="13e09-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="13e09-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="13e09-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13e09-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="13e09-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13e09-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="13e09-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="13e09-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="13e09-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13e09-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="13e09-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13e09-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="13e09-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="13e09-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="13e09-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e09-164">createdDateTime</span></span>|<span data-ttu-id="13e09-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e09-165">DateTimeOffset</span></span>|<span data-ttu-id="13e09-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="13e09-166">DateTime the object was created.</span></span> <span data-ttu-id="13e09-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-168">description</span><span class="sxs-lookup"><span data-stu-id="13e09-168">description</span></span>|<span data-ttu-id="13e09-169">String</span><span class="sxs-lookup"><span data-stu-id="13e09-169">String</span></span>|<span data-ttu-id="13e09-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13e09-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13e09-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-172">displayName</span><span class="sxs-lookup"><span data-stu-id="13e09-172">displayName</span></span>|<span data-ttu-id="13e09-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13e09-173">String</span></span>|<span data-ttu-id="13e09-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13e09-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13e09-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-176">versão</span><span class="sxs-lookup"><span data-stu-id="13e09-176">version</span></span>|<span data-ttu-id="13e09-177">Int32</span><span class="sxs-lookup"><span data-stu-id="13e09-177">Int32</span></span>|<span data-ttu-id="13e09-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13e09-178">Version of the device configuration.</span></span> <span data-ttu-id="13e09-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e09-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e09-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="13e09-180">payloadName</span></span>|<span data-ttu-id="13e09-181">String</span><span class="sxs-lookup"><span data-stu-id="13e09-181">String</span></span>|<span data-ttu-id="13e09-182">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="13e09-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="13e09-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="13e09-183">payloadFileName</span></span>|<span data-ttu-id="13e09-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13e09-184">String</span></span>|<span data-ttu-id="13e09-185">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="13e09-185">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="13e09-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="13e09-186">\*.xml).</span></span>|
|<span data-ttu-id="13e09-187">payload</span><span class="sxs-lookup"><span data-stu-id="13e09-187">payload</span></span>|<span data-ttu-id="13e09-188">Binária</span><span class="sxs-lookup"><span data-stu-id="13e09-188">Binary</span></span>|<span data-ttu-id="13e09-189">Carga.</span><span class="sxs-lookup"><span data-stu-id="13e09-189">Payload.</span></span> <span data-ttu-id="13e09-190">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="13e09-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="13e09-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e09-191">Response</span></span>
<span data-ttu-id="13e09-192">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13e09-192">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e09-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13e09-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="13e09-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13e09-194">Request</span></span>
<span data-ttu-id="13e09-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13e09-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1146

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="13e09-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e09-196">Response</span></span>
<span data-ttu-id="13e09-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13e09-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1318

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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





