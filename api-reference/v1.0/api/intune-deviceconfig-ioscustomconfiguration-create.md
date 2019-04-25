---
title: Criar iosCustomConfiguration
description: Cria um novo objeto iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 594583d77c271f47fa99facb7551991a8e73f5d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552900"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="c40f2-103">Criar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40f2-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="c40f2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c40f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c40f2-105">Cria um novo objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c40f2-105">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c40f2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c40f2-106">Prerequisites</span></span>
<span data-ttu-id="c40f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c40f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c40f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c40f2-109">Permission type</span></span>|<span data-ttu-id="c40f2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c40f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c40f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c40f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c40f2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40f2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c40f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c40f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c40f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c40f2-114">Not supported.</span></span>|
|<span data-ttu-id="c40f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c40f2-115">Application</span></span>|<span data-ttu-id="c40f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c40f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c40f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c40f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c40f2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c40f2-118">Request headers</span></span>
|<span data-ttu-id="c40f2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c40f2-119">Header</span></span>|<span data-ttu-id="c40f2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c40f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c40f2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c40f2-121">Authorization</span></span>|<span data-ttu-id="c40f2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c40f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c40f2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c40f2-123">Accept</span></span>|<span data-ttu-id="c40f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c40f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c40f2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c40f2-125">Request body</span></span>
<span data-ttu-id="c40f2-126">No corpo da solicitação, forneça uma representação JSON do objeto iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c40f2-126">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="c40f2-127">A tabela a seguir mostra as propriedades que são necessárias ao criar iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c40f2-127">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="c40f2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c40f2-128">Property</span></span>|<span data-ttu-id="c40f2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c40f2-129">Type</span></span>|<span data-ttu-id="c40f2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c40f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40f2-131">id</span><span class="sxs-lookup"><span data-stu-id="c40f2-131">id</span></span>|<span data-ttu-id="c40f2-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40f2-132">String</span></span>|<span data-ttu-id="c40f2-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c40f2-133">Key of the entity.</span></span> <span data-ttu-id="c40f2-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c40f2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c40f2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40f2-136">DateTimeOffset</span></span>|<span data-ttu-id="c40f2-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c40f2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c40f2-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c40f2-139">createdDateTime</span></span>|<span data-ttu-id="c40f2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40f2-140">DateTimeOffset</span></span>|<span data-ttu-id="c40f2-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c40f2-141">DateTime the object was created.</span></span> <span data-ttu-id="c40f2-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-143">description</span><span class="sxs-lookup"><span data-stu-id="c40f2-143">description</span></span>|<span data-ttu-id="c40f2-144">String</span><span class="sxs-lookup"><span data-stu-id="c40f2-144">String</span></span>|<span data-ttu-id="c40f2-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40f2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c40f2-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c40f2-147">displayName</span></span>|<span data-ttu-id="c40f2-148">String</span><span class="sxs-lookup"><span data-stu-id="c40f2-148">String</span></span>|<span data-ttu-id="c40f2-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40f2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c40f2-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-151">versão</span><span class="sxs-lookup"><span data-stu-id="c40f2-151">version</span></span>|<span data-ttu-id="c40f2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c40f2-152">Int32</span></span>|<span data-ttu-id="c40f2-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c40f2-153">Version of the device configuration.</span></span> <span data-ttu-id="c40f2-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c40f2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c40f2-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="c40f2-155">payloadName</span></span>|<span data-ttu-id="c40f2-156">String</span><span class="sxs-lookup"><span data-stu-id="c40f2-156">String</span></span>|<span data-ttu-id="c40f2-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c40f2-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="c40f2-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c40f2-158">payloadFileName</span></span>|<span data-ttu-id="c40f2-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c40f2-159">String</span></span>|<span data-ttu-id="c40f2-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="c40f2-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="c40f2-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="c40f2-161">\*.xml).</span></span>|
|<span data-ttu-id="c40f2-162">payload</span><span class="sxs-lookup"><span data-stu-id="c40f2-162">payload</span></span>|<span data-ttu-id="c40f2-163">Binária</span><span class="sxs-lookup"><span data-stu-id="c40f2-163">Binary</span></span>|<span data-ttu-id="c40f2-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="c40f2-164">Payload.</span></span> <span data-ttu-id="c40f2-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="c40f2-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="c40f2-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40f2-166">Response</span></span>
<span data-ttu-id="c40f2-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c40f2-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c40f2-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c40f2-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="c40f2-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c40f2-169">Request</span></span>
<span data-ttu-id="c40f2-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c40f2-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c40f2-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40f2-171">Response</span></span>
<span data-ttu-id="c40f2-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c40f2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



