---
title: Criar iosCustomConfiguration
description: Cria um novo objeto iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51ae9c2755a6de77950769f3bf7550025662b58a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473753"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="35f94-103">Criar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="35f94-103">Create iosCustomConfiguration</span></span>

<span data-ttu-id="35f94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35f94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f94-106">Cria um novo objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f94-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35f94-107">Prerequisites</span></span>
<span data-ttu-id="35f94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35f94-110">Permission type</span></span>|<span data-ttu-id="35f94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35f94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35f94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35f94-115">Not supported.</span></span>|
|<span data-ttu-id="35f94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35f94-116">Application</span></span>|<span data-ttu-id="35f94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35f94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35f94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35f94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35f94-119">Request headers</span></span>
|<span data-ttu-id="35f94-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35f94-120">Header</span></span>|<span data-ttu-id="35f94-121">Valor</span><span class="sxs-lookup"><span data-stu-id="35f94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="35f94-122">Authorization</span></span>|<span data-ttu-id="35f94-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f94-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35f94-124">Accept</span></span>|<span data-ttu-id="35f94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35f94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35f94-126">Request body</span></span>
<span data-ttu-id="35f94-127">No corpo da solicitação, forneça uma representação JSON do objeto iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35f94-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="35f94-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35f94-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="35f94-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35f94-129">Property</span></span>|<span data-ttu-id="35f94-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="35f94-130">Type</span></span>|<span data-ttu-id="35f94-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f94-132">id</span><span class="sxs-lookup"><span data-stu-id="35f94-132">id</span></span>|<span data-ttu-id="35f94-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f94-133">String</span></span>|<span data-ttu-id="35f94-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35f94-134">Key of the entity.</span></span> <span data-ttu-id="35f94-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35f94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="35f94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f94-137">DateTimeOffset</span></span>|<span data-ttu-id="35f94-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="35f94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="35f94-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35f94-140">createdDateTime</span></span>|<span data-ttu-id="35f94-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f94-141">DateTimeOffset</span></span>|<span data-ttu-id="35f94-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="35f94-142">DateTime the object was created.</span></span> <span data-ttu-id="35f94-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-144">description</span><span class="sxs-lookup"><span data-stu-id="35f94-144">description</span></span>|<span data-ttu-id="35f94-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f94-145">String</span></span>|<span data-ttu-id="35f94-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35f94-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35f94-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-148">displayName</span><span class="sxs-lookup"><span data-stu-id="35f94-148">displayName</span></span>|<span data-ttu-id="35f94-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f94-149">String</span></span>|<span data-ttu-id="35f94-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35f94-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35f94-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-152">versão</span><span class="sxs-lookup"><span data-stu-id="35f94-152">version</span></span>|<span data-ttu-id="35f94-153">Int32</span><span class="sxs-lookup"><span data-stu-id="35f94-153">Int32</span></span>|<span data-ttu-id="35f94-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35f94-154">Version of the device configuration.</span></span> <span data-ttu-id="35f94-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f94-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f94-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="35f94-156">payloadName</span></span>|<span data-ttu-id="35f94-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f94-157">String</span></span>|<span data-ttu-id="35f94-158">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="35f94-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="35f94-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="35f94-159">payloadFileName</span></span>|<span data-ttu-id="35f94-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f94-160">String</span></span>|<span data-ttu-id="35f94-161">Nome do arquivo de carga (\*.mobileconfig \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="35f94-161">Payload file name (\*.mobileconfig \| \*.xml).</span></span>|
|<span data-ttu-id="35f94-162">payload</span><span class="sxs-lookup"><span data-stu-id="35f94-162">payload</span></span>|<span data-ttu-id="35f94-163">Binária</span><span class="sxs-lookup"><span data-stu-id="35f94-163">Binary</span></span>|<span data-ttu-id="35f94-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="35f94-164">Payload.</span></span> <span data-ttu-id="35f94-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="35f94-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="35f94-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="35f94-166">Response</span></span>
<span data-ttu-id="35f94-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35f94-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f94-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35f94-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f94-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35f94-169">Request</span></span>
<span data-ttu-id="35f94-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f94-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="35f94-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="35f94-171">Response</span></span>
<span data-ttu-id="35f94-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35f94-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









