---
title: Criar macOSExtensionsConfiguration
description: Criar um novo objeto macOSExtensionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7101e56b49dd3c94be3d9da41cc3d2bc0ce7f53
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179324"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="6f033-103">Criar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f033-103">Create macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="6f033-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f033-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f033-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f033-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f033-106">Criar um novo objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6f033-106">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f033-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f033-107">Prerequisites</span></span>
<span data-ttu-id="6f033-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f033-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f033-110">Permission type</span></span>|<span data-ttu-id="6f033-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f033-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f033-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f033-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f033-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f033-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f033-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f033-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f033-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f033-115">Not supported.</span></span>|
|<span data-ttu-id="6f033-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f033-116">Application</span></span>|<span data-ttu-id="6f033-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f033-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f033-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f033-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f033-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f033-119">Request headers</span></span>
|<span data-ttu-id="6f033-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f033-120">Header</span></span>|<span data-ttu-id="6f033-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6f033-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f033-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f033-122">Authorization</span></span>|<span data-ttu-id="6f033-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f033-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f033-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f033-124">Accept</span></span>|<span data-ttu-id="6f033-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f033-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f033-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f033-126">Request body</span></span>
<span data-ttu-id="6f033-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f033-127">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="6f033-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f033-128">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="6f033-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f033-129">Property</span></span>|<span data-ttu-id="6f033-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f033-130">Type</span></span>|<span data-ttu-id="6f033-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f033-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f033-132">id</span><span class="sxs-lookup"><span data-stu-id="6f033-132">id</span></span>|<span data-ttu-id="6f033-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f033-133">String</span></span>|<span data-ttu-id="6f033-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f033-134">Key of the entity.</span></span> <span data-ttu-id="6f033-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f033-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6f033-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f033-137">DateTimeOffset</span></span>|<span data-ttu-id="6f033-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6f033-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6f033-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f033-140">roleScopeTagIds</span></span>|<span data-ttu-id="6f033-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f033-141">String collection</span></span>|<span data-ttu-id="6f033-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6f033-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f033-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f033-144">supportsScopeTags</span></span>|<span data-ttu-id="6f033-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f033-145">Boolean</span></span>|<span data-ttu-id="6f033-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6f033-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f033-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6f033-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f033-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6f033-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f033-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f033-149">This property is read-only.</span></span> <span data-ttu-id="6f033-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f033-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6f033-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f033-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6f033-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6f033-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6f033-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f033-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6f033-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f033-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6f033-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6f033-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6f033-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f033-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6f033-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f033-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6f033-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6f033-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6f033-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f033-163">createdDateTime</span></span>|<span data-ttu-id="6f033-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f033-164">DateTimeOffset</span></span>|<span data-ttu-id="6f033-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6f033-165">DateTime the object was created.</span></span> <span data-ttu-id="6f033-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-167">descrição</span><span class="sxs-lookup"><span data-stu-id="6f033-167">description</span></span>|<span data-ttu-id="6f033-168">String</span><span class="sxs-lookup"><span data-stu-id="6f033-168">String</span></span>|<span data-ttu-id="6f033-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f033-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f033-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6f033-171">displayName</span></span>|<span data-ttu-id="6f033-172">String</span><span class="sxs-lookup"><span data-stu-id="6f033-172">String</span></span>|<span data-ttu-id="6f033-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f033-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f033-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-175">versão</span><span class="sxs-lookup"><span data-stu-id="6f033-175">version</span></span>|<span data-ttu-id="6f033-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6f033-176">Int32</span></span>|<span data-ttu-id="6f033-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f033-177">Version of the device configuration.</span></span> <span data-ttu-id="6f033-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f033-179">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="6f033-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="6f033-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f033-180">Boolean</span></span>|<span data-ttu-id="6f033-181">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="6f033-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="6f033-182">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="6f033-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="6f033-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f033-183">String collection</span></span>|<span data-ttu-id="6f033-184">Todas as extensões de kernel assinadas com validade pelos identificadores de equipe nesta lista poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="6f033-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="6f033-185">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="6f033-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="6f033-186">coleção [macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="6f033-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="6f033-187">Uma lista de extensões do kernel que terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="6f033-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="6f033-188">.</span><span class="sxs-lookup"><span data-stu-id="6f033-188"></span></span> <span data-ttu-id="6f033-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f033-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6f033-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f033-190">Response</span></span>
<span data-ttu-id="6f033-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f033-191">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f033-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f033-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f033-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f033-193">Request</span></span>
<span data-ttu-id="6f033-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f033-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1383

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6f033-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f033-195">Response</span></span>
<span data-ttu-id="6f033-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f033-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1555

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```




