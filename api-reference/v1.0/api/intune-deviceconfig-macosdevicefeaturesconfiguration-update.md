---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0539e19de3cf7189e4bc35fea78f85bd52eaa80e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870242"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="6ceba-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ceba-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6ceba-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ceba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ceba-105">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ceba-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ceba-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ceba-106">Prerequisites</span></span>
<span data-ttu-id="6ceba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ceba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ceba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ceba-109">Permission type</span></span>|<span data-ttu-id="6ceba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ceba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ceba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ceba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ceba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ceba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ceba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ceba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ceba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ceba-114">Not supported.</span></span>|
|<span data-ttu-id="6ceba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ceba-115">Application</span></span>|<span data-ttu-id="6ceba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ceba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ceba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ceba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ceba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ceba-118">Request headers</span></span>
|<span data-ttu-id="6ceba-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ceba-119">Header</span></span>|<span data-ttu-id="6ceba-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6ceba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ceba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ceba-121">Authorization</span></span>|<span data-ttu-id="6ceba-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ceba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ceba-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ceba-123">Accept</span></span>|<span data-ttu-id="6ceba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ceba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ceba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ceba-125">Request body</span></span>
<span data-ttu-id="6ceba-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ceba-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6ceba-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ceba-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6ceba-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ceba-128">Property</span></span>|<span data-ttu-id="6ceba-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ceba-129">Type</span></span>|<span data-ttu-id="6ceba-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ceba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ceba-131">id</span><span class="sxs-lookup"><span data-stu-id="6ceba-131">id</span></span>|<span data-ttu-id="6ceba-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ceba-132">String</span></span>|<span data-ttu-id="6ceba-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ceba-133">Key of the entity.</span></span> <span data-ttu-id="6ceba-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ceba-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ceba-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6ceba-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ceba-136">DateTimeOffset</span></span>|<span data-ttu-id="6ceba-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6ceba-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6ceba-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ceba-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ceba-139">createdDateTime</span></span>|<span data-ttu-id="6ceba-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ceba-140">DateTimeOffset</span></span>|<span data-ttu-id="6ceba-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6ceba-141">DateTime the object was created.</span></span> <span data-ttu-id="6ceba-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ceba-143">description</span><span class="sxs-lookup"><span data-stu-id="6ceba-143">description</span></span>|<span data-ttu-id="6ceba-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ceba-144">String</span></span>|<span data-ttu-id="6ceba-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ceba-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ceba-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ceba-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6ceba-147">displayName</span></span>|<span data-ttu-id="6ceba-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ceba-148">String</span></span>|<span data-ttu-id="6ceba-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ceba-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ceba-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ceba-151">version</span><span class="sxs-lookup"><span data-stu-id="6ceba-151">version</span></span>|<span data-ttu-id="6ceba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ceba-152">Int32</span></span>|<span data-ttu-id="6ceba-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ceba-153">Version of the device configuration.</span></span> <span data-ttu-id="6ceba-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ceba-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6ceba-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ceba-155">Response</span></span>
<span data-ttu-id="6ceba-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ceba-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ceba-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ceba-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ceba-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ceba-158">Request</span></span>
<span data-ttu-id="6ceba-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ceba-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ceba-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ceba-160">Response</span></span>
<span data-ttu-id="6ceba-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ceba-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



