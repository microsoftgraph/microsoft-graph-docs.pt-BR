---
title: Atualizar macOSExtensionsConfiguration
description: Atualiza as propriedades de um objeto macOSExtensionsConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2cf5ebc963aaf3abe4b45c7ae92f743b613be56
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42745923"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="73ba2-103">Atualizar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ba2-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="73ba2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73ba2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73ba2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73ba2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73ba2-106">Atualiza as propriedades de um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73ba2-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73ba2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73ba2-107">Prerequisites</span></span>
<span data-ttu-id="73ba2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73ba2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73ba2-110">Permission type</span></span>|<span data-ttu-id="73ba2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73ba2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73ba2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73ba2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73ba2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ba2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73ba2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73ba2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73ba2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73ba2-115">Not supported.</span></span>|
|<span data-ttu-id="73ba2-116">Application</span><span class="sxs-lookup"><span data-stu-id="73ba2-116">Application</span></span>|<span data-ttu-id="73ba2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ba2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73ba2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73ba2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="73ba2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73ba2-119">Request headers</span></span>
|<span data-ttu-id="73ba2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73ba2-120">Header</span></span>|<span data-ttu-id="73ba2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73ba2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73ba2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73ba2-122">Authorization</span></span>|<span data-ttu-id="73ba2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73ba2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73ba2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73ba2-124">Accept</span></span>|<span data-ttu-id="73ba2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73ba2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73ba2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73ba2-126">Request body</span></span>
<span data-ttu-id="73ba2-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73ba2-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="73ba2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73ba2-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="73ba2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73ba2-129">Property</span></span>|<span data-ttu-id="73ba2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73ba2-130">Type</span></span>|<span data-ttu-id="73ba2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73ba2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ba2-132">id</span><span class="sxs-lookup"><span data-stu-id="73ba2-132">id</span></span>|<span data-ttu-id="73ba2-133">String</span><span class="sxs-lookup"><span data-stu-id="73ba2-133">String</span></span>|<span data-ttu-id="73ba2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73ba2-134">Key of the entity.</span></span> <span data-ttu-id="73ba2-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73ba2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73ba2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73ba2-137">DateTimeOffset</span></span>|<span data-ttu-id="73ba2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="73ba2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73ba2-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73ba2-140">roleScopeTagIds</span></span>|<span data-ttu-id="73ba2-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73ba2-141">String collection</span></span>|<span data-ttu-id="73ba2-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73ba2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73ba2-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73ba2-144">supportsScopeTags</span></span>|<span data-ttu-id="73ba2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="73ba2-145">Boolean</span></span>|<span data-ttu-id="73ba2-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="73ba2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73ba2-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="73ba2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73ba2-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="73ba2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73ba2-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73ba2-149">This property is read-only.</span></span> <span data-ttu-id="73ba2-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73ba2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="73ba2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73ba2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="73ba2-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="73ba2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="73ba2-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73ba2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="73ba2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73ba2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="73ba2-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="73ba2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="73ba2-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73ba2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="73ba2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73ba2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="73ba2-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="73ba2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="73ba2-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73ba2-163">createdDateTime</span></span>|<span data-ttu-id="73ba2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73ba2-164">DateTimeOffset</span></span>|<span data-ttu-id="73ba2-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="73ba2-165">DateTime the object was created.</span></span> <span data-ttu-id="73ba2-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-167">description</span><span class="sxs-lookup"><span data-stu-id="73ba2-167">description</span></span>|<span data-ttu-id="73ba2-168">String</span><span class="sxs-lookup"><span data-stu-id="73ba2-168">String</span></span>|<span data-ttu-id="73ba2-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73ba2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73ba2-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="73ba2-171">displayName</span></span>|<span data-ttu-id="73ba2-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73ba2-172">String</span></span>|<span data-ttu-id="73ba2-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73ba2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73ba2-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-175">versão</span><span class="sxs-lookup"><span data-stu-id="73ba2-175">version</span></span>|<span data-ttu-id="73ba2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="73ba2-176">Int32</span></span>|<span data-ttu-id="73ba2-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73ba2-177">Version of the device configuration.</span></span> <span data-ttu-id="73ba2-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ba2-179">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="73ba2-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="73ba2-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="73ba2-180">Boolean</span></span>|<span data-ttu-id="73ba2-181">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="73ba2-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="73ba2-182">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="73ba2-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="73ba2-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73ba2-183">String collection</span></span>|<span data-ttu-id="73ba2-184">Todas as extensões de kernel assinadas com validade pelos identificadores de equipe nesta lista poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="73ba2-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="73ba2-185">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="73ba2-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="73ba2-186">coleção [macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="73ba2-187">Uma lista de extensões do kernel que terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="73ba2-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="73ba2-188">.</span><span class="sxs-lookup"><span data-stu-id="73ba2-188">.</span></span> <span data-ttu-id="73ba2-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="73ba2-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="73ba2-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="73ba2-190">Response</span></span>
<span data-ttu-id="73ba2-191">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73ba2-191">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73ba2-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73ba2-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="73ba2-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73ba2-193">Request</span></span>
<span data-ttu-id="73ba2-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73ba2-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="73ba2-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="73ba2-195">Response</span></span>
<span data-ttu-id="73ba2-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73ba2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




