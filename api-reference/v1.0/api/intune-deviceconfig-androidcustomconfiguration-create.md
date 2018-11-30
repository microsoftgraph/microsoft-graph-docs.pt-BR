---
title: Criar androidCustomConfiguration
description: Criar um novo objeto androidCustomConfiguration.
ms.openlocfilehash: 7ce26b92d25f062a7dacb44a09ebe2250b680dd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007170"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="c86a9-103">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c86a9-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="c86a9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c86a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c86a9-105">Criar um novo objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c86a9-105">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c86a9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c86a9-106">Prerequisites</span></span>
<span data-ttu-id="c86a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c86a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c86a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c86a9-109">Permission type</span></span>|<span data-ttu-id="c86a9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c86a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c86a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c86a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c86a9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86a9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c86a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c86a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c86a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c86a9-114">Not supported.</span></span>|
|<span data-ttu-id="c86a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c86a9-115">Application</span></span>|<span data-ttu-id="c86a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c86a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c86a9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c86a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c86a9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c86a9-118">Request headers</span></span>
|<span data-ttu-id="c86a9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c86a9-119">Header</span></span>|<span data-ttu-id="c86a9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c86a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c86a9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c86a9-121">Authorization</span></span>|<span data-ttu-id="c86a9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c86a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c86a9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c86a9-123">Accept</span></span>|<span data-ttu-id="c86a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c86a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c86a9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c86a9-125">Request body</span></span>
<span data-ttu-id="c86a9-126">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c86a9-126">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="c86a9-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c86a9-127">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="c86a9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c86a9-128">Property</span></span>|<span data-ttu-id="c86a9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c86a9-129">Type</span></span>|<span data-ttu-id="c86a9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c86a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c86a9-131">id</span><span class="sxs-lookup"><span data-stu-id="c86a9-131">id</span></span>|<span data-ttu-id="c86a9-132">String</span><span class="sxs-lookup"><span data-stu-id="c86a9-132">String</span></span>|<span data-ttu-id="c86a9-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c86a9-133">Key of the entity.</span></span> <span data-ttu-id="c86a9-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c86a9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c86a9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86a9-136">DateTimeOffset</span></span>|<span data-ttu-id="c86a9-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c86a9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c86a9-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c86a9-139">createdDateTime</span></span>|<span data-ttu-id="c86a9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86a9-140">DateTimeOffset</span></span>|<span data-ttu-id="c86a9-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c86a9-141">DateTime the object was created.</span></span> <span data-ttu-id="c86a9-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-143">description</span><span class="sxs-lookup"><span data-stu-id="c86a9-143">description</span></span>|<span data-ttu-id="c86a9-144">String</span><span class="sxs-lookup"><span data-stu-id="c86a9-144">String</span></span>|<span data-ttu-id="c86a9-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c86a9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c86a9-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c86a9-147">displayName</span></span>|<span data-ttu-id="c86a9-148">String</span><span class="sxs-lookup"><span data-stu-id="c86a9-148">String</span></span>|<span data-ttu-id="c86a9-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c86a9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c86a9-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-151">version</span><span class="sxs-lookup"><span data-stu-id="c86a9-151">version</span></span>|<span data-ttu-id="c86a9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c86a9-152">Int32</span></span>|<span data-ttu-id="c86a9-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c86a9-153">Version of the device configuration.</span></span> <span data-ttu-id="c86a9-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c86a9-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c86a9-155">omaSettings</span></span>|<span data-ttu-id="c86a9-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c86a9-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c86a9-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="c86a9-157">OMA settings.</span></span> <span data-ttu-id="c86a9-158">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="c86a9-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c86a9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c86a9-159">Response</span></span>
<span data-ttu-id="c86a9-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c86a9-160">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c86a9-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c86a9-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="c86a9-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c86a9-162">Request</span></span>
<span data-ttu-id="c86a9-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c86a9-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c86a9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c86a9-164">Response</span></span>
<span data-ttu-id="c86a9-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c86a9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



