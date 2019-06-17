---
title: Criar windows10EnterpriseModernAppManagementConfiguration
description: Criar um novo objeto windows10EnterpriseModernAppManagementConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6a0c514543b322dd577ff9780d8fa82a77351bc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962607"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="a59db-103">Criar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="a59db-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="a59db-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a59db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a59db-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a59db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a59db-106">Criar um novo objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a59db-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a59db-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a59db-107">Prerequisites</span></span>
<span data-ttu-id="a59db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59db-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a59db-110">Permission type</span></span>|<span data-ttu-id="a59db-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a59db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a59db-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a59db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a59db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a59db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a59db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a59db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59db-115">Not supported.</span></span>|
|<span data-ttu-id="a59db-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a59db-116">Application</span></span>|<span data-ttu-id="a59db-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a59db-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a59db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a59db-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a59db-119">Request headers</span></span>
|<span data-ttu-id="a59db-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a59db-120">Header</span></span>|<span data-ttu-id="a59db-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a59db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a59db-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a59db-122">Authorization</span></span>|<span data-ttu-id="a59db-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a59db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a59db-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a59db-124">Accept</span></span>|<span data-ttu-id="a59db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a59db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59db-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a59db-126">Request body</span></span>
<span data-ttu-id="a59db-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a59db-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="a59db-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a59db-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="a59db-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a59db-129">Property</span></span>|<span data-ttu-id="a59db-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a59db-130">Type</span></span>|<span data-ttu-id="a59db-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59db-132">id</span><span class="sxs-lookup"><span data-stu-id="a59db-132">id</span></span>|<span data-ttu-id="a59db-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59db-133">String</span></span>|<span data-ttu-id="a59db-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a59db-134">Key of the entity.</span></span> <span data-ttu-id="a59db-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a59db-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a59db-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59db-137">DateTimeOffset</span></span>|<span data-ttu-id="a59db-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a59db-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a59db-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a59db-140">roleScopeTagIds</span></span>|<span data-ttu-id="a59db-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59db-141">String collection</span></span>|<span data-ttu-id="a59db-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a59db-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a59db-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a59db-144">supportsScopeTags</span></span>|<span data-ttu-id="a59db-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59db-145">Boolean</span></span>|<span data-ttu-id="a59db-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a59db-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a59db-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a59db-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a59db-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a59db-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a59db-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a59db-149">This property is read-only.</span></span> <span data-ttu-id="a59db-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a59db-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a59db-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a59db-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a59db-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a59db-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a59db-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a59db-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a59db-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a59db-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a59db-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a59db-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a59db-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a59db-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a59db-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a59db-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a59db-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a59db-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a59db-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a59db-163">createdDateTime</span></span>|<span data-ttu-id="a59db-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59db-164">DateTimeOffset</span></span>|<span data-ttu-id="a59db-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a59db-165">DateTime the object was created.</span></span> <span data-ttu-id="a59db-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-167">descrição</span><span class="sxs-lookup"><span data-stu-id="a59db-167">description</span></span>|<span data-ttu-id="a59db-168">String</span><span class="sxs-lookup"><span data-stu-id="a59db-168">String</span></span>|<span data-ttu-id="a59db-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59db-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a59db-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a59db-171">displayName</span></span>|<span data-ttu-id="a59db-172">String</span><span class="sxs-lookup"><span data-stu-id="a59db-172">String</span></span>|<span data-ttu-id="a59db-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59db-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a59db-174">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-175">versão</span><span class="sxs-lookup"><span data-stu-id="a59db-175">version</span></span>|<span data-ttu-id="a59db-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a59db-176">Int32</span></span>|<span data-ttu-id="a59db-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59db-177">Version of the device configuration.</span></span> <span data-ttu-id="a59db-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a59db-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a59db-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="a59db-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="a59db-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59db-180">Boolean</span></span>|<span data-ttu-id="a59db-181">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="a59db-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="a59db-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59db-182">Response</span></span>
<span data-ttu-id="a59db-183">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59db-183">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a59db-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a59db-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="a59db-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a59db-185">Request</span></span>
<span data-ttu-id="a59db-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a59db-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1087

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
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
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="a59db-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59db-187">Response</span></span>
<span data-ttu-id="a59db-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a59db-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1259

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
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
  "uninstallBuiltInApps": true
}
```





