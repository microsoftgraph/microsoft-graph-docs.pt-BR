---
title: Atualizar androidWorkProfileCustomConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61800aadbb996a64131798e7394e4f581d2b3b6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401165"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="e602e-103">Atualizar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e602e-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="e602e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e602e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e602e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e602e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e602e-106">Atualiza as propriedades de um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e602e-106">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e602e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e602e-107">Prerequisites</span></span>
<span data-ttu-id="e602e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e602e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e602e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e602e-110">Permission type</span></span>|<span data-ttu-id="e602e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e602e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e602e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e602e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e602e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e602e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e602e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e602e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e602e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e602e-115">Not supported.</span></span>|
|<span data-ttu-id="e602e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e602e-116">Application</span></span>|<span data-ttu-id="e602e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e602e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e602e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e602e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e602e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e602e-119">Request headers</span></span>
|<span data-ttu-id="e602e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e602e-120">Header</span></span>|<span data-ttu-id="e602e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e602e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e602e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e602e-122">Authorization</span></span>|<span data-ttu-id="e602e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e602e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e602e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e602e-124">Accept</span></span>|<span data-ttu-id="e602e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e602e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e602e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e602e-126">Request body</span></span>
<span data-ttu-id="e602e-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e602e-127">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="e602e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e602e-128">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="e602e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e602e-129">Property</span></span>|<span data-ttu-id="e602e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e602e-130">Type</span></span>|<span data-ttu-id="e602e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e602e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e602e-132">id</span><span class="sxs-lookup"><span data-stu-id="e602e-132">id</span></span>|<span data-ttu-id="e602e-133">String</span><span class="sxs-lookup"><span data-stu-id="e602e-133">String</span></span>|<span data-ttu-id="e602e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e602e-134">Key of the entity.</span></span> <span data-ttu-id="e602e-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e602e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e602e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e602e-137">DateTimeOffset</span></span>|<span data-ttu-id="e602e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e602e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e602e-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e602e-140">createdDateTime</span></span>|<span data-ttu-id="e602e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e602e-141">DateTimeOffset</span></span>|<span data-ttu-id="e602e-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e602e-142">DateTime the object was created.</span></span> <span data-ttu-id="e602e-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-144">description</span><span class="sxs-lookup"><span data-stu-id="e602e-144">description</span></span>|<span data-ttu-id="e602e-145">String</span><span class="sxs-lookup"><span data-stu-id="e602e-145">String</span></span>|<span data-ttu-id="e602e-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e602e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e602e-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e602e-148">displayName</span></span>|<span data-ttu-id="e602e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e602e-149">String</span></span>|<span data-ttu-id="e602e-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e602e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e602e-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-152">versão</span><span class="sxs-lookup"><span data-stu-id="e602e-152">version</span></span>|<span data-ttu-id="e602e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e602e-153">Int32</span></span>|<span data-ttu-id="e602e-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e602e-154">Version of the device configuration.</span></span> <span data-ttu-id="e602e-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e602e-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e602e-156">omaSettings</span></span>|<span data-ttu-id="e602e-157">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e602e-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e602e-158">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="e602e-158">OMA settings.</span></span> <span data-ttu-id="e602e-159">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e602e-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e602e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e602e-160">Response</span></span>
<span data-ttu-id="e602e-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e602e-161">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e602e-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e602e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e602e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e602e-163">Request</span></span>
<span data-ttu-id="e602e-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e602e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e602e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e602e-165">Response</span></span>
<span data-ttu-id="e602e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e602e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```






