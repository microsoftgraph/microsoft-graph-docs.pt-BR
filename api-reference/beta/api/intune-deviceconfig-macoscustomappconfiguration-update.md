---
title: Atualizar macOSCustomAppConfiguration
description: Atualiza as propriedades de um objeto macOSCustomAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe62c0cd065657331b3a6a01f60607dac10e6390
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442436"
---
# <a name="update-macoscustomappconfiguration"></a><span data-ttu-id="5cadd-103">Atualizar macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5cadd-103">Update macOSCustomAppConfiguration</span></span>

<span data-ttu-id="5cadd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5cadd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cadd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cadd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cadd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cadd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cadd-107">Atualiza as propriedades de um objeto [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5cadd-107">Update the properties of a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cadd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cadd-108">Prerequisites</span></span>
<span data-ttu-id="5cadd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cadd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cadd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cadd-111">Permission type</span></span>|<span data-ttu-id="5cadd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cadd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cadd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cadd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cadd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cadd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5cadd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cadd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cadd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cadd-116">Not supported.</span></span>|
|<span data-ttu-id="5cadd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cadd-117">Application</span></span>|<span data-ttu-id="5cadd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cadd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cadd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cadd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5cadd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cadd-120">Request headers</span></span>
|<span data-ttu-id="5cadd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cadd-121">Header</span></span>|<span data-ttu-id="5cadd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5cadd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cadd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cadd-123">Authorization</span></span>|<span data-ttu-id="5cadd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cadd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cadd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cadd-125">Accept</span></span>|<span data-ttu-id="5cadd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cadd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cadd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cadd-127">Request body</span></span>
<span data-ttu-id="5cadd-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5cadd-128">In the request body, supply a JSON representation for the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

<span data-ttu-id="5cadd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5cadd-129">The following table shows the properties that are required when you create the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

|<span data-ttu-id="5cadd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cadd-130">Property</span></span>|<span data-ttu-id="5cadd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cadd-131">Type</span></span>|<span data-ttu-id="5cadd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cadd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cadd-133">id</span><span class="sxs-lookup"><span data-stu-id="5cadd-133">id</span></span>|<span data-ttu-id="5cadd-134">String</span><span class="sxs-lookup"><span data-stu-id="5cadd-134">String</span></span>|<span data-ttu-id="5cadd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5cadd-135">Key of the entity.</span></span> <span data-ttu-id="5cadd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cadd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5cadd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cadd-138">DateTimeOffset</span></span>|<span data-ttu-id="5cadd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5cadd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5cadd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5cadd-141">roleScopeTagIds</span></span>|<span data-ttu-id="5cadd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5cadd-142">String collection</span></span>|<span data-ttu-id="5cadd-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5cadd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5cadd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5cadd-145">supportsScopeTags</span></span>|<span data-ttu-id="5cadd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cadd-146">Boolean</span></span>|<span data-ttu-id="5cadd-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5cadd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5cadd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5cadd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5cadd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5cadd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5cadd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cadd-150">This property is read-only.</span></span> <span data-ttu-id="5cadd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5cadd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5cadd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5cadd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5cadd-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5cadd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5cadd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5cadd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5cadd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5cadd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5cadd-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5cadd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5cadd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5cadd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5cadd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5cadd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5cadd-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5cadd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5cadd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cadd-164">createdDateTime</span></span>|<span data-ttu-id="5cadd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cadd-165">DateTimeOffset</span></span>|<span data-ttu-id="5cadd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5cadd-166">DateTime the object was created.</span></span> <span data-ttu-id="5cadd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-168">description</span><span class="sxs-lookup"><span data-stu-id="5cadd-168">description</span></span>|<span data-ttu-id="5cadd-169">String</span><span class="sxs-lookup"><span data-stu-id="5cadd-169">String</span></span>|<span data-ttu-id="5cadd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5cadd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5cadd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5cadd-172">displayName</span></span>|<span data-ttu-id="5cadd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cadd-173">String</span></span>|<span data-ttu-id="5cadd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5cadd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5cadd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-176">versão</span><span class="sxs-lookup"><span data-stu-id="5cadd-176">version</span></span>|<span data-ttu-id="5cadd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5cadd-177">Int32</span></span>|<span data-ttu-id="5cadd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5cadd-178">Version of the device configuration.</span></span> <span data-ttu-id="5cadd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5cadd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5cadd-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="5cadd-180">bundleId</span></span>|<span data-ttu-id="5cadd-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cadd-181">String</span></span>|<span data-ttu-id="5cadd-182">ID do pacote para direcionamento.</span><span class="sxs-lookup"><span data-stu-id="5cadd-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="5cadd-183">fileName</span><span class="sxs-lookup"><span data-stu-id="5cadd-183">fileName</span></span>|<span data-ttu-id="5cadd-184">String</span><span class="sxs-lookup"><span data-stu-id="5cadd-184">String</span></span>|<span data-ttu-id="5cadd-185">Nome do arquivo de configuração (\*. plist</span><span class="sxs-lookup"><span data-stu-id="5cadd-185">Configuration file name (\*.plist</span></span> | <span data-ttu-id="5cadd-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="5cadd-186">\*.xml).</span></span>|
|<span data-ttu-id="5cadd-187">configurationXml</span><span class="sxs-lookup"><span data-stu-id="5cadd-187">configurationXml</span></span>|<span data-ttu-id="5cadd-188">Binária</span><span class="sxs-lookup"><span data-stu-id="5cadd-188">Binary</span></span>|<span data-ttu-id="5cadd-189">XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="5cadd-189">Configuration xml.</span></span> <span data-ttu-id="5cadd-190">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="5cadd-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="5cadd-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cadd-191">Response</span></span>
<span data-ttu-id="5cadd-192">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cadd-192">If successful, this method returns a `200 OK` response code and an updated [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cadd-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cadd-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cadd-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cadd-194">Request</span></span>
<span data-ttu-id="5cadd-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cadd-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1149

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="5cadd-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cadd-196">Response</span></span>
<span data-ttu-id="5cadd-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cadd-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1321

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
  "id": "1b8a4e02-4e02-1b8a-024e-8a1b024e8a1b",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





