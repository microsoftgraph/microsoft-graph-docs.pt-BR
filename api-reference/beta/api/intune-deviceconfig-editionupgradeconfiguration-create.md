---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c55d5871e7cd361b66cec0f9e6c0d822752c3b2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163669"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="c37b5-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c37b5-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="c37b5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c37b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c37b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c37b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c37b5-106">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c37b5-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c37b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c37b5-107">Prerequisites</span></span>
<span data-ttu-id="c37b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c37b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c37b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c37b5-110">Permission type</span></span>|<span data-ttu-id="c37b5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c37b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c37b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c37b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c37b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c37b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c37b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c37b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c37b5-115">Not supported.</span></span>|
|<span data-ttu-id="c37b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c37b5-116">Application</span></span>|<span data-ttu-id="c37b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c37b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c37b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c37b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c37b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c37b5-119">Request headers</span></span>
|<span data-ttu-id="c37b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c37b5-120">Header</span></span>|<span data-ttu-id="c37b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c37b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c37b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c37b5-122">Authorization</span></span>|<span data-ttu-id="c37b5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c37b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c37b5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c37b5-124">Accept</span></span>|<span data-ttu-id="c37b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c37b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c37b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c37b5-126">Request body</span></span>
<span data-ttu-id="c37b5-127">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c37b5-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="c37b5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c37b5-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="c37b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c37b5-129">Property</span></span>|<span data-ttu-id="c37b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c37b5-130">Type</span></span>|<span data-ttu-id="c37b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c37b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37b5-132">id</span><span class="sxs-lookup"><span data-stu-id="c37b5-132">id</span></span>|<span data-ttu-id="c37b5-133">String</span><span class="sxs-lookup"><span data-stu-id="c37b5-133">String</span></span>|<span data-ttu-id="c37b5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c37b5-134">Key of the entity.</span></span> <span data-ttu-id="c37b5-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c37b5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c37b5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c37b5-137">DateTimeOffset</span></span>|<span data-ttu-id="c37b5-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c37b5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c37b5-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c37b5-140">roleScopeTagIds</span></span>|<span data-ttu-id="c37b5-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c37b5-141">String collection</span></span>|<span data-ttu-id="c37b5-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c37b5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c37b5-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c37b5-144">supportsScopeTags</span></span>|<span data-ttu-id="c37b5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c37b5-145">Boolean</span></span>|<span data-ttu-id="c37b5-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c37b5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c37b5-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c37b5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c37b5-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c37b5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c37b5-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c37b5-149">This property is read-only.</span></span> <span data-ttu-id="c37b5-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c37b5-151">createdDateTime</span></span>|<span data-ttu-id="c37b5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c37b5-152">DateTimeOffset</span></span>|<span data-ttu-id="c37b5-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c37b5-153">DateTime the object was created.</span></span> <span data-ttu-id="c37b5-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-155">description</span><span class="sxs-lookup"><span data-stu-id="c37b5-155">description</span></span>|<span data-ttu-id="c37b5-156">String</span><span class="sxs-lookup"><span data-stu-id="c37b5-156">String</span></span>|<span data-ttu-id="c37b5-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c37b5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c37b5-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c37b5-159">displayName</span></span>|<span data-ttu-id="c37b5-160">String</span><span class="sxs-lookup"><span data-stu-id="c37b5-160">String</span></span>|<span data-ttu-id="c37b5-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c37b5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c37b5-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-163">version</span><span class="sxs-lookup"><span data-stu-id="c37b5-163">version</span></span>|<span data-ttu-id="c37b5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c37b5-164">Int32</span></span>|<span data-ttu-id="c37b5-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c37b5-165">Version of the device configuration.</span></span> <span data-ttu-id="c37b5-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c37b5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c37b5-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="c37b5-167">licenseType</span></span>|[<span data-ttu-id="c37b5-168">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="c37b5-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="c37b5-169">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c37b5-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="c37b5-170">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="c37b5-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="c37b5-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="c37b5-171">targetEdition</span></span>|[<span data-ttu-id="c37b5-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="c37b5-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="c37b5-173">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c37b5-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="c37b5-174">Os valores possíveis são `windows10Enterprise`: `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`,.</span><span class="sxs-lookup"><span data-stu-id="c37b5-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="c37b5-175">license</span><span class="sxs-lookup"><span data-stu-id="c37b5-175">license</span></span>|<span data-ttu-id="c37b5-176">String</span><span class="sxs-lookup"><span data-stu-id="c37b5-176">String</span></span>|<span data-ttu-id="c37b5-177">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c37b5-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="c37b5-178">productKey</span><span class="sxs-lookup"><span data-stu-id="c37b5-178">productKey</span></span>|<span data-ttu-id="c37b5-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c37b5-179">String</span></span>|<span data-ttu-id="c37b5-180">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="c37b5-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="c37b5-181">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="c37b5-181">windowsSMode</span></span>|[<span data-ttu-id="c37b5-182">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c37b5-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="c37b5-183">Configuração de modo S.</span><span class="sxs-lookup"><span data-stu-id="c37b5-183">S mode configuration.</span></span> <span data-ttu-id="c37b5-184">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="c37b5-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="c37b5-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c37b5-185">Response</span></span>
<span data-ttu-id="c37b5-186">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c37b5-186">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c37b5-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c37b5-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="c37b5-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c37b5-188">Request</span></span>
<span data-ttu-id="c37b5-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c37b5-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
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

### <a name="response"></a><span data-ttu-id="c37b5-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="c37b5-190">Response</span></span>
<span data-ttu-id="c37b5-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c37b5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




