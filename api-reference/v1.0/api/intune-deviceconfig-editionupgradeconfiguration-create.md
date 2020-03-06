---
title: Criar editionUpgradeConfiguration
description: Cria um novo objeto editionUpgradeConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b6e4df796ef37b2c446f497c8c8fe0007d297fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514687"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="6b756-103">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b756-103">Create editionUpgradeConfiguration</span></span>

<span data-ttu-id="6b756-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b756-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b756-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b756-106">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b756-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b756-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b756-107">Prerequisites</span></span>
<span data-ttu-id="6b756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b756-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b756-110">Permission type</span></span>|<span data-ttu-id="6b756-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b756-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b756-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b756-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b756-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b756-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b756-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b756-115">Not supported.</span></span>|
|<span data-ttu-id="6b756-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b756-116">Application</span></span>|<span data-ttu-id="6b756-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b756-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b756-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b756-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b756-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b756-119">Request headers</span></span>
|<span data-ttu-id="6b756-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b756-120">Header</span></span>|<span data-ttu-id="6b756-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b756-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b756-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b756-122">Authorization</span></span>|<span data-ttu-id="6b756-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b756-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b756-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b756-124">Accept</span></span>|<span data-ttu-id="6b756-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b756-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b756-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b756-126">Request body</span></span>
<span data-ttu-id="6b756-127">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b756-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="6b756-128">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b756-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="6b756-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b756-129">Property</span></span>|<span data-ttu-id="6b756-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b756-130">Type</span></span>|<span data-ttu-id="6b756-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b756-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b756-132">id</span><span class="sxs-lookup"><span data-stu-id="6b756-132">id</span></span>|<span data-ttu-id="6b756-133">String</span><span class="sxs-lookup"><span data-stu-id="6b756-133">String</span></span>|<span data-ttu-id="6b756-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b756-134">Key of the entity.</span></span> <span data-ttu-id="6b756-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b756-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6b756-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b756-137">DateTimeOffset</span></span>|<span data-ttu-id="6b756-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b756-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6b756-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b756-140">createdDateTime</span></span>|<span data-ttu-id="6b756-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b756-141">DateTimeOffset</span></span>|<span data-ttu-id="6b756-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6b756-142">DateTime the object was created.</span></span> <span data-ttu-id="6b756-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-144">description</span><span class="sxs-lookup"><span data-stu-id="6b756-144">description</span></span>|<span data-ttu-id="6b756-145">String</span><span class="sxs-lookup"><span data-stu-id="6b756-145">String</span></span>|<span data-ttu-id="6b756-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b756-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b756-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6b756-148">displayName</span></span>|<span data-ttu-id="6b756-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b756-149">String</span></span>|<span data-ttu-id="6b756-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b756-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b756-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-152">versão</span><span class="sxs-lookup"><span data-stu-id="6b756-152">version</span></span>|<span data-ttu-id="6b756-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6b756-153">Int32</span></span>|<span data-ttu-id="6b756-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6b756-154">Version of the device configuration.</span></span> <span data-ttu-id="6b756-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b756-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b756-156">licenseType</span><span class="sxs-lookup"><span data-stu-id="6b756-156">licenseType</span></span>|[<span data-ttu-id="6b756-157">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="6b756-157">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="6b756-158">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="6b756-158">Edition Upgrade License Type.</span></span> <span data-ttu-id="6b756-159">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="6b756-159">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="6b756-160">targetEdition</span><span class="sxs-lookup"><span data-stu-id="6b756-160">targetEdition</span></span>|[<span data-ttu-id="6b756-161">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="6b756-161">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="6b756-162">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="6b756-162">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="6b756-163">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="6b756-163">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="6b756-164">license</span><span class="sxs-lookup"><span data-stu-id="6b756-164">license</span></span>|<span data-ttu-id="6b756-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b756-165">String</span></span>|<span data-ttu-id="6b756-166">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="6b756-166">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="6b756-167">productKey</span><span class="sxs-lookup"><span data-stu-id="6b756-167">productKey</span></span>|<span data-ttu-id="6b756-168">String</span><span class="sxs-lookup"><span data-stu-id="6b756-168">String</span></span>|<span data-ttu-id="6b756-169">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="6b756-169">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="6b756-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b756-170">Response</span></span>
<span data-ttu-id="6b756-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b756-171">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b756-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b756-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b756-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b756-173">Request</span></span>
<span data-ttu-id="6b756-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b756-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b756-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b756-175">Response</span></span>
<span data-ttu-id="6b756-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b756-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




