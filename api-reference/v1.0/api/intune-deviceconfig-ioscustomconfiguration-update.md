---
title: Atualizar iosCustomConfiguration
description: Atualizar as propriedades de um objeto iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e410fee8eeefe4dbb1018e921e0aac77b8f23369
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552799"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="de9d8-103">Atualizar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="de9d8-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="de9d8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de9d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de9d8-105">Atualizar as propriedades de um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de9d8-105">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de9d8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de9d8-106">Prerequisites</span></span>
<span data-ttu-id="de9d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de9d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de9d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de9d8-109">Permission type</span></span>|<span data-ttu-id="de9d8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de9d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de9d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de9d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de9d8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de9d8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de9d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de9d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de9d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de9d8-114">Not supported.</span></span>|
|<span data-ttu-id="de9d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de9d8-115">Application</span></span>|<span data-ttu-id="de9d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de9d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de9d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de9d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="de9d8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de9d8-118">Request headers</span></span>
|<span data-ttu-id="de9d8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de9d8-119">Header</span></span>|<span data-ttu-id="de9d8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="de9d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de9d8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de9d8-121">Authorization</span></span>|<span data-ttu-id="de9d8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de9d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de9d8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de9d8-123">Accept</span></span>|<span data-ttu-id="de9d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de9d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de9d8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de9d8-125">Request body</span></span>
<span data-ttu-id="de9d8-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de9d8-126">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="de9d8-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de9d8-127">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="de9d8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de9d8-128">Property</span></span>|<span data-ttu-id="de9d8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="de9d8-129">Type</span></span>|<span data-ttu-id="de9d8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="de9d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de9d8-131">id</span><span class="sxs-lookup"><span data-stu-id="de9d8-131">id</span></span>|<span data-ttu-id="de9d8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de9d8-132">String</span></span>|<span data-ttu-id="de9d8-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de9d8-133">Key of the entity.</span></span> <span data-ttu-id="de9d8-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de9d8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="de9d8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de9d8-136">DateTimeOffset</span></span>|<span data-ttu-id="de9d8-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="de9d8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="de9d8-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de9d8-139">createdDateTime</span></span>|<span data-ttu-id="de9d8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de9d8-140">DateTimeOffset</span></span>|<span data-ttu-id="de9d8-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="de9d8-141">DateTime the object was created.</span></span> <span data-ttu-id="de9d8-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-143">description</span><span class="sxs-lookup"><span data-stu-id="de9d8-143">description</span></span>|<span data-ttu-id="de9d8-144">String</span><span class="sxs-lookup"><span data-stu-id="de9d8-144">String</span></span>|<span data-ttu-id="de9d8-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de9d8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de9d8-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="de9d8-147">displayName</span></span>|<span data-ttu-id="de9d8-148">String</span><span class="sxs-lookup"><span data-stu-id="de9d8-148">String</span></span>|<span data-ttu-id="de9d8-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de9d8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de9d8-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-151">versão</span><span class="sxs-lookup"><span data-stu-id="de9d8-151">version</span></span>|<span data-ttu-id="de9d8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="de9d8-152">Int32</span></span>|<span data-ttu-id="de9d8-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de9d8-153">Version of the device configuration.</span></span> <span data-ttu-id="de9d8-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de9d8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de9d8-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="de9d8-155">payloadName</span></span>|<span data-ttu-id="de9d8-156">String</span><span class="sxs-lookup"><span data-stu-id="de9d8-156">String</span></span>|<span data-ttu-id="de9d8-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="de9d8-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="de9d8-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="de9d8-158">payloadFileName</span></span>|<span data-ttu-id="de9d8-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de9d8-159">String</span></span>|<span data-ttu-id="de9d8-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="de9d8-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="de9d8-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="de9d8-161">\*.xml).</span></span>|
|<span data-ttu-id="de9d8-162">payload</span><span class="sxs-lookup"><span data-stu-id="de9d8-162">payload</span></span>|<span data-ttu-id="de9d8-163">Binária</span><span class="sxs-lookup"><span data-stu-id="de9d8-163">Binary</span></span>|<span data-ttu-id="de9d8-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="de9d8-164">Payload.</span></span> <span data-ttu-id="de9d8-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="de9d8-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="de9d8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="de9d8-166">Response</span></span>
<span data-ttu-id="de9d8-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de9d8-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de9d8-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de9d8-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="de9d8-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de9d8-169">Request</span></span>
<span data-ttu-id="de9d8-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de9d8-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="de9d8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="de9d8-171">Response</span></span>
<span data-ttu-id="de9d8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de9d8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



