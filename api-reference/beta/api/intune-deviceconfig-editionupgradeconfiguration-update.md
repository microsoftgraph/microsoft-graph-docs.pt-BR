---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 913c115e040698fb4c0934b8c12e57fa60caf116
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948461"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="ceeed-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="ceeed-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="ceeed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ceeed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceeed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ceeed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceeed-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ceeed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceeed-107">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ceeed-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceeed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceeed-108">Prerequisites</span></span>
<span data-ttu-id="ceeed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceeed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceeed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceeed-111">Permission type</span></span>|<span data-ttu-id="ceeed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ceeed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceeed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceeed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceeed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceeed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ceeed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceeed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceeed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceeed-116">Not supported.</span></span>|
|<span data-ttu-id="ceeed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceeed-117">Application</span></span>|<span data-ttu-id="ceeed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceeed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceeed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceeed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ceeed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeed-120">Request headers</span></span>
|<span data-ttu-id="ceeed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceeed-121">Header</span></span>|<span data-ttu-id="ceeed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ceeed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceeed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceeed-123">Authorization</span></span>|<span data-ttu-id="ceeed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceeed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceeed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ceeed-125">Accept</span></span>|<span data-ttu-id="ceeed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceeed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceeed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeed-127">Request body</span></span>
<span data-ttu-id="ceeed-128">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ceeed-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="ceeed-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ceeed-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="ceeed-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceeed-130">Property</span></span>|<span data-ttu-id="ceeed-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceeed-131">Type</span></span>|<span data-ttu-id="ceeed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceeed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceeed-133">id</span><span class="sxs-lookup"><span data-stu-id="ceeed-133">id</span></span>|<span data-ttu-id="ceeed-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceeed-134">String</span></span>|<span data-ttu-id="ceeed-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ceeed-135">Key of the entity.</span></span> <span data-ttu-id="ceeed-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceeed-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ceeed-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceeed-138">DateTimeOffset</span></span>|<span data-ttu-id="ceeed-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ceeed-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ceeed-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ceeed-141">roleScopeTagIds</span></span>|<span data-ttu-id="ceeed-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ceeed-142">String collection</span></span>|<span data-ttu-id="ceeed-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ceeed-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ceeed-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ceeed-145">supportsScopeTags</span></span>|<span data-ttu-id="ceeed-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="ceeed-146">Boolean</span></span>|<span data-ttu-id="ceeed-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ceeed-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ceeed-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ceeed-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ceeed-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="ceeed-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ceeed-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ceeed-150">This property is read-only.</span></span> <span data-ttu-id="ceeed-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ceeed-152">createdDateTime</span></span>|<span data-ttu-id="ceeed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceeed-153">DateTimeOffset</span></span>|<span data-ttu-id="ceeed-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ceeed-154">DateTime the object was created.</span></span> <span data-ttu-id="ceeed-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-156">description</span><span class="sxs-lookup"><span data-stu-id="ceeed-156">description</span></span>|<span data-ttu-id="ceeed-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceeed-157">String</span></span>|<span data-ttu-id="ceeed-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ceeed-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ceeed-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ceeed-160">displayName</span></span>|<span data-ttu-id="ceeed-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceeed-161">String</span></span>|<span data-ttu-id="ceeed-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ceeed-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ceeed-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-164">version</span><span class="sxs-lookup"><span data-stu-id="ceeed-164">version</span></span>|<span data-ttu-id="ceeed-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ceeed-165">Int32</span></span>|<span data-ttu-id="ceeed-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ceeed-166">Version of the device configuration.</span></span> <span data-ttu-id="ceeed-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ceeed-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ceeed-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="ceeed-168">licenseType</span></span>|[<span data-ttu-id="ceeed-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="ceeed-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="ceeed-170">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="ceeed-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="ceeed-171">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ceeed-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="ceeed-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="ceeed-172">targetEdition</span></span>|[<span data-ttu-id="ceeed-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="ceeed-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="ceeed-174">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="ceeed-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="ceeed-175">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ceeed-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="ceeed-176">license</span><span class="sxs-lookup"><span data-stu-id="ceeed-176">license</span></span>|<span data-ttu-id="ceeed-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceeed-177">String</span></span>|<span data-ttu-id="ceeed-178">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="ceeed-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="ceeed-179">productKey</span><span class="sxs-lookup"><span data-stu-id="ceeed-179">productKey</span></span>|<span data-ttu-id="ceeed-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceeed-180">String</span></span>|<span data-ttu-id="ceeed-181">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="ceeed-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="ceeed-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="ceeed-182">windowsSMode</span></span>|[<span data-ttu-id="ceeed-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="ceeed-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="ceeed-184">Configuração do modo de S.</span><span class="sxs-lookup"><span data-stu-id="ceeed-184">S mode configuration.</span></span> <span data-ttu-id="ceeed-185">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="ceeed-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="ceeed-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceeed-186">Response</span></span>
<span data-ttu-id="ceeed-187">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceeed-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceeed-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceeed-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceeed-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeed-189">Request</span></span>
<span data-ttu-id="ceeed-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceeed-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ceeed-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceeed-191">Response</span></span>
<span data-ttu-id="ceeed-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceeed-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





