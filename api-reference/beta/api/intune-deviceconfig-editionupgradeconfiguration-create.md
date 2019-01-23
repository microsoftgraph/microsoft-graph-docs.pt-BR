---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67a86f00fb8160d9226de0343b21230977523ef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421239"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="9cdcf-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9cdcf-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="9cdcf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cdcf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cdcf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cdcf-107">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9cdcf-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cdcf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cdcf-108">Prerequisites</span></span>
<span data-ttu-id="9cdcf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cdcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9cdcf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cdcf-111">Permission type</span></span>|<span data-ttu-id="9cdcf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cdcf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cdcf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cdcf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cdcf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cdcf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-116">Not supported.</span></span>|
|<span data-ttu-id="9cdcf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cdcf-117">Application</span></span>|<span data-ttu-id="9cdcf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cdcf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cdcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9cdcf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cdcf-120">Request headers</span></span>
|<span data-ttu-id="9cdcf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cdcf-121">Header</span></span>|<span data-ttu-id="9cdcf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9cdcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cdcf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cdcf-123">Authorization</span></span>|<span data-ttu-id="9cdcf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cdcf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cdcf-125">Accept</span></span>|<span data-ttu-id="9cdcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cdcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cdcf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cdcf-127">Request body</span></span>
<span data-ttu-id="9cdcf-128">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="9cdcf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="9cdcf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cdcf-130">Property</span></span>|<span data-ttu-id="9cdcf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cdcf-131">Type</span></span>|<span data-ttu-id="9cdcf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cdcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cdcf-133">id</span><span class="sxs-lookup"><span data-stu-id="9cdcf-133">id</span></span>|<span data-ttu-id="9cdcf-134">String</span><span class="sxs-lookup"><span data-stu-id="9cdcf-134">String</span></span>|<span data-ttu-id="9cdcf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-135">Key of the entity.</span></span> <span data-ttu-id="9cdcf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cdcf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9cdcf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cdcf-138">DateTimeOffset</span></span>|<span data-ttu-id="9cdcf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9cdcf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9cdcf-141">roleScopeTagIds</span></span>|<span data-ttu-id="9cdcf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9cdcf-142">String collection</span></span>|<span data-ttu-id="9cdcf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9cdcf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9cdcf-145">supportsScopeTags</span></span>|<span data-ttu-id="9cdcf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cdcf-146">Boolean</span></span>|<span data-ttu-id="9cdcf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9cdcf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9cdcf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9cdcf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-150">This property is read-only.</span></span> <span data-ttu-id="9cdcf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cdcf-152">createdDateTime</span></span>|<span data-ttu-id="9cdcf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cdcf-153">DateTimeOffset</span></span>|<span data-ttu-id="9cdcf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-154">DateTime the object was created.</span></span> <span data-ttu-id="9cdcf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-156">description</span><span class="sxs-lookup"><span data-stu-id="9cdcf-156">description</span></span>|<span data-ttu-id="9cdcf-157">String</span><span class="sxs-lookup"><span data-stu-id="9cdcf-157">String</span></span>|<span data-ttu-id="9cdcf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9cdcf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9cdcf-160">displayName</span></span>|<span data-ttu-id="9cdcf-161">String</span><span class="sxs-lookup"><span data-stu-id="9cdcf-161">String</span></span>|<span data-ttu-id="9cdcf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9cdcf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-164">version</span><span class="sxs-lookup"><span data-stu-id="9cdcf-164">version</span></span>|<span data-ttu-id="9cdcf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9cdcf-165">Int32</span></span>|<span data-ttu-id="9cdcf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-166">Version of the device configuration.</span></span> <span data-ttu-id="9cdcf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9cdcf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9cdcf-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="9cdcf-168">licenseType</span></span>|[<span data-ttu-id="9cdcf-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="9cdcf-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="9cdcf-170">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="9cdcf-171">Os valores possíveis são: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="9cdcf-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="9cdcf-172">targetEdition</span></span>|[<span data-ttu-id="9cdcf-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="9cdcf-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="9cdcf-174">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="9cdcf-175">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="9cdcf-176">license</span><span class="sxs-lookup"><span data-stu-id="9cdcf-176">license</span></span>|<span data-ttu-id="9cdcf-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cdcf-177">String</span></span>|<span data-ttu-id="9cdcf-178">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="9cdcf-179">productKey</span><span class="sxs-lookup"><span data-stu-id="9cdcf-179">productKey</span></span>|<span data-ttu-id="9cdcf-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cdcf-180">String</span></span>|<span data-ttu-id="9cdcf-181">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="9cdcf-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="9cdcf-182">windowsSMode</span></span>|[<span data-ttu-id="9cdcf-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9cdcf-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="9cdcf-184">Configuração do modo de S.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-184">S mode configuration.</span></span> <span data-ttu-id="9cdcf-185">Os valores possíveis são: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="9cdcf-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cdcf-186">Response</span></span>
<span data-ttu-id="9cdcf-187">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cdcf-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cdcf-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cdcf-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cdcf-189">Request</span></span>
<span data-ttu-id="9cdcf-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9cdcf-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cdcf-191">Response</span></span>
<span data-ttu-id="9cdcf-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cdcf-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




