---
title: Atualizar macOSExtensionsConfiguration
description: Atualiza as propriedades de um objeto macOSExtensionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b64610e2905b8d510565e22124a37b49308d8060
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306603"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="45462-103">Atualizar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="45462-103">Update macOSExtensionsConfiguration</span></span>

<span data-ttu-id="45462-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45462-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45462-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45462-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45462-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45462-107">Atualiza as propriedades de um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45462-107">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45462-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45462-108">Prerequisites</span></span>
<span data-ttu-id="45462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45462-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45462-111">Permission type</span></span>|<span data-ttu-id="45462-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45462-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45462-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45462-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45462-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45462-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45462-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45462-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45462-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45462-116">Not supported.</span></span>|
|<span data-ttu-id="45462-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45462-117">Application</span></span>|<span data-ttu-id="45462-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45462-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45462-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45462-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="45462-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45462-120">Request headers</span></span>
|<span data-ttu-id="45462-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45462-121">Header</span></span>|<span data-ttu-id="45462-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45462-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45462-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45462-123">Authorization</span></span>|<span data-ttu-id="45462-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45462-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45462-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45462-125">Accept</span></span>|<span data-ttu-id="45462-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45462-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45462-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45462-127">Request body</span></span>
<span data-ttu-id="45462-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45462-128">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="45462-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45462-129">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="45462-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45462-130">Property</span></span>|<span data-ttu-id="45462-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45462-131">Type</span></span>|<span data-ttu-id="45462-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45462-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45462-133">id</span><span class="sxs-lookup"><span data-stu-id="45462-133">id</span></span>|<span data-ttu-id="45462-134">String</span><span class="sxs-lookup"><span data-stu-id="45462-134">String</span></span>|<span data-ttu-id="45462-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45462-135">Key of the entity.</span></span> <span data-ttu-id="45462-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45462-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45462-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45462-138">DateTimeOffset</span></span>|<span data-ttu-id="45462-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45462-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45462-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45462-141">roleScopeTagIds</span></span>|<span data-ttu-id="45462-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45462-142">String collection</span></span>|<span data-ttu-id="45462-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="45462-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45462-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45462-145">supportsScopeTags</span></span>|<span data-ttu-id="45462-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="45462-146">Boolean</span></span>|<span data-ttu-id="45462-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="45462-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45462-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="45462-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45462-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="45462-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45462-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45462-150">This property is read-only.</span></span> <span data-ttu-id="45462-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45462-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="45462-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45462-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="45462-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="45462-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="45462-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45462-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="45462-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45462-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="45462-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="45462-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="45462-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45462-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="45462-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45462-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="45462-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="45462-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="45462-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45462-164">createdDateTime</span></span>|<span data-ttu-id="45462-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45462-165">DateTimeOffset</span></span>|<span data-ttu-id="45462-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45462-166">DateTime the object was created.</span></span> <span data-ttu-id="45462-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-168">description</span><span class="sxs-lookup"><span data-stu-id="45462-168">description</span></span>|<span data-ttu-id="45462-169">String</span><span class="sxs-lookup"><span data-stu-id="45462-169">String</span></span>|<span data-ttu-id="45462-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45462-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45462-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-172">displayName</span><span class="sxs-lookup"><span data-stu-id="45462-172">displayName</span></span>|<span data-ttu-id="45462-173">String</span><span class="sxs-lookup"><span data-stu-id="45462-173">String</span></span>|<span data-ttu-id="45462-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45462-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45462-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-176">versão</span><span class="sxs-lookup"><span data-stu-id="45462-176">version</span></span>|<span data-ttu-id="45462-177">Int32</span><span class="sxs-lookup"><span data-stu-id="45462-177">Int32</span></span>|<span data-ttu-id="45462-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45462-178">Version of the device configuration.</span></span> <span data-ttu-id="45462-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45462-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45462-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="45462-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="45462-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="45462-181">Boolean</span></span>|<span data-ttu-id="45462-182">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="45462-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="45462-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="45462-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="45462-184">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45462-184">String collection</span></span>|<span data-ttu-id="45462-185">Todas as extensões de kernel assinadas com validade pelos identificadores de equipe nesta lista poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="45462-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="45462-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="45462-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="45462-187">coleção [macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="45462-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="45462-188">Uma lista de extensões do kernel que terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="45462-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="45462-189">.</span><span class="sxs-lookup"><span data-stu-id="45462-189">.</span></span> <span data-ttu-id="45462-190">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45462-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="45462-191">systemExtensionsBlockOverride</span><span class="sxs-lookup"><span data-stu-id="45462-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="45462-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="45462-192">Boolean</span></span>|<span data-ttu-id="45462-193">Obtém ou define se é para permitir que o usuário aprove extensões de sistema adicionais não explicitamente permitidas por perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="45462-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="45462-194">systemExtensionsAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="45462-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="45462-195">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45462-195">String collection</span></span>|<span data-ttu-id="45462-196">Obtém ou define uma lista de identificadores de equipe permitidos.</span><span class="sxs-lookup"><span data-stu-id="45462-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="45462-197">Qualquer extensão do sistema assinada com qualquer um dos identificadores de equipe especificados será aprovada.</span><span class="sxs-lookup"><span data-stu-id="45462-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="45462-198">systemExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="45462-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="45462-199">coleção [macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md)</span><span class="sxs-lookup"><span data-stu-id="45462-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="45462-200">Obtém ou define uma lista de extensões de sistema macOS permitidas.</span><span class="sxs-lookup"><span data-stu-id="45462-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="45462-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45462-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="45462-202">systemExtensionsAllowedTypes</span><span class="sxs-lookup"><span data-stu-id="45462-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="45462-203">coleção [macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)</span><span class="sxs-lookup"><span data-stu-id="45462-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="45462-204">Obtém ou define uma lista de tipos de extensões de sistema macOS permitidos.</span><span class="sxs-lookup"><span data-stu-id="45462-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="45462-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45462-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="45462-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="45462-206">Response</span></span>
<span data-ttu-id="45462-207">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45462-207">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45462-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45462-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="45462-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45462-209">Request</span></span>
<span data-ttu-id="45462-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45462-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1965

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
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="45462-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="45462-211">Response</span></span>
<span data-ttu-id="45462-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45462-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2137

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
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```




