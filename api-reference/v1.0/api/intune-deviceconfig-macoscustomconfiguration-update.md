---
title: Atualizar macOSCustomConfiguration
description: Atualizar as propriedades de um objeto macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 733428184ccca9dafbf343683c296708ef016ccb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809524"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="796ee-103">Atualizar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="796ee-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="796ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="796ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="796ee-105">Atualizar as propriedades de um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="796ee-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="796ee-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="796ee-106">Prerequisites</span></span>
<span data-ttu-id="796ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="796ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="796ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="796ee-109">Permission type</span></span>|<span data-ttu-id="796ee-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="796ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="796ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="796ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="796ee-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796ee-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="796ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="796ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="796ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="796ee-114">Not supported.</span></span>|
|<span data-ttu-id="796ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="796ee-115">Application</span></span>|<span data-ttu-id="796ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="796ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="796ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="796ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="796ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="796ee-118">Request headers</span></span>
|<span data-ttu-id="796ee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="796ee-119">Header</span></span>|<span data-ttu-id="796ee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="796ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="796ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="796ee-121">Authorization</span></span>|<span data-ttu-id="796ee-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="796ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="796ee-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="796ee-123">Accept</span></span>|<span data-ttu-id="796ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="796ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="796ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="796ee-125">Request body</span></span>
<span data-ttu-id="796ee-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="796ee-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="796ee-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="796ee-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="796ee-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="796ee-128">Property</span></span>|<span data-ttu-id="796ee-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="796ee-129">Type</span></span>|<span data-ttu-id="796ee-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="796ee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="796ee-131">id</span><span class="sxs-lookup"><span data-stu-id="796ee-131">id</span></span>|<span data-ttu-id="796ee-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="796ee-132">String</span></span>|<span data-ttu-id="796ee-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="796ee-133">Key of the entity.</span></span> <span data-ttu-id="796ee-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="796ee-135">lastModifiedDateTime</span></span>|<span data-ttu-id="796ee-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796ee-136">DateTimeOffset</span></span>|<span data-ttu-id="796ee-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="796ee-137">DateTime the object was last modified.</span></span> <span data-ttu-id="796ee-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="796ee-139">createdDateTime</span></span>|<span data-ttu-id="796ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796ee-140">DateTimeOffset</span></span>|<span data-ttu-id="796ee-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="796ee-141">DateTime the object was created.</span></span> <span data-ttu-id="796ee-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-143">description</span><span class="sxs-lookup"><span data-stu-id="796ee-143">description</span></span>|<span data-ttu-id="796ee-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="796ee-144">String</span></span>|<span data-ttu-id="796ee-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="796ee-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="796ee-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-147">displayName</span><span class="sxs-lookup"><span data-stu-id="796ee-147">displayName</span></span>|<span data-ttu-id="796ee-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="796ee-148">String</span></span>|<span data-ttu-id="796ee-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="796ee-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="796ee-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-151">version</span><span class="sxs-lookup"><span data-stu-id="796ee-151">version</span></span>|<span data-ttu-id="796ee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="796ee-152">Int32</span></span>|<span data-ttu-id="796ee-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="796ee-153">Version of the device configuration.</span></span> <span data-ttu-id="796ee-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="796ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="796ee-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="796ee-155">payloadName</span></span>|<span data-ttu-id="796ee-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="796ee-156">String</span></span>|<span data-ttu-id="796ee-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="796ee-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="796ee-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="796ee-158">payloadFileName</span></span>|<span data-ttu-id="796ee-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="796ee-159">String</span></span>|<span data-ttu-id="796ee-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="796ee-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="796ee-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="796ee-161">\*.xml).</span></span>|
|<span data-ttu-id="796ee-162">payload</span><span class="sxs-lookup"><span data-stu-id="796ee-162">payload</span></span>|<span data-ttu-id="796ee-163">Binária</span><span class="sxs-lookup"><span data-stu-id="796ee-163">Binary</span></span>|<span data-ttu-id="796ee-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="796ee-164">Payload.</span></span> <span data-ttu-id="796ee-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="796ee-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="796ee-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="796ee-166">Response</span></span>
<span data-ttu-id="796ee-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="796ee-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="796ee-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="796ee-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="796ee-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="796ee-169">Request</span></span>
<span data-ttu-id="796ee-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="796ee-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="796ee-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="796ee-171">Response</span></span>
<span data-ttu-id="796ee-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="796ee-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



