---
title: Criar macOSCustomAppConfiguration
description: Criar um novo objeto macOSCustomAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3035a596963663b7ca58229d01d84bea4aede4af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297403"
---
# <a name="create-macoscustomappconfiguration"></a><span data-ttu-id="36fb0-103">Criar macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="36fb0-103">Create macOSCustomAppConfiguration</span></span>

<span data-ttu-id="36fb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36fb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36fb0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36fb0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36fb0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36fb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36fb0-107">Criar um novo objeto [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="36fb0-107">Create a new [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36fb0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36fb0-108">Prerequisites</span></span>
<span data-ttu-id="36fb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36fb0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36fb0-111">Permission type</span></span>|<span data-ttu-id="36fb0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36fb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36fb0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36fb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36fb0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36fb0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36fb0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36fb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36fb0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36fb0-116">Not supported.</span></span>|
|<span data-ttu-id="36fb0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36fb0-117">Application</span></span>|<span data-ttu-id="36fb0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36fb0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36fb0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36fb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36fb0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36fb0-120">Request headers</span></span>
|<span data-ttu-id="36fb0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36fb0-121">Header</span></span>|<span data-ttu-id="36fb0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="36fb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36fb0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36fb0-123">Authorization</span></span>|<span data-ttu-id="36fb0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36fb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36fb0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36fb0-125">Accept</span></span>|<span data-ttu-id="36fb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36fb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36fb0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36fb0-127">Request body</span></span>
<span data-ttu-id="36fb0-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="36fb0-128">In the request body, supply a JSON representation for the macOSCustomAppConfiguration object.</span></span>

<span data-ttu-id="36fb0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="36fb0-129">The following table shows the properties that are required when you create the macOSCustomAppConfiguration.</span></span>

|<span data-ttu-id="36fb0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36fb0-130">Property</span></span>|<span data-ttu-id="36fb0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="36fb0-131">Type</span></span>|<span data-ttu-id="36fb0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="36fb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36fb0-133">id</span><span class="sxs-lookup"><span data-stu-id="36fb0-133">id</span></span>|<span data-ttu-id="36fb0-134">String</span><span class="sxs-lookup"><span data-stu-id="36fb0-134">String</span></span>|<span data-ttu-id="36fb0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36fb0-135">Key of the entity.</span></span> <span data-ttu-id="36fb0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36fb0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="36fb0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36fb0-138">DateTimeOffset</span></span>|<span data-ttu-id="36fb0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="36fb0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="36fb0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36fb0-141">roleScopeTagIds</span></span>|<span data-ttu-id="36fb0-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="36fb0-142">String collection</span></span>|<span data-ttu-id="36fb0-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="36fb0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36fb0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36fb0-145">supportsScopeTags</span></span>|<span data-ttu-id="36fb0-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="36fb0-146">Boolean</span></span>|<span data-ttu-id="36fb0-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="36fb0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36fb0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="36fb0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36fb0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="36fb0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36fb0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36fb0-150">This property is read-only.</span></span> <span data-ttu-id="36fb0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36fb0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36fb0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36fb0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36fb0-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="36fb0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36fb0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36fb0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36fb0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36fb0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36fb0-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="36fb0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36fb0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36fb0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36fb0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36fb0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36fb0-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="36fb0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36fb0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36fb0-164">createdDateTime</span></span>|<span data-ttu-id="36fb0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36fb0-165">DateTimeOffset</span></span>|<span data-ttu-id="36fb0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="36fb0-166">DateTime the object was created.</span></span> <span data-ttu-id="36fb0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-168">description</span><span class="sxs-lookup"><span data-stu-id="36fb0-168">description</span></span>|<span data-ttu-id="36fb0-169">String</span><span class="sxs-lookup"><span data-stu-id="36fb0-169">String</span></span>|<span data-ttu-id="36fb0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36fb0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36fb0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="36fb0-172">displayName</span></span>|<span data-ttu-id="36fb0-173">String</span><span class="sxs-lookup"><span data-stu-id="36fb0-173">String</span></span>|<span data-ttu-id="36fb0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36fb0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36fb0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-176">versão</span><span class="sxs-lookup"><span data-stu-id="36fb0-176">version</span></span>|<span data-ttu-id="36fb0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="36fb0-177">Int32</span></span>|<span data-ttu-id="36fb0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36fb0-178">Version of the device configuration.</span></span> <span data-ttu-id="36fb0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36fb0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36fb0-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="36fb0-180">bundleId</span></span>|<span data-ttu-id="36fb0-181">String</span><span class="sxs-lookup"><span data-stu-id="36fb0-181">String</span></span>|<span data-ttu-id="36fb0-182">ID do pacote para direcionamento.</span><span class="sxs-lookup"><span data-stu-id="36fb0-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="36fb0-183">fileName</span><span class="sxs-lookup"><span data-stu-id="36fb0-183">fileName</span></span>|<span data-ttu-id="36fb0-184">String</span><span class="sxs-lookup"><span data-stu-id="36fb0-184">String</span></span>|<span data-ttu-id="36fb0-185">Nome do arquivo de configuração (\*. plist</span><span class="sxs-lookup"><span data-stu-id="36fb0-185">Configuration file name (\*.plist</span></span> | <span data-ttu-id="36fb0-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="36fb0-186">\*.xml).</span></span>|
|<span data-ttu-id="36fb0-187">configurationXml</span><span class="sxs-lookup"><span data-stu-id="36fb0-187">configurationXml</span></span>|<span data-ttu-id="36fb0-188">Binária</span><span class="sxs-lookup"><span data-stu-id="36fb0-188">Binary</span></span>|<span data-ttu-id="36fb0-189">XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="36fb0-189">Configuration xml.</span></span> <span data-ttu-id="36fb0-190">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="36fb0-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="36fb0-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fb0-191">Response</span></span>
<span data-ttu-id="36fb0-192">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36fb0-192">If successful, this method returns a `201 Created` response code and a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36fb0-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36fb0-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="36fb0-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36fb0-194">Request</span></span>
<span data-ttu-id="36fb0-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36fb0-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="36fb0-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="36fb0-196">Response</span></span>
<span data-ttu-id="36fb0-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36fb0-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




