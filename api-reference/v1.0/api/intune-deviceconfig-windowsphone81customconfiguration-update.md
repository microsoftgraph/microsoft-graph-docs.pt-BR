---
title: Atualizar windowsPhone81CustomConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8df2884a3c7ebbcbce729f279ca9509c318cf84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957323"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="fd696-103">Atualizar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd696-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="fd696-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd696-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd696-105">Atualizar as propriedades de um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd696-105">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd696-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd696-106">Prerequisites</span></span>
<span data-ttu-id="fd696-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd696-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd696-109">Permission type</span></span>|<span data-ttu-id="fd696-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd696-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd696-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd696-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd696-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd696-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd696-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd696-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd696-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd696-114">Not supported.</span></span>|
|<span data-ttu-id="fd696-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd696-115">Application</span></span>|<span data-ttu-id="fd696-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd696-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd696-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd696-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fd696-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd696-118">Request headers</span></span>
|<span data-ttu-id="fd696-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd696-119">Header</span></span>|<span data-ttu-id="fd696-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fd696-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd696-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd696-121">Authorization</span></span>|<span data-ttu-id="fd696-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd696-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd696-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd696-123">Accept</span></span>|<span data-ttu-id="fd696-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd696-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd696-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd696-125">Request body</span></span>
<span data-ttu-id="fd696-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd696-126">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="fd696-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd696-127">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="fd696-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd696-128">Property</span></span>|<span data-ttu-id="fd696-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd696-129">Type</span></span>|<span data-ttu-id="fd696-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd696-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd696-131">id</span><span class="sxs-lookup"><span data-stu-id="fd696-131">id</span></span>|<span data-ttu-id="fd696-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd696-132">String</span></span>|<span data-ttu-id="fd696-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd696-133">Key of the entity.</span></span> <span data-ttu-id="fd696-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd696-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fd696-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd696-136">DateTimeOffset</span></span>|<span data-ttu-id="fd696-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fd696-137">DateTime the object was last modified.</span></span> <span data-ttu-id="fd696-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd696-139">createdDateTime</span></span>|<span data-ttu-id="fd696-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd696-140">DateTimeOffset</span></span>|<span data-ttu-id="fd696-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fd696-141">DateTime the object was created.</span></span> <span data-ttu-id="fd696-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-143">description</span><span class="sxs-lookup"><span data-stu-id="fd696-143">description</span></span>|<span data-ttu-id="fd696-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd696-144">String</span></span>|<span data-ttu-id="fd696-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd696-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fd696-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-147">displayName</span><span class="sxs-lookup"><span data-stu-id="fd696-147">displayName</span></span>|<span data-ttu-id="fd696-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd696-148">String</span></span>|<span data-ttu-id="fd696-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd696-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fd696-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-151">version</span><span class="sxs-lookup"><span data-stu-id="fd696-151">version</span></span>|<span data-ttu-id="fd696-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fd696-152">Int32</span></span>|<span data-ttu-id="fd696-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd696-153">Version of the device configuration.</span></span> <span data-ttu-id="fd696-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd696-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="fd696-155">omaSettings</span></span>|<span data-ttu-id="fd696-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd696-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="fd696-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="fd696-157">OMA settings.</span></span> <span data-ttu-id="fd696-158">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="fd696-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fd696-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd696-159">Response</span></span>
<span data-ttu-id="fd696-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd696-160">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd696-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd696-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd696-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd696-162">Request</span></span>
<span data-ttu-id="fd696-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd696-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="fd696-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd696-164">Response</span></span>
<span data-ttu-id="fd696-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd696-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



