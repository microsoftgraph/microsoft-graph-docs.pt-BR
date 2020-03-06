---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8586f537d282701a09fd9d1209317610a876798b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514358"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="68720-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="68720-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="68720-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68720-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68720-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68720-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68720-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68720-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68720-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68720-107">Prerequisites</span></span>
<span data-ttu-id="68720-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68720-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68720-110">Permission type</span></span>|<span data-ttu-id="68720-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68720-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68720-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68720-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68720-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68720-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68720-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68720-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68720-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68720-115">Not supported.</span></span>|
|<span data-ttu-id="68720-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68720-116">Application</span></span>|<span data-ttu-id="68720-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68720-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68720-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68720-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68720-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68720-119">Request headers</span></span>
|<span data-ttu-id="68720-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68720-120">Header</span></span>|<span data-ttu-id="68720-121">Valor</span><span class="sxs-lookup"><span data-stu-id="68720-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68720-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="68720-122">Authorization</span></span>|<span data-ttu-id="68720-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68720-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68720-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68720-124">Accept</span></span>|<span data-ttu-id="68720-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68720-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68720-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68720-126">Request body</span></span>
<span data-ttu-id="68720-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68720-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="68720-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68720-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="68720-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68720-129">Property</span></span>|<span data-ttu-id="68720-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="68720-130">Type</span></span>|<span data-ttu-id="68720-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="68720-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68720-132">id</span><span class="sxs-lookup"><span data-stu-id="68720-132">id</span></span>|<span data-ttu-id="68720-133">String</span><span class="sxs-lookup"><span data-stu-id="68720-133">String</span></span>|<span data-ttu-id="68720-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68720-134">Key of the entity.</span></span> <span data-ttu-id="68720-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68720-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68720-136">lastModifiedDateTime</span></span>|<span data-ttu-id="68720-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68720-137">DateTimeOffset</span></span>|<span data-ttu-id="68720-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="68720-138">DateTime the object was last modified.</span></span> <span data-ttu-id="68720-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68720-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68720-140">createdDateTime</span></span>|<span data-ttu-id="68720-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68720-141">DateTimeOffset</span></span>|<span data-ttu-id="68720-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="68720-142">DateTime the object was created.</span></span> <span data-ttu-id="68720-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68720-144">description</span><span class="sxs-lookup"><span data-stu-id="68720-144">description</span></span>|<span data-ttu-id="68720-145">String</span><span class="sxs-lookup"><span data-stu-id="68720-145">String</span></span>|<span data-ttu-id="68720-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68720-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68720-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68720-148">displayName</span><span class="sxs-lookup"><span data-stu-id="68720-148">displayName</span></span>|<span data-ttu-id="68720-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68720-149">String</span></span>|<span data-ttu-id="68720-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68720-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68720-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68720-152">versão</span><span class="sxs-lookup"><span data-stu-id="68720-152">version</span></span>|<span data-ttu-id="68720-153">Int32</span><span class="sxs-lookup"><span data-stu-id="68720-153">Int32</span></span>|<span data-ttu-id="68720-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68720-154">Version of the device configuration.</span></span> <span data-ttu-id="68720-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68720-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="68720-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="68720-156">Response</span></span>
<span data-ttu-id="68720-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68720-157">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68720-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68720-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="68720-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68720-159">Request</span></span>
<span data-ttu-id="68720-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68720-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="68720-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="68720-161">Response</span></span>
<span data-ttu-id="68720-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68720-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




