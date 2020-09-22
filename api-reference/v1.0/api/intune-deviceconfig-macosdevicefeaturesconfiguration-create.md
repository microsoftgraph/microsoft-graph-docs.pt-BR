---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ceec8fc70c77600c9ea57676f1328c5be73ddc73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023195"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="92ff8-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="92ff8-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="92ff8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92ff8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92ff8-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92ff8-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92ff8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92ff8-107">Prerequisites</span></span>
<span data-ttu-id="92ff8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ff8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92ff8-110">Permission type</span></span>|<span data-ttu-id="92ff8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92ff8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92ff8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92ff8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92ff8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ff8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92ff8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92ff8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92ff8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92ff8-115">Not supported.</span></span>|
|<span data-ttu-id="92ff8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92ff8-116">Application</span></span>|<span data-ttu-id="92ff8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92ff8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92ff8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92ff8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92ff8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92ff8-119">Request headers</span></span>
|<span data-ttu-id="92ff8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92ff8-120">Header</span></span>|<span data-ttu-id="92ff8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="92ff8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92ff8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92ff8-122">Authorization</span></span>|<span data-ttu-id="92ff8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ff8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92ff8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92ff8-124">Accept</span></span>|<span data-ttu-id="92ff8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92ff8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ff8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92ff8-126">Request body</span></span>
<span data-ttu-id="92ff8-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92ff8-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="92ff8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92ff8-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="92ff8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92ff8-129">Property</span></span>|<span data-ttu-id="92ff8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ff8-130">Type</span></span>|<span data-ttu-id="92ff8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ff8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ff8-132">id</span><span class="sxs-lookup"><span data-stu-id="92ff8-132">id</span></span>|<span data-ttu-id="92ff8-133">String</span><span class="sxs-lookup"><span data-stu-id="92ff8-133">String</span></span>|<span data-ttu-id="92ff8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92ff8-134">Key of the entity.</span></span> <span data-ttu-id="92ff8-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92ff8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92ff8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="92ff8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92ff8-137">DateTimeOffset</span></span>|<span data-ttu-id="92ff8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="92ff8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="92ff8-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92ff8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92ff8-140">createdDateTime</span></span>|<span data-ttu-id="92ff8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92ff8-141">DateTimeOffset</span></span>|<span data-ttu-id="92ff8-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="92ff8-142">DateTime the object was created.</span></span> <span data-ttu-id="92ff8-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92ff8-144">description</span><span class="sxs-lookup"><span data-stu-id="92ff8-144">description</span></span>|<span data-ttu-id="92ff8-145">String</span><span class="sxs-lookup"><span data-stu-id="92ff8-145">String</span></span>|<span data-ttu-id="92ff8-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92ff8-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92ff8-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92ff8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="92ff8-148">displayName</span></span>|<span data-ttu-id="92ff8-149">String</span><span class="sxs-lookup"><span data-stu-id="92ff8-149">String</span></span>|<span data-ttu-id="92ff8-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92ff8-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92ff8-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92ff8-152">versão</span><span class="sxs-lookup"><span data-stu-id="92ff8-152">version</span></span>|<span data-ttu-id="92ff8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="92ff8-153">Int32</span></span>|<span data-ttu-id="92ff8-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92ff8-154">Version of the device configuration.</span></span> <span data-ttu-id="92ff8-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92ff8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="92ff8-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ff8-156">Response</span></span>
<span data-ttu-id="92ff8-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92ff8-157">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ff8-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92ff8-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="92ff8-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92ff8-159">Request</span></span>
<span data-ttu-id="92ff8-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92ff8-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92ff8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ff8-161">Response</span></span>
<span data-ttu-id="92ff8-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92ff8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









