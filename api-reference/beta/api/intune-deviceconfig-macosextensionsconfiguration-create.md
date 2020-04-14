---
title: Criar macOSExtensionsConfiguration
description: Criar um novo objeto macOSExtensionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4d31941139d98212a6fc7554a2a110db8b40805
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437963"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="d8920-103">Criar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8920-103">Create macOSExtensionsConfiguration</span></span>

<span data-ttu-id="d8920-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8920-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8920-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8920-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8920-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8920-107">Criar um novo objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8920-107">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8920-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8920-108">Prerequisites</span></span>
<span data-ttu-id="d8920-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8920-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8920-111">Permission type</span></span>|<span data-ttu-id="d8920-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8920-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8920-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8920-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8920-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8920-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8920-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8920-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8920-116">Not supported.</span></span>|
|<span data-ttu-id="d8920-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8920-117">Application</span></span>|<span data-ttu-id="d8920-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8920-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8920-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8920-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8920-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8920-120">Request headers</span></span>
|<span data-ttu-id="d8920-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8920-121">Header</span></span>|<span data-ttu-id="d8920-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8920-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8920-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8920-123">Authorization</span></span>|<span data-ttu-id="d8920-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8920-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8920-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8920-125">Accept</span></span>|<span data-ttu-id="d8920-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8920-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8920-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8920-127">Request body</span></span>
<span data-ttu-id="d8920-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d8920-128">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="d8920-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d8920-129">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="d8920-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8920-130">Property</span></span>|<span data-ttu-id="d8920-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8920-131">Type</span></span>|<span data-ttu-id="d8920-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8920-133">id</span><span class="sxs-lookup"><span data-stu-id="d8920-133">id</span></span>|<span data-ttu-id="d8920-134">String</span><span class="sxs-lookup"><span data-stu-id="d8920-134">String</span></span>|<span data-ttu-id="d8920-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8920-135">Key of the entity.</span></span> <span data-ttu-id="d8920-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8920-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d8920-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8920-138">DateTimeOffset</span></span>|<span data-ttu-id="d8920-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d8920-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d8920-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8920-141">roleScopeTagIds</span></span>|<span data-ttu-id="d8920-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d8920-142">String collection</span></span>|<span data-ttu-id="d8920-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d8920-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8920-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8920-145">supportsScopeTags</span></span>|<span data-ttu-id="d8920-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8920-146">Boolean</span></span>|<span data-ttu-id="d8920-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d8920-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8920-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d8920-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8920-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d8920-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8920-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8920-150">This property is read-only.</span></span> <span data-ttu-id="d8920-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8920-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d8920-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8920-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d8920-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d8920-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d8920-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8920-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d8920-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8920-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d8920-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d8920-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d8920-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d8920-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d8920-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d8920-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d8920-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d8920-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d8920-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8920-164">createdDateTime</span></span>|<span data-ttu-id="d8920-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8920-165">DateTimeOffset</span></span>|<span data-ttu-id="d8920-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d8920-166">DateTime the object was created.</span></span> <span data-ttu-id="d8920-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-168">description</span><span class="sxs-lookup"><span data-stu-id="d8920-168">description</span></span>|<span data-ttu-id="d8920-169">String</span><span class="sxs-lookup"><span data-stu-id="d8920-169">String</span></span>|<span data-ttu-id="d8920-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8920-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8920-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d8920-172">displayName</span></span>|<span data-ttu-id="d8920-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8920-173">String</span></span>|<span data-ttu-id="d8920-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8920-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8920-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-176">versão</span><span class="sxs-lookup"><span data-stu-id="d8920-176">version</span></span>|<span data-ttu-id="d8920-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d8920-177">Int32</span></span>|<span data-ttu-id="d8920-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8920-178">Version of the device configuration.</span></span> <span data-ttu-id="d8920-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8920-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="d8920-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="d8920-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8920-181">Boolean</span></span>|<span data-ttu-id="d8920-182">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="d8920-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="d8920-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="d8920-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="d8920-184">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d8920-184">String collection</span></span>|<span data-ttu-id="d8920-185">Todas as extensões de kernel assinadas com validade pelos identificadores de equipe nesta lista poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="d8920-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="d8920-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="d8920-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="d8920-187">coleção [macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="d8920-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="d8920-188">Uma lista de extensões do kernel que terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="d8920-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="d8920-189">.</span><span class="sxs-lookup"><span data-stu-id="d8920-189">.</span></span> <span data-ttu-id="d8920-190">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d8920-190">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d8920-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8920-191">Response</span></span>
<span data-ttu-id="d8920-192">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8920-192">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8920-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8920-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8920-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8920-194">Request</span></span>
<span data-ttu-id="d8920-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8920-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8920-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8920-196">Response</span></span>
<span data-ttu-id="d8920-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8920-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



