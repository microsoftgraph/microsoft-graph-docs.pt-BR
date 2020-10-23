---
title: Criar da ioseducationdeviceconfiguration
description: Criar um novo objeto da ioseducationdeviceconfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 739a777fb5074731e1e813c96513ef66ae7b2d7d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724845"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="3af32-103">Criar da ioseducationdeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="3af32-103">Create iosEducationDeviceConfiguration</span></span>

<span data-ttu-id="3af32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3af32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3af32-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3af32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3af32-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3af32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af32-107">Criar um novo objeto [da ioseducationdeviceconfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3af32-107">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3af32-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3af32-108">Prerequisites</span></span>
<span data-ttu-id="3af32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3af32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af32-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3af32-111">Permission type</span></span>|<span data-ttu-id="3af32-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3af32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3af32-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3af32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3af32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3af32-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3af32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3af32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3af32-116">Not supported.</span></span>|
|<span data-ttu-id="3af32-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3af32-117">Application</span></span>|<span data-ttu-id="3af32-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af32-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3af32-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3af32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3af32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3af32-120">Request headers</span></span>
|<span data-ttu-id="3af32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3af32-121">Header</span></span>|<span data-ttu-id="3af32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3af32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3af32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3af32-123">Authorization</span></span>|<span data-ttu-id="3af32-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3af32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3af32-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3af32-125">Accept</span></span>|<span data-ttu-id="3af32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3af32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3af32-127">Request body</span></span>
<span data-ttu-id="3af32-128">No corpo da solicitação, forneça uma representação JSON do objeto da ioseducationdeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="3af32-128">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="3af32-129">A tabela a seguir mostra as propriedades que são necessárias ao criar da ioseducationdeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="3af32-129">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="3af32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3af32-130">Property</span></span>|<span data-ttu-id="3af32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3af32-131">Type</span></span>|<span data-ttu-id="3af32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3af32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af32-133">id</span><span class="sxs-lookup"><span data-stu-id="3af32-133">id</span></span>|<span data-ttu-id="3af32-134">String</span><span class="sxs-lookup"><span data-stu-id="3af32-134">String</span></span>|<span data-ttu-id="3af32-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3af32-135">Key of the entity.</span></span> <span data-ttu-id="3af32-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3af32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3af32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3af32-138">DateTimeOffset</span></span>|<span data-ttu-id="3af32-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3af32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3af32-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3af32-141">roleScopeTagIds</span></span>|<span data-ttu-id="3af32-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3af32-142">String collection</span></span>|<span data-ttu-id="3af32-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3af32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3af32-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3af32-145">supportsScopeTags</span></span>|<span data-ttu-id="3af32-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3af32-146">Boolean</span></span>|<span data-ttu-id="3af32-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3af32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3af32-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3af32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3af32-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3af32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3af32-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3af32-150">This property is read-only.</span></span> <span data-ttu-id="3af32-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3af32-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3af32-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3af32-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3af32-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3af32-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3af32-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3af32-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3af32-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3af32-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3af32-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3af32-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3af32-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3af32-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3af32-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3af32-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3af32-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3af32-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3af32-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3af32-164">createdDateTime</span></span>|<span data-ttu-id="3af32-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3af32-165">DateTimeOffset</span></span>|<span data-ttu-id="3af32-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3af32-166">DateTime the object was created.</span></span> <span data-ttu-id="3af32-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-168">description</span><span class="sxs-lookup"><span data-stu-id="3af32-168">description</span></span>|<span data-ttu-id="3af32-169">String</span><span class="sxs-lookup"><span data-stu-id="3af32-169">String</span></span>|<span data-ttu-id="3af32-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3af32-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3af32-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3af32-172">displayName</span></span>|<span data-ttu-id="3af32-173">String</span><span class="sxs-lookup"><span data-stu-id="3af32-173">String</span></span>|<span data-ttu-id="3af32-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3af32-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3af32-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3af32-176">versão</span><span class="sxs-lookup"><span data-stu-id="3af32-176">version</span></span>|<span data-ttu-id="3af32-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3af32-177">Int32</span></span>|<span data-ttu-id="3af32-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3af32-178">Version of the device configuration.</span></span> <span data-ttu-id="3af32-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3af32-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3af32-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af32-180">Response</span></span>
<span data-ttu-id="3af32-181">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [da ioseducationdeviceconfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3af32-181">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af32-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3af32-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="3af32-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3af32-183">Request</span></span>
<span data-ttu-id="3af32-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3af32-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1034

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="3af32-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af32-185">Response</span></span>
<span data-ttu-id="3af32-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3af32-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1206

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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





