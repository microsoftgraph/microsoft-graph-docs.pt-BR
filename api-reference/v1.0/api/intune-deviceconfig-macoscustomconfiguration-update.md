---
title: Atualizar macOSCustomConfiguration
description: Atualizar as propriedades de um objeto macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29d7ef8b896a6c47760a777c3b30e6c09a0642f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258909"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="28b2f-103">Atualizar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="28b2f-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="28b2f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28b2f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28b2f-105">Atualizar as propriedades de um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28b2f-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28b2f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28b2f-106">Prerequisites</span></span>
<span data-ttu-id="28b2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="28b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28b2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28b2f-109">Permission type</span></span>|<span data-ttu-id="28b2f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28b2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28b2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28b2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28b2f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b2f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28b2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28b2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28b2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b2f-114">Not supported.</span></span>|
|<span data-ttu-id="28b2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28b2f-115">Application</span></span>|<span data-ttu-id="28b2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b2f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28b2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28b2f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="28b2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28b2f-118">Request headers</span></span>
|<span data-ttu-id="28b2f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28b2f-119">Header</span></span>|<span data-ttu-id="28b2f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="28b2f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28b2f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="28b2f-121">Authorization</span></span>|<span data-ttu-id="28b2f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b2f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28b2f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28b2f-123">Accept</span></span>|<span data-ttu-id="28b2f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28b2f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28b2f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28b2f-125">Request body</span></span>
<span data-ttu-id="28b2f-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28b2f-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="28b2f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28b2f-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="28b2f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b2f-128">Property</span></span>|<span data-ttu-id="28b2f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b2f-129">Type</span></span>|<span data-ttu-id="28b2f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b2f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b2f-131">id</span><span class="sxs-lookup"><span data-stu-id="28b2f-131">id</span></span>|<span data-ttu-id="28b2f-132">String</span><span class="sxs-lookup"><span data-stu-id="28b2f-132">String</span></span>|<span data-ttu-id="28b2f-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="28b2f-133">Key of the entity.</span></span> <span data-ttu-id="28b2f-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28b2f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="28b2f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28b2f-136">DateTimeOffset</span></span>|<span data-ttu-id="28b2f-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="28b2f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="28b2f-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28b2f-139">createdDateTime</span></span>|<span data-ttu-id="28b2f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28b2f-140">DateTimeOffset</span></span>|<span data-ttu-id="28b2f-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="28b2f-141">DateTime the object was created.</span></span> <span data-ttu-id="28b2f-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-143">description</span><span class="sxs-lookup"><span data-stu-id="28b2f-143">description</span></span>|<span data-ttu-id="28b2f-144">String</span><span class="sxs-lookup"><span data-stu-id="28b2f-144">String</span></span>|<span data-ttu-id="28b2f-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="28b2f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28b2f-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="28b2f-147">displayName</span></span>|<span data-ttu-id="28b2f-148">String</span><span class="sxs-lookup"><span data-stu-id="28b2f-148">String</span></span>|<span data-ttu-id="28b2f-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="28b2f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28b2f-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-151">version</span><span class="sxs-lookup"><span data-stu-id="28b2f-151">version</span></span>|<span data-ttu-id="28b2f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="28b2f-152">Int32</span></span>|<span data-ttu-id="28b2f-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="28b2f-153">Version of the device configuration.</span></span> <span data-ttu-id="28b2f-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28b2f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28b2f-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="28b2f-155">payloadName</span></span>|<span data-ttu-id="28b2f-156">String</span><span class="sxs-lookup"><span data-stu-id="28b2f-156">String</span></span>|<span data-ttu-id="28b2f-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="28b2f-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="28b2f-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="28b2f-158">payloadFileName</span></span>|<span data-ttu-id="28b2f-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b2f-159">String</span></span>|<span data-ttu-id="28b2f-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="28b2f-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="28b2f-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="28b2f-161">\*.xml).</span></span>|
|<span data-ttu-id="28b2f-162">payload</span><span class="sxs-lookup"><span data-stu-id="28b2f-162">payload</span></span>|<span data-ttu-id="28b2f-163">Binária</span><span class="sxs-lookup"><span data-stu-id="28b2f-163">Binary</span></span>|<span data-ttu-id="28b2f-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="28b2f-164">Payload.</span></span> <span data-ttu-id="28b2f-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="28b2f-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="28b2f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b2f-166">Response</span></span>
<span data-ttu-id="28b2f-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28b2f-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28b2f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28b2f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="28b2f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b2f-169">Request</span></span>
<span data-ttu-id="28b2f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28b2f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28b2f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b2f-171">Response</span></span>
<span data-ttu-id="28b2f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28b2f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



