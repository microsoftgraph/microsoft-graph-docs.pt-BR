---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c32873ffe50a4a35f94324d782e055508389e7e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937919"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="dc6e7-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc6e7-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="dc6e7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc6e7-105">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dc6e7-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc6e7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc6e7-106">Prerequisites</span></span>
<span data-ttu-id="dc6e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc6e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc6e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc6e7-109">Permission type</span></span>|<span data-ttu-id="dc6e7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc6e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc6e7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc6e7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc6e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc6e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-114">Not supported.</span></span>|
|<span data-ttu-id="dc6e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc6e7-115">Application</span></span>|<span data-ttu-id="dc6e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc6e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc6e7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dc6e7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6e7-118">Request headers</span></span>
|<span data-ttu-id="dc6e7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc6e7-119">Header</span></span>|<span data-ttu-id="dc6e7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dc6e7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc6e7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc6e7-121">Authorization</span></span>|<span data-ttu-id="dc6e7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc6e7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc6e7-123">Accept</span></span>|<span data-ttu-id="dc6e7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc6e7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc6e7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6e7-125">Request body</span></span>
<span data-ttu-id="dc6e7-126">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="dc6e7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="dc6e7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc6e7-128">Property</span></span>|<span data-ttu-id="dc6e7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc6e7-129">Type</span></span>|<span data-ttu-id="dc6e7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc6e7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc6e7-131">id</span><span class="sxs-lookup"><span data-stu-id="dc6e7-131">id</span></span>|<span data-ttu-id="dc6e7-132">String</span><span class="sxs-lookup"><span data-stu-id="dc6e7-132">String</span></span>|<span data-ttu-id="dc6e7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-133">Key of the entity.</span></span> <span data-ttu-id="dc6e7-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc6e7-135">lastModifiedDateTime</span></span>|<span data-ttu-id="dc6e7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc6e7-136">DateTimeOffset</span></span>|<span data-ttu-id="dc6e7-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-137">DateTime the object was last modified.</span></span> <span data-ttu-id="dc6e7-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc6e7-139">createdDateTime</span></span>|<span data-ttu-id="dc6e7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc6e7-140">DateTimeOffset</span></span>|<span data-ttu-id="dc6e7-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-141">DateTime the object was created.</span></span> <span data-ttu-id="dc6e7-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-143">description</span><span class="sxs-lookup"><span data-stu-id="dc6e7-143">description</span></span>|<span data-ttu-id="dc6e7-144">String</span><span class="sxs-lookup"><span data-stu-id="dc6e7-144">String</span></span>|<span data-ttu-id="dc6e7-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dc6e7-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="dc6e7-147">displayName</span></span>|<span data-ttu-id="dc6e7-148">String</span><span class="sxs-lookup"><span data-stu-id="dc6e7-148">String</span></span>|<span data-ttu-id="dc6e7-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dc6e7-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-151">version</span><span class="sxs-lookup"><span data-stu-id="dc6e7-151">version</span></span>|<span data-ttu-id="dc6e7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dc6e7-152">Int32</span></span>|<span data-ttu-id="dc6e7-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-153">Version of the device configuration.</span></span> <span data-ttu-id="dc6e7-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc6e7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc6e7-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="dc6e7-155">licenseType</span></span>|[<span data-ttu-id="dc6e7-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="dc6e7-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="dc6e7-157">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="dc6e7-158">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="dc6e7-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="dc6e7-159">targetEdition</span></span>|[<span data-ttu-id="dc6e7-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="dc6e7-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="dc6e7-161">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="dc6e7-162">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="dc6e7-163">license</span><span class="sxs-lookup"><span data-stu-id="dc6e7-163">license</span></span>|<span data-ttu-id="dc6e7-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc6e7-164">String</span></span>|<span data-ttu-id="dc6e7-165">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="dc6e7-166">productKey</span><span class="sxs-lookup"><span data-stu-id="dc6e7-166">productKey</span></span>|<span data-ttu-id="dc6e7-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc6e7-167">String</span></span>|<span data-ttu-id="dc6e7-168">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="dc6e7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6e7-169">Response</span></span>
<span data-ttu-id="dc6e7-170">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc6e7-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc6e7-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc6e7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6e7-172">Request</span></span>
<span data-ttu-id="dc6e7-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="dc6e7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6e7-174">Response</span></span>
<span data-ttu-id="dc6e7-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc6e7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



