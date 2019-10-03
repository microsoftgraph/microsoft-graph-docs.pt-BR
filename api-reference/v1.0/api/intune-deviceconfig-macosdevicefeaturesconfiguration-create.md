---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 385b4dccdc75c00f6efdfda05a3d0a37c57ba6fe
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365989"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="49f99-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="49f99-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="49f99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f99-105">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49f99-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49f99-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49f99-106">Prerequisites</span></span>
<span data-ttu-id="49f99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49f99-109">Permission type</span></span>|<span data-ttu-id="49f99-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49f99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49f99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49f99-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f99-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49f99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49f99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49f99-114">Not supported.</span></span>|
|<span data-ttu-id="49f99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49f99-115">Application</span></span>|<span data-ttu-id="49f99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49f99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49f99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49f99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49f99-118">Request headers</span></span>
|<span data-ttu-id="49f99-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49f99-119">Header</span></span>|<span data-ttu-id="49f99-120">Valor</span><span class="sxs-lookup"><span data-stu-id="49f99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49f99-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49f99-121">Authorization</span></span>|<span data-ttu-id="49f99-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49f99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49f99-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49f99-123">Accept</span></span>|<span data-ttu-id="49f99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49f99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49f99-125">Request body</span></span>
<span data-ttu-id="49f99-126">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49f99-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="49f99-127">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49f99-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="49f99-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49f99-128">Property</span></span>|<span data-ttu-id="49f99-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f99-129">Type</span></span>|<span data-ttu-id="49f99-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f99-131">id</span><span class="sxs-lookup"><span data-stu-id="49f99-131">id</span></span>|<span data-ttu-id="49f99-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49f99-132">String</span></span>|<span data-ttu-id="49f99-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="49f99-133">Key of the entity.</span></span> <span data-ttu-id="49f99-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49f99-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49f99-135">lastModifiedDateTime</span></span>|<span data-ttu-id="49f99-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f99-136">DateTimeOffset</span></span>|<span data-ttu-id="49f99-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="49f99-137">DateTime the object was last modified.</span></span> <span data-ttu-id="49f99-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49f99-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49f99-139">createdDateTime</span></span>|<span data-ttu-id="49f99-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f99-140">DateTimeOffset</span></span>|<span data-ttu-id="49f99-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="49f99-141">DateTime the object was created.</span></span> <span data-ttu-id="49f99-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49f99-143">descrição</span><span class="sxs-lookup"><span data-stu-id="49f99-143">description</span></span>|<span data-ttu-id="49f99-144">String</span><span class="sxs-lookup"><span data-stu-id="49f99-144">String</span></span>|<span data-ttu-id="49f99-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49f99-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49f99-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49f99-147">displayName</span><span class="sxs-lookup"><span data-stu-id="49f99-147">displayName</span></span>|<span data-ttu-id="49f99-148">String</span><span class="sxs-lookup"><span data-stu-id="49f99-148">String</span></span>|<span data-ttu-id="49f99-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49f99-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49f99-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49f99-151">versão</span><span class="sxs-lookup"><span data-stu-id="49f99-151">version</span></span>|<span data-ttu-id="49f99-152">Int32</span><span class="sxs-lookup"><span data-stu-id="49f99-152">Int32</span></span>|<span data-ttu-id="49f99-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49f99-153">Version of the device configuration.</span></span> <span data-ttu-id="49f99-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f99-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="49f99-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f99-155">Response</span></span>
<span data-ttu-id="49f99-156">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49f99-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f99-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49f99-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="49f99-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49f99-158">Request</span></span>
<span data-ttu-id="49f99-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49f99-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49f99-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f99-160">Response</span></span>
<span data-ttu-id="49f99-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49f99-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




