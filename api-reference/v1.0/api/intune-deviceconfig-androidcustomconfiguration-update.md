---
title: Atualizar androidCustomConfiguration
description: Atualiza as propriedades de um objeto androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1993068e374a6719cfdaff0ea76ec6fcf4bc1a46
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264208"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="c98d5-103">Atualizar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c98d5-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="c98d5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c98d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c98d5-105">Atualiza as propriedades de um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c98d5-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c98d5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c98d5-106">Prerequisites</span></span>
<span data-ttu-id="c98d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c98d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c98d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c98d5-109">Permission type</span></span>|<span data-ttu-id="c98d5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c98d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c98d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c98d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c98d5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c98d5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c98d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c98d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c98d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c98d5-114">Not supported.</span></span>|
|<span data-ttu-id="c98d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c98d5-115">Application</span></span>|<span data-ttu-id="c98d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c98d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c98d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c98d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c98d5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c98d5-118">Request headers</span></span>
|<span data-ttu-id="c98d5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c98d5-119">Header</span></span>|<span data-ttu-id="c98d5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c98d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c98d5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c98d5-121">Authorization</span></span>|<span data-ttu-id="c98d5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c98d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c98d5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c98d5-123">Accept</span></span>|<span data-ttu-id="c98d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c98d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c98d5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c98d5-125">Request body</span></span>
<span data-ttu-id="c98d5-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c98d5-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="c98d5-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c98d5-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="c98d5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c98d5-128">Property</span></span>|<span data-ttu-id="c98d5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c98d5-129">Type</span></span>|<span data-ttu-id="c98d5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c98d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c98d5-131">id</span><span class="sxs-lookup"><span data-stu-id="c98d5-131">id</span></span>|<span data-ttu-id="c98d5-132">String</span><span class="sxs-lookup"><span data-stu-id="c98d5-132">String</span></span>|<span data-ttu-id="c98d5-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c98d5-133">Key of the entity.</span></span> <span data-ttu-id="c98d5-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c98d5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c98d5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c98d5-136">DateTimeOffset</span></span>|<span data-ttu-id="c98d5-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c98d5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c98d5-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c98d5-139">createdDateTime</span></span>|<span data-ttu-id="c98d5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c98d5-140">DateTimeOffset</span></span>|<span data-ttu-id="c98d5-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c98d5-141">DateTime the object was created.</span></span> <span data-ttu-id="c98d5-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-143">description</span><span class="sxs-lookup"><span data-stu-id="c98d5-143">description</span></span>|<span data-ttu-id="c98d5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c98d5-144">String</span></span>|<span data-ttu-id="c98d5-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c98d5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c98d5-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c98d5-147">displayName</span></span>|<span data-ttu-id="c98d5-148">String</span><span class="sxs-lookup"><span data-stu-id="c98d5-148">String</span></span>|<span data-ttu-id="c98d5-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c98d5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c98d5-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-151">version</span><span class="sxs-lookup"><span data-stu-id="c98d5-151">version</span></span>|<span data-ttu-id="c98d5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c98d5-152">Int32</span></span>|<span data-ttu-id="c98d5-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c98d5-153">Version of the device configuration.</span></span> <span data-ttu-id="c98d5-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c98d5-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c98d5-155">omaSettings</span></span>|<span data-ttu-id="c98d5-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c98d5-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c98d5-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="c98d5-157">OMA settings.</span></span> <span data-ttu-id="c98d5-158">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="c98d5-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c98d5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98d5-159">Response</span></span>
<span data-ttu-id="c98d5-160">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c98d5-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c98d5-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c98d5-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="c98d5-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c98d5-162">Request</span></span>
<span data-ttu-id="c98d5-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c98d5-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="c98d5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98d5-164">Response</span></span>
<span data-ttu-id="c98d5-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c98d5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



