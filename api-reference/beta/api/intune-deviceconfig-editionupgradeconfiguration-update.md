---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
ms.openlocfilehash: ca438526cbb781a34690e93fe51aeed523f57b50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032948"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="3741a-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="3741a-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="3741a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3741a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3741a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3741a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3741a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3741a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3741a-107">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3741a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3741a-108">Prerequisites</span></span>
<span data-ttu-id="3741a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3741a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3741a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3741a-111">Permission type</span></span>|<span data-ttu-id="3741a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3741a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3741a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3741a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3741a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3741a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3741a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3741a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3741a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3741a-116">Not supported.</span></span>|
|<span data-ttu-id="3741a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3741a-117">Application</span></span>|<span data-ttu-id="3741a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3741a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3741a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3741a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3741a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-120">Request headers</span></span>
|<span data-ttu-id="3741a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3741a-121">Header</span></span>|<span data-ttu-id="3741a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3741a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3741a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3741a-123">Authorization</span></span>|<span data-ttu-id="3741a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3741a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3741a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3741a-125">Accept</span></span>|<span data-ttu-id="3741a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3741a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3741a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-127">Request body</span></span>
<span data-ttu-id="3741a-128">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="3741a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3741a-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="3741a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3741a-130">Property</span></span>|<span data-ttu-id="3741a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3741a-131">Type</span></span>|<span data-ttu-id="3741a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3741a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3741a-133">id</span><span class="sxs-lookup"><span data-stu-id="3741a-133">id</span></span>|<span data-ttu-id="3741a-134">String</span><span class="sxs-lookup"><span data-stu-id="3741a-134">String</span></span>|<span data-ttu-id="3741a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3741a-135">Key of the entity.</span></span> <span data-ttu-id="3741a-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3741a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3741a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3741a-138">DateTimeOffset</span></span>|<span data-ttu-id="3741a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3741a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3741a-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3741a-141">roleScopeTagIds</span></span>|<span data-ttu-id="3741a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3741a-142">String collection</span></span>|<span data-ttu-id="3741a-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="3741a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3741a-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3741a-145">supportsScopeTags</span></span>|<span data-ttu-id="3741a-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3741a-146">Boolean</span></span>|<span data-ttu-id="3741a-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3741a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3741a-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3741a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3741a-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3741a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3741a-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3741a-150">This property is read-only.</span></span> <span data-ttu-id="3741a-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3741a-152">createdDateTime</span></span>|<span data-ttu-id="3741a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3741a-153">DateTimeOffset</span></span>|<span data-ttu-id="3741a-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3741a-154">DateTime the object was created.</span></span> <span data-ttu-id="3741a-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-156">description</span><span class="sxs-lookup"><span data-stu-id="3741a-156">description</span></span>|<span data-ttu-id="3741a-157">String</span><span class="sxs-lookup"><span data-stu-id="3741a-157">String</span></span>|<span data-ttu-id="3741a-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3741a-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3741a-160">displayName</span></span>|<span data-ttu-id="3741a-161">String</span><span class="sxs-lookup"><span data-stu-id="3741a-161">String</span></span>|<span data-ttu-id="3741a-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3741a-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-164">version</span><span class="sxs-lookup"><span data-stu-id="3741a-164">version</span></span>|<span data-ttu-id="3741a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3741a-165">Int32</span></span>|<span data-ttu-id="3741a-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3741a-166">Version of the device configuration.</span></span> <span data-ttu-id="3741a-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3741a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3741a-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="3741a-168">licenseType</span></span>|[<span data-ttu-id="3741a-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="3741a-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="3741a-170">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="3741a-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="3741a-171">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="3741a-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="3741a-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="3741a-172">targetEdition</span></span>|[<span data-ttu-id="3741a-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="3741a-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="3741a-174">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="3741a-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="3741a-175">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="3741a-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="3741a-176">license</span><span class="sxs-lookup"><span data-stu-id="3741a-176">license</span></span>|<span data-ttu-id="3741a-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-177">String</span></span>|<span data-ttu-id="3741a-178">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="3741a-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="3741a-179">productKey</span><span class="sxs-lookup"><span data-stu-id="3741a-179">productKey</span></span>|<span data-ttu-id="3741a-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3741a-180">String</span></span>|<span data-ttu-id="3741a-181">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="3741a-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="3741a-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="3741a-182">windowsSMode</span></span>|[<span data-ttu-id="3741a-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="3741a-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="3741a-184">Configuração do modo de S.</span><span class="sxs-lookup"><span data-stu-id="3741a-184">S mode configuration.</span></span> <span data-ttu-id="3741a-185">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="3741a-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="3741a-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="3741a-186">Response</span></span>
<span data-ttu-id="3741a-187">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3741a-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3741a-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3741a-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="3741a-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3741a-189">Request</span></span>
<span data-ttu-id="3741a-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3741a-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 429

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="3741a-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="3741a-191">Response</span></span>
<span data-ttu-id="3741a-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3741a-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```





