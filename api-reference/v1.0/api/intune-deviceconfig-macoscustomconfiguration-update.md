---
title: Atualizar macOSCustomConfiguration
description: Atualizar as propriedades de um objeto macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9faae3c3562c6ea3dddd0e1b0de6290becd63967
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997502"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="0d96e-103">Atualizar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d96e-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="0d96e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d96e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d96e-105">Atualizar as propriedades de um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d96e-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d96e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d96e-106">Prerequisites</span></span>
<span data-ttu-id="0d96e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d96e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d96e-109">Permission type</span></span>|<span data-ttu-id="0d96e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d96e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d96e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d96e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d96e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d96e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d96e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d96e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d96e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d96e-114">Not supported.</span></span>|
|<span data-ttu-id="0d96e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d96e-115">Application</span></span>|<span data-ttu-id="0d96e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d96e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d96e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d96e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0d96e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d96e-118">Request headers</span></span>
|<span data-ttu-id="0d96e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d96e-119">Header</span></span>|<span data-ttu-id="0d96e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0d96e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d96e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d96e-121">Authorization</span></span>|<span data-ttu-id="0d96e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d96e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d96e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d96e-123">Accept</span></span>|<span data-ttu-id="0d96e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0d96e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d96e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d96e-125">Request body</span></span>
<span data-ttu-id="0d96e-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d96e-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="0d96e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d96e-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="0d96e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d96e-128">Property</span></span>|<span data-ttu-id="0d96e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d96e-129">Type</span></span>|<span data-ttu-id="0d96e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d96e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d96e-131">id</span><span class="sxs-lookup"><span data-stu-id="0d96e-131">id</span></span>|<span data-ttu-id="0d96e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d96e-132">String</span></span>|<span data-ttu-id="0d96e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d96e-133">Key of the entity.</span></span> <span data-ttu-id="0d96e-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d96e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0d96e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d96e-136">DateTimeOffset</span></span>|<span data-ttu-id="0d96e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0d96e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0d96e-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d96e-139">createdDateTime</span></span>|<span data-ttu-id="0d96e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d96e-140">DateTimeOffset</span></span>|<span data-ttu-id="0d96e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0d96e-141">DateTime the object was created.</span></span> <span data-ttu-id="0d96e-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-143">descrição</span><span class="sxs-lookup"><span data-stu-id="0d96e-143">description</span></span>|<span data-ttu-id="0d96e-144">String</span><span class="sxs-lookup"><span data-stu-id="0d96e-144">String</span></span>|<span data-ttu-id="0d96e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d96e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d96e-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0d96e-147">displayName</span></span>|<span data-ttu-id="0d96e-148">String</span><span class="sxs-lookup"><span data-stu-id="0d96e-148">String</span></span>|<span data-ttu-id="0d96e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d96e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d96e-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-151">versão</span><span class="sxs-lookup"><span data-stu-id="0d96e-151">version</span></span>|<span data-ttu-id="0d96e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0d96e-152">Int32</span></span>|<span data-ttu-id="0d96e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d96e-153">Version of the device configuration.</span></span> <span data-ttu-id="0d96e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d96e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d96e-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="0d96e-155">payloadName</span></span>|<span data-ttu-id="0d96e-156">String</span><span class="sxs-lookup"><span data-stu-id="0d96e-156">String</span></span>|<span data-ttu-id="0d96e-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0d96e-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="0d96e-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="0d96e-158">payloadFileName</span></span>|<span data-ttu-id="0d96e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d96e-159">String</span></span>|<span data-ttu-id="0d96e-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="0d96e-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="0d96e-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="0d96e-161">\*.xml).</span></span>|
|<span data-ttu-id="0d96e-162">payload</span><span class="sxs-lookup"><span data-stu-id="0d96e-162">payload</span></span>|<span data-ttu-id="0d96e-163">Binária</span><span class="sxs-lookup"><span data-stu-id="0d96e-163">Binary</span></span>|<span data-ttu-id="0d96e-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="0d96e-164">Payload.</span></span> <span data-ttu-id="0d96e-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="0d96e-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="0d96e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d96e-166">Response</span></span>
<span data-ttu-id="0d96e-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d96e-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d96e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d96e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d96e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d96e-169">Request</span></span>
<span data-ttu-id="0d96e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d96e-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d96e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d96e-171">Response</span></span>
<span data-ttu-id="0d96e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d96e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



