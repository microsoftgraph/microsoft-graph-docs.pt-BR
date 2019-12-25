---
title: Atualizar androidCustomConfiguration
description: Atualiza as propriedades de um objeto androidCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75080639484fc13ec37958e15c4823d86d8bbb4c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37354508"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="cbc44-103">Atualizar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="cbc44-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="cbc44-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbc44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbc44-105">Atualiza as propriedades de um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc44-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbc44-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbc44-106">Prerequisites</span></span>
<span data-ttu-id="cbc44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbc44-109">Permission type</span></span>|<span data-ttu-id="cbc44-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbc44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc44-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbc44-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbc44-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbc44-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbc44-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbc44-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbc44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc44-114">Not supported.</span></span>|
|<span data-ttu-id="cbc44-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbc44-115">Application</span></span>|<span data-ttu-id="cbc44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc44-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbc44-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc44-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cbc44-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc44-118">Request headers</span></span>
|<span data-ttu-id="cbc44-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbc44-119">Header</span></span>|<span data-ttu-id="cbc44-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cbc44-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbc44-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbc44-121">Authorization</span></span>|<span data-ttu-id="cbc44-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbc44-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbc44-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbc44-123">Accept</span></span>|<span data-ttu-id="cbc44-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbc44-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc44-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc44-125">Request body</span></span>
<span data-ttu-id="cbc44-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc44-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="cbc44-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cbc44-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="cbc44-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbc44-128">Property</span></span>|<span data-ttu-id="cbc44-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbc44-129">Type</span></span>|<span data-ttu-id="cbc44-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbc44-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbc44-131">id</span><span class="sxs-lookup"><span data-stu-id="cbc44-131">id</span></span>|<span data-ttu-id="cbc44-132">String</span><span class="sxs-lookup"><span data-stu-id="cbc44-132">String</span></span>|<span data-ttu-id="cbc44-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cbc44-133">Key of the entity.</span></span> <span data-ttu-id="cbc44-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc44-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cbc44-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc44-136">DateTimeOffset</span></span>|<span data-ttu-id="cbc44-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cbc44-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cbc44-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc44-139">createdDateTime</span></span>|<span data-ttu-id="cbc44-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc44-140">DateTimeOffset</span></span>|<span data-ttu-id="cbc44-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cbc44-141">DateTime the object was created.</span></span> <span data-ttu-id="cbc44-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-143">descrição</span><span class="sxs-lookup"><span data-stu-id="cbc44-143">description</span></span>|<span data-ttu-id="cbc44-144">String</span><span class="sxs-lookup"><span data-stu-id="cbc44-144">String</span></span>|<span data-ttu-id="cbc44-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbc44-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cbc44-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cbc44-147">displayName</span></span>|<span data-ttu-id="cbc44-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbc44-148">String</span></span>|<span data-ttu-id="cbc44-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbc44-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cbc44-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-151">versão</span><span class="sxs-lookup"><span data-stu-id="cbc44-151">version</span></span>|<span data-ttu-id="cbc44-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cbc44-152">Int32</span></span>|<span data-ttu-id="cbc44-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbc44-153">Version of the device configuration.</span></span> <span data-ttu-id="cbc44-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cbc44-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="cbc44-155">omaSettings</span></span>|<span data-ttu-id="cbc44-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cbc44-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="cbc44-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="cbc44-157">OMA settings.</span></span> <span data-ttu-id="cbc44-158">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="cbc44-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="cbc44-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc44-159">Response</span></span>
<span data-ttu-id="cbc44-160">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc44-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc44-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbc44-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbc44-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc44-162">Request</span></span>
<span data-ttu-id="cbc44-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbc44-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbc44-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc44-164">Response</span></span>
<span data-ttu-id="cbc44-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbc44-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




