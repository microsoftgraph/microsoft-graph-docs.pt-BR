---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0028e9a34a45165f7adcd228b6d752a7947db5a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442115"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="0b256-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b256-103">Update editionUpgradeConfiguration</span></span>

<span data-ttu-id="0b256-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b256-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b256-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b256-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b256-106">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b256-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b256-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b256-107">Prerequisites</span></span>
<span data-ttu-id="0b256-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b256-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b256-110">Permission type</span></span>|<span data-ttu-id="0b256-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b256-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b256-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b256-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b256-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b256-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b256-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b256-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b256-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b256-115">Not supported.</span></span>|
|<span data-ttu-id="0b256-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b256-116">Application</span></span>|<span data-ttu-id="0b256-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b256-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b256-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b256-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0b256-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b256-119">Request headers</span></span>
|<span data-ttu-id="0b256-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b256-120">Header</span></span>|<span data-ttu-id="0b256-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b256-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b256-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b256-122">Authorization</span></span>|<span data-ttu-id="0b256-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b256-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b256-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b256-124">Accept</span></span>|<span data-ttu-id="0b256-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b256-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b256-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b256-126">Request body</span></span>
<span data-ttu-id="0b256-127">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b256-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="0b256-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b256-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="0b256-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b256-129">Property</span></span>|<span data-ttu-id="0b256-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b256-130">Type</span></span>|<span data-ttu-id="0b256-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b256-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b256-132">id</span><span class="sxs-lookup"><span data-stu-id="0b256-132">id</span></span>|<span data-ttu-id="0b256-133">String</span><span class="sxs-lookup"><span data-stu-id="0b256-133">String</span></span>|<span data-ttu-id="0b256-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b256-134">Key of the entity.</span></span> <span data-ttu-id="0b256-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b256-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0b256-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b256-137">DateTimeOffset</span></span>|<span data-ttu-id="0b256-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0b256-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0b256-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b256-140">createdDateTime</span></span>|<span data-ttu-id="0b256-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b256-141">DateTimeOffset</span></span>|<span data-ttu-id="0b256-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0b256-142">DateTime the object was created.</span></span> <span data-ttu-id="0b256-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-144">description</span><span class="sxs-lookup"><span data-stu-id="0b256-144">description</span></span>|<span data-ttu-id="0b256-145">String</span><span class="sxs-lookup"><span data-stu-id="0b256-145">String</span></span>|<span data-ttu-id="0b256-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b256-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b256-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0b256-148">displayName</span></span>|<span data-ttu-id="0b256-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b256-149">String</span></span>|<span data-ttu-id="0b256-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b256-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b256-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-152">versão</span><span class="sxs-lookup"><span data-stu-id="0b256-152">version</span></span>|<span data-ttu-id="0b256-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0b256-153">Int32</span></span>|<span data-ttu-id="0b256-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b256-154">Version of the device configuration.</span></span> <span data-ttu-id="0b256-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b256-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b256-156">licenseType</span><span class="sxs-lookup"><span data-stu-id="0b256-156">licenseType</span></span>|[<span data-ttu-id="0b256-157">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="0b256-157">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="0b256-158">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="0b256-158">Edition Upgrade License Type.</span></span> <span data-ttu-id="0b256-159">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="0b256-159">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="0b256-160">targetEdition</span><span class="sxs-lookup"><span data-stu-id="0b256-160">targetEdition</span></span>|[<span data-ttu-id="0b256-161">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="0b256-161">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="0b256-162">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="0b256-162">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="0b256-163">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="0b256-163">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="0b256-164">license</span><span class="sxs-lookup"><span data-stu-id="0b256-164">license</span></span>|<span data-ttu-id="0b256-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b256-165">String</span></span>|<span data-ttu-id="0b256-166">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="0b256-166">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="0b256-167">productKey</span><span class="sxs-lookup"><span data-stu-id="0b256-167">productKey</span></span>|<span data-ttu-id="0b256-168">String</span><span class="sxs-lookup"><span data-stu-id="0b256-168">String</span></span>|<span data-ttu-id="0b256-169">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="0b256-169">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="0b256-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b256-170">Response</span></span>
<span data-ttu-id="0b256-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b256-171">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b256-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b256-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b256-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b256-173">Request</span></span>
<span data-ttu-id="0b256-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b256-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="0b256-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b256-175">Response</span></span>
<span data-ttu-id="0b256-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b256-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```






