---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ff6c3782c9633e67f470121c825bf9a63db050c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959485"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="9b639-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b639-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="9b639-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b639-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b639-105">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b639-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b639-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b639-106">Prerequisites</span></span>
<span data-ttu-id="9b639-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b639-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b639-109">Permission type</span></span>|<span data-ttu-id="9b639-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b639-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b639-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b639-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b639-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b639-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b639-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b639-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b639-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b639-114">Not supported.</span></span>|
|<span data-ttu-id="9b639-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b639-115">Application</span></span>|<span data-ttu-id="9b639-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b639-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b639-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b639-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9b639-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b639-118">Request headers</span></span>
|<span data-ttu-id="9b639-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b639-119">Header</span></span>|<span data-ttu-id="9b639-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9b639-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b639-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b639-121">Authorization</span></span>|<span data-ttu-id="9b639-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b639-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b639-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b639-123">Accept</span></span>|<span data-ttu-id="9b639-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b639-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b639-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b639-125">Request body</span></span>
<span data-ttu-id="9b639-126">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9b639-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="9b639-127">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9b639-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="9b639-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b639-128">Property</span></span>|<span data-ttu-id="9b639-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b639-129">Type</span></span>|<span data-ttu-id="9b639-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b639-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b639-131">id</span><span class="sxs-lookup"><span data-stu-id="9b639-131">id</span></span>|<span data-ttu-id="9b639-132">String</span><span class="sxs-lookup"><span data-stu-id="9b639-132">String</span></span>|<span data-ttu-id="9b639-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b639-133">Key of the entity.</span></span> <span data-ttu-id="9b639-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b639-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9b639-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b639-136">DateTimeOffset</span></span>|<span data-ttu-id="9b639-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9b639-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9b639-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b639-139">createdDateTime</span></span>|<span data-ttu-id="9b639-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b639-140">DateTimeOffset</span></span>|<span data-ttu-id="9b639-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9b639-141">DateTime the object was created.</span></span> <span data-ttu-id="9b639-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-143">descrição</span><span class="sxs-lookup"><span data-stu-id="9b639-143">description</span></span>|<span data-ttu-id="9b639-144">String</span><span class="sxs-lookup"><span data-stu-id="9b639-144">String</span></span>|<span data-ttu-id="9b639-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b639-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b639-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9b639-147">displayName</span></span>|<span data-ttu-id="9b639-148">String</span><span class="sxs-lookup"><span data-stu-id="9b639-148">String</span></span>|<span data-ttu-id="9b639-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b639-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b639-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-151">versão</span><span class="sxs-lookup"><span data-stu-id="9b639-151">version</span></span>|<span data-ttu-id="9b639-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9b639-152">Int32</span></span>|<span data-ttu-id="9b639-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b639-153">Version of the device configuration.</span></span> <span data-ttu-id="9b639-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b639-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b639-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="9b639-155">payloadName</span></span>|<span data-ttu-id="9b639-156">String</span><span class="sxs-lookup"><span data-stu-id="9b639-156">String</span></span>|<span data-ttu-id="9b639-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9b639-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="9b639-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="9b639-158">payloadFileName</span></span>|<span data-ttu-id="9b639-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b639-159">String</span></span>|<span data-ttu-id="9b639-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="9b639-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="9b639-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="9b639-161">\*.xml).</span></span>|
|<span data-ttu-id="9b639-162">payload</span><span class="sxs-lookup"><span data-stu-id="9b639-162">payload</span></span>|<span data-ttu-id="9b639-163">Binária</span><span class="sxs-lookup"><span data-stu-id="9b639-163">Binary</span></span>|<span data-ttu-id="9b639-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="9b639-164">Payload.</span></span> <span data-ttu-id="9b639-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="9b639-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="9b639-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b639-166">Response</span></span>
<span data-ttu-id="9b639-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b639-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b639-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b639-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b639-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b639-169">Request</span></span>
<span data-ttu-id="9b639-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b639-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="9b639-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b639-171">Response</span></span>
<span data-ttu-id="9b639-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b639-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



