---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90583d103211f374ed761813a033000546fbc036
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514393"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="b2780-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2780-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="b2780-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2780-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2780-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2780-106">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2780-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2780-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2780-107">Prerequisites</span></span>
<span data-ttu-id="b2780-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2780-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2780-110">Permission type</span></span>|<span data-ttu-id="b2780-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2780-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2780-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2780-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2780-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2780-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2780-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2780-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2780-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2780-115">Not supported.</span></span>|
|<span data-ttu-id="b2780-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2780-116">Application</span></span>|<span data-ttu-id="b2780-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2780-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2780-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2780-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b2780-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2780-119">Request headers</span></span>
|<span data-ttu-id="b2780-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2780-120">Header</span></span>|<span data-ttu-id="b2780-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2780-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2780-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2780-122">Authorization</span></span>|<span data-ttu-id="b2780-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2780-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2780-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2780-124">Accept</span></span>|<span data-ttu-id="b2780-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2780-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2780-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2780-126">Request body</span></span>
<span data-ttu-id="b2780-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b2780-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="b2780-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b2780-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="b2780-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2780-129">Property</span></span>|<span data-ttu-id="b2780-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2780-130">Type</span></span>|<span data-ttu-id="b2780-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2780-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2780-132">id</span><span class="sxs-lookup"><span data-stu-id="b2780-132">id</span></span>|<span data-ttu-id="b2780-133">String</span><span class="sxs-lookup"><span data-stu-id="b2780-133">String</span></span>|<span data-ttu-id="b2780-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2780-134">Key of the entity.</span></span> <span data-ttu-id="b2780-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2780-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b2780-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2780-137">DateTimeOffset</span></span>|<span data-ttu-id="b2780-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b2780-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b2780-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2780-140">createdDateTime</span></span>|<span data-ttu-id="b2780-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2780-141">DateTimeOffset</span></span>|<span data-ttu-id="b2780-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2780-142">DateTime the object was created.</span></span> <span data-ttu-id="b2780-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-144">description</span><span class="sxs-lookup"><span data-stu-id="b2780-144">description</span></span>|<span data-ttu-id="b2780-145">String</span><span class="sxs-lookup"><span data-stu-id="b2780-145">String</span></span>|<span data-ttu-id="b2780-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2780-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2780-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b2780-148">displayName</span></span>|<span data-ttu-id="b2780-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2780-149">String</span></span>|<span data-ttu-id="b2780-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2780-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2780-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-152">versão</span><span class="sxs-lookup"><span data-stu-id="b2780-152">version</span></span>|<span data-ttu-id="b2780-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b2780-153">Int32</span></span>|<span data-ttu-id="b2780-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2780-154">Version of the device configuration.</span></span> <span data-ttu-id="b2780-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2780-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2780-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="b2780-156">payloadName</span></span>|<span data-ttu-id="b2780-157">String</span><span class="sxs-lookup"><span data-stu-id="b2780-157">String</span></span>|<span data-ttu-id="b2780-158">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b2780-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="b2780-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="b2780-159">payloadFileName</span></span>|<span data-ttu-id="b2780-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2780-160">String</span></span>|<span data-ttu-id="b2780-161">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="b2780-161">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="b2780-162">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="b2780-162">\*.xml).</span></span>|
|<span data-ttu-id="b2780-163">payload</span><span class="sxs-lookup"><span data-stu-id="b2780-163">payload</span></span>|<span data-ttu-id="b2780-164">Binária</span><span class="sxs-lookup"><span data-stu-id="b2780-164">Binary</span></span>|<span data-ttu-id="b2780-165">Carga.</span><span class="sxs-lookup"><span data-stu-id="b2780-165">Payload.</span></span> <span data-ttu-id="b2780-166">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="b2780-166">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="b2780-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2780-167">Response</span></span>
<span data-ttu-id="b2780-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2780-168">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2780-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2780-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2780-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2780-170">Request</span></span>
<span data-ttu-id="b2780-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2780-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2780-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2780-172">Response</span></span>
<span data-ttu-id="b2780-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2780-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




