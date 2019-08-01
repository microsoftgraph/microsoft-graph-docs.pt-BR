---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 165fe90924d24d225ab7d8f789c3cc2dd8d959a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997455"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="8cc2e-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cc2e-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8cc2e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc2e-105">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2e-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc2e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc2e-106">Prerequisites</span></span>
<span data-ttu-id="8cc2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc2e-109">Permission type</span></span>|<span data-ttu-id="8cc2e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc2e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc2e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-114">Not supported.</span></span>|
|<span data-ttu-id="8cc2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc2e-115">Application</span></span>|<span data-ttu-id="8cc2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc2e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8cc2e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2e-118">Request headers</span></span>
|<span data-ttu-id="8cc2e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc2e-119">Header</span></span>|<span data-ttu-id="8cc2e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc2e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc2e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc2e-121">Authorization</span></span>|<span data-ttu-id="8cc2e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc2e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cc2e-123">Accept</span></span>|<span data-ttu-id="8cc2e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc2e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc2e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2e-125">Request body</span></span>
<span data-ttu-id="8cc2e-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2e-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="8cc2e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2e-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="8cc2e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc2e-128">Property</span></span>|<span data-ttu-id="8cc2e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc2e-129">Type</span></span>|<span data-ttu-id="8cc2e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc2e-131">id</span><span class="sxs-lookup"><span data-stu-id="8cc2e-131">id</span></span>|<span data-ttu-id="8cc2e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2e-132">String</span></span>|<span data-ttu-id="8cc2e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-133">Key of the entity.</span></span> <span data-ttu-id="8cc2e-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc2e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc2e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc2e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc2e-136">DateTimeOffset</span></span>|<span data-ttu-id="8cc2e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8cc2e-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc2e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc2e-139">createdDateTime</span></span>|<span data-ttu-id="8cc2e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc2e-140">DateTimeOffset</span></span>|<span data-ttu-id="8cc2e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-141">DateTime the object was created.</span></span> <span data-ttu-id="8cc2e-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc2e-143">descrição</span><span class="sxs-lookup"><span data-stu-id="8cc2e-143">description</span></span>|<span data-ttu-id="8cc2e-144">String</span><span class="sxs-lookup"><span data-stu-id="8cc2e-144">String</span></span>|<span data-ttu-id="8cc2e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8cc2e-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc2e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc2e-147">displayName</span></span>|<span data-ttu-id="8cc2e-148">String</span><span class="sxs-lookup"><span data-stu-id="8cc2e-148">String</span></span>|<span data-ttu-id="8cc2e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8cc2e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc2e-151">versão</span><span class="sxs-lookup"><span data-stu-id="8cc2e-151">version</span></span>|<span data-ttu-id="8cc2e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc2e-152">Int32</span></span>|<span data-ttu-id="8cc2e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-153">Version of the device configuration.</span></span> <span data-ttu-id="8cc2e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8cc2e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc2e-155">Response</span></span>
<span data-ttu-id="8cc2e-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc2e-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc2e-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc2e-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2e-158">Request</span></span>
<span data-ttu-id="8cc2e-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="8cc2e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc2e-160">Response</span></span>
<span data-ttu-id="8cc2e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc2e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```



