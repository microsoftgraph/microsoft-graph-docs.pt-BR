---
title: Atualizar editionUpgradeConfiguration
description: Atualizar as propriedades de um objeto editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3dba0ce2627735bc783f1f5e41c62aec1b5c681c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972184"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="41514-103">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="41514-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="41514-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41514-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41514-105">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41514-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41514-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41514-106">Prerequisites</span></span>
<span data-ttu-id="41514-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41514-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41514-109">Permission type</span></span>|<span data-ttu-id="41514-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41514-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41514-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41514-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41514-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41514-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41514-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41514-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41514-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41514-114">Not supported.</span></span>|
|<span data-ttu-id="41514-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41514-115">Application</span></span>|<span data-ttu-id="41514-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41514-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41514-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41514-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="41514-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41514-118">Request headers</span></span>
|<span data-ttu-id="41514-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41514-119">Header</span></span>|<span data-ttu-id="41514-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41514-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41514-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41514-121">Authorization</span></span>|<span data-ttu-id="41514-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41514-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41514-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41514-123">Accept</span></span>|<span data-ttu-id="41514-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41514-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41514-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41514-125">Request body</span></span>
<span data-ttu-id="41514-126">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41514-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="41514-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41514-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="41514-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41514-128">Property</span></span>|<span data-ttu-id="41514-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="41514-129">Type</span></span>|<span data-ttu-id="41514-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="41514-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41514-131">id</span><span class="sxs-lookup"><span data-stu-id="41514-131">id</span></span>|<span data-ttu-id="41514-132">String</span><span class="sxs-lookup"><span data-stu-id="41514-132">String</span></span>|<span data-ttu-id="41514-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41514-133">Key of the entity.</span></span> <span data-ttu-id="41514-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41514-135">lastModifiedDateTime</span></span>|<span data-ttu-id="41514-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41514-136">DateTimeOffset</span></span>|<span data-ttu-id="41514-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="41514-137">DateTime the object was last modified.</span></span> <span data-ttu-id="41514-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41514-139">createdDateTime</span></span>|<span data-ttu-id="41514-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41514-140">DateTimeOffset</span></span>|<span data-ttu-id="41514-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="41514-141">DateTime the object was created.</span></span> <span data-ttu-id="41514-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-143">description</span><span class="sxs-lookup"><span data-stu-id="41514-143">description</span></span>|<span data-ttu-id="41514-144">String</span><span class="sxs-lookup"><span data-stu-id="41514-144">String</span></span>|<span data-ttu-id="41514-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41514-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41514-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-147">displayName</span><span class="sxs-lookup"><span data-stu-id="41514-147">displayName</span></span>|<span data-ttu-id="41514-148">String</span><span class="sxs-lookup"><span data-stu-id="41514-148">String</span></span>|<span data-ttu-id="41514-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41514-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41514-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-151">version</span><span class="sxs-lookup"><span data-stu-id="41514-151">version</span></span>|<span data-ttu-id="41514-152">Int32</span><span class="sxs-lookup"><span data-stu-id="41514-152">Int32</span></span>|<span data-ttu-id="41514-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="41514-153">Version of the device configuration.</span></span> <span data-ttu-id="41514-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41514-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41514-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="41514-155">licenseType</span></span>|[<span data-ttu-id="41514-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="41514-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="41514-157">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="41514-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="41514-158">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="41514-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="41514-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="41514-159">targetEdition</span></span>|[<span data-ttu-id="41514-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="41514-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="41514-161">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="41514-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="41514-162">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="41514-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="41514-163">license</span><span class="sxs-lookup"><span data-stu-id="41514-163">license</span></span>|<span data-ttu-id="41514-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41514-164">String</span></span>|<span data-ttu-id="41514-165">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="41514-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="41514-166">productKey</span><span class="sxs-lookup"><span data-stu-id="41514-166">productKey</span></span>|<span data-ttu-id="41514-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41514-167">String</span></span>|<span data-ttu-id="41514-168">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="41514-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="41514-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="41514-169">Response</span></span>
<span data-ttu-id="41514-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41514-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41514-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41514-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="41514-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41514-172">Request</span></span>
<span data-ttu-id="41514-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41514-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41514-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="41514-174">Response</span></span>
<span data-ttu-id="41514-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41514-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



