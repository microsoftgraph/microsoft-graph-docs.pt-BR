---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fd923367898dae191dfae4ac8b2dd026b368641
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964308"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="2b336-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b336-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="2b336-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b336-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b336-105">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b336-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b336-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b336-106">Prerequisites</span></span>
<span data-ttu-id="2b336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b336-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b336-109">Permission type</span></span>|<span data-ttu-id="2b336-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b336-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b336-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b336-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b336-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b336-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b336-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b336-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b336-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b336-114">Not supported.</span></span>|
|<span data-ttu-id="2b336-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b336-115">Application</span></span>|<span data-ttu-id="2b336-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b336-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b336-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b336-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b336-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b336-118">Request headers</span></span>
|<span data-ttu-id="2b336-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b336-119">Header</span></span>|<span data-ttu-id="2b336-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2b336-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b336-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b336-121">Authorization</span></span>|<span data-ttu-id="2b336-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b336-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b336-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b336-123">Accept</span></span>|<span data-ttu-id="2b336-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2b336-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b336-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b336-125">Request body</span></span>
<span data-ttu-id="2b336-126">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b336-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="2b336-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b336-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="2b336-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b336-128">Property</span></span>|<span data-ttu-id="2b336-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b336-129">Type</span></span>|<span data-ttu-id="2b336-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b336-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b336-131">id</span><span class="sxs-lookup"><span data-stu-id="2b336-131">id</span></span>|<span data-ttu-id="2b336-132">String</span><span class="sxs-lookup"><span data-stu-id="2b336-132">String</span></span>|<span data-ttu-id="2b336-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2b336-133">Key of the entity.</span></span> <span data-ttu-id="2b336-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b336-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2b336-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b336-136">DateTimeOffset</span></span>|<span data-ttu-id="2b336-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2b336-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2b336-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b336-139">createdDateTime</span></span>|<span data-ttu-id="2b336-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b336-140">DateTimeOffset</span></span>|<span data-ttu-id="2b336-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2b336-141">DateTime the object was created.</span></span> <span data-ttu-id="2b336-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-143">descrição</span><span class="sxs-lookup"><span data-stu-id="2b336-143">description</span></span>|<span data-ttu-id="2b336-144">String</span><span class="sxs-lookup"><span data-stu-id="2b336-144">String</span></span>|<span data-ttu-id="2b336-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b336-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b336-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2b336-147">displayName</span></span>|<span data-ttu-id="2b336-148">String</span><span class="sxs-lookup"><span data-stu-id="2b336-148">String</span></span>|<span data-ttu-id="2b336-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b336-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b336-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-151">versão</span><span class="sxs-lookup"><span data-stu-id="2b336-151">version</span></span>|<span data-ttu-id="2b336-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2b336-152">Int32</span></span>|<span data-ttu-id="2b336-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b336-153">Version of the device configuration.</span></span> <span data-ttu-id="2b336-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b336-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b336-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="2b336-155">licenseType</span></span>|[<span data-ttu-id="2b336-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="2b336-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="2b336-157">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="2b336-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="2b336-158">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="2b336-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="2b336-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="2b336-159">targetEdition</span></span>|[<span data-ttu-id="2b336-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="2b336-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="2b336-161">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="2b336-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="2b336-162">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="2b336-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="2b336-163">license</span><span class="sxs-lookup"><span data-stu-id="2b336-163">license</span></span>|<span data-ttu-id="2b336-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b336-164">String</span></span>|<span data-ttu-id="2b336-165">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="2b336-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="2b336-166">productKey</span><span class="sxs-lookup"><span data-stu-id="2b336-166">productKey</span></span>|<span data-ttu-id="2b336-167">String</span><span class="sxs-lookup"><span data-stu-id="2b336-167">String</span></span>|<span data-ttu-id="2b336-168">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="2b336-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="2b336-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b336-169">Response</span></span>
<span data-ttu-id="2b336-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b336-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b336-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b336-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b336-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b336-172">Request</span></span>
<span data-ttu-id="2b336-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b336-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b336-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b336-174">Response</span></span>
<span data-ttu-id="2b336-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b336-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



