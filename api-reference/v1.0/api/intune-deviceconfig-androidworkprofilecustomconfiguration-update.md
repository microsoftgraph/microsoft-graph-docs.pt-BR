---
title: Atualizar androidWorkProfileCustomConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 668304adc0b3dcdfab076603767c1d46e4198d21
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019475"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="75f01-103">Atualizar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="75f01-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="75f01-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75f01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f01-105">Atualiza as propriedades de um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="75f01-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75f01-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75f01-106">Prerequisites</span></span>
<span data-ttu-id="75f01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75f01-109">Permission type</span></span>|<span data-ttu-id="75f01-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75f01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f01-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75f01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75f01-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f01-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75f01-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75f01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f01-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75f01-114">Not supported.</span></span>|
|<span data-ttu-id="75f01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75f01-115">Application</span></span>|<span data-ttu-id="75f01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75f01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f01-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75f01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="75f01-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75f01-118">Request headers</span></span>
|<span data-ttu-id="75f01-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75f01-119">Header</span></span>|<span data-ttu-id="75f01-120">Valor</span><span class="sxs-lookup"><span data-stu-id="75f01-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75f01-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="75f01-121">Authorization</span></span>|<span data-ttu-id="75f01-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75f01-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75f01-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75f01-123">Accept</span></span>|<span data-ttu-id="75f01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="75f01-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f01-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75f01-125">Request body</span></span>
<span data-ttu-id="75f01-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="75f01-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="75f01-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75f01-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="75f01-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75f01-128">Property</span></span>|<span data-ttu-id="75f01-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="75f01-129">Type</span></span>|<span data-ttu-id="75f01-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="75f01-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f01-131">id</span><span class="sxs-lookup"><span data-stu-id="75f01-131">id</span></span>|<span data-ttu-id="75f01-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75f01-132">String</span></span>|<span data-ttu-id="75f01-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75f01-133">Key of the entity.</span></span> <span data-ttu-id="75f01-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75f01-135">lastModifiedDateTime</span></span>|<span data-ttu-id="75f01-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75f01-136">DateTimeOffset</span></span>|<span data-ttu-id="75f01-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="75f01-137">DateTime the object was last modified.</span></span> <span data-ttu-id="75f01-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75f01-139">createdDateTime</span></span>|<span data-ttu-id="75f01-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75f01-140">DateTimeOffset</span></span>|<span data-ttu-id="75f01-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="75f01-141">DateTime the object was created.</span></span> <span data-ttu-id="75f01-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-143">descrição</span><span class="sxs-lookup"><span data-stu-id="75f01-143">description</span></span>|<span data-ttu-id="75f01-144">String</span><span class="sxs-lookup"><span data-stu-id="75f01-144">String</span></span>|<span data-ttu-id="75f01-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75f01-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75f01-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-147">displayName</span><span class="sxs-lookup"><span data-stu-id="75f01-147">displayName</span></span>|<span data-ttu-id="75f01-148">String</span><span class="sxs-lookup"><span data-stu-id="75f01-148">String</span></span>|<span data-ttu-id="75f01-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75f01-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75f01-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-151">versão</span><span class="sxs-lookup"><span data-stu-id="75f01-151">version</span></span>|<span data-ttu-id="75f01-152">Int32</span><span class="sxs-lookup"><span data-stu-id="75f01-152">Int32</span></span>|<span data-ttu-id="75f01-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75f01-153">Version of the device configuration.</span></span> <span data-ttu-id="75f01-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75f01-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="75f01-155">omaSettings</span></span>|<span data-ttu-id="75f01-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="75f01-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="75f01-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="75f01-157">OMA settings.</span></span> <span data-ttu-id="75f01-158">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="75f01-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="75f01-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="75f01-159">Response</span></span>
<span data-ttu-id="75f01-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75f01-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75f01-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75f01-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="75f01-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75f01-162">Request</span></span>
<span data-ttu-id="75f01-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75f01-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75f01-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="75f01-164">Response</span></span>
<span data-ttu-id="75f01-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75f01-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



