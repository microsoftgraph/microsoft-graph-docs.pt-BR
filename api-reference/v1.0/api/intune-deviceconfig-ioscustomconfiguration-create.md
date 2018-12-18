---
title: Criar iosCustomConfiguration
description: Cria um novo objeto iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 2b445ae1e8025eb90426c51580890c765842b622
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328802"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="c62cf-103">Criar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c62cf-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="c62cf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c62cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c62cf-105">Cria um novo objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c62cf-105">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c62cf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c62cf-106">Prerequisites</span></span>
<span data-ttu-id="c62cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c62cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c62cf-109">Permission type</span></span>|<span data-ttu-id="c62cf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c62cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c62cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c62cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c62cf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c62cf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c62cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c62cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c62cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c62cf-114">Not supported.</span></span>|
|<span data-ttu-id="c62cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c62cf-115">Application</span></span>|<span data-ttu-id="c62cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c62cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c62cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c62cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c62cf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c62cf-118">Request headers</span></span>
|<span data-ttu-id="c62cf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c62cf-119">Header</span></span>|<span data-ttu-id="c62cf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c62cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c62cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c62cf-121">Authorization</span></span>|<span data-ttu-id="c62cf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c62cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c62cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c62cf-123">Accept</span></span>|<span data-ttu-id="c62cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c62cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62cf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c62cf-125">Request body</span></span>
<span data-ttu-id="c62cf-126">No corpo da solicitação, forneça uma representação JSON do objeto iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c62cf-126">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="c62cf-127">A tabela a seguir mostra as propriedades que são necessárias ao criar iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c62cf-127">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="c62cf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c62cf-128">Property</span></span>|<span data-ttu-id="c62cf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c62cf-129">Type</span></span>|<span data-ttu-id="c62cf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c62cf-131">id</span><span class="sxs-lookup"><span data-stu-id="c62cf-131">id</span></span>|<span data-ttu-id="c62cf-132">String</span><span class="sxs-lookup"><span data-stu-id="c62cf-132">String</span></span>|<span data-ttu-id="c62cf-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c62cf-133">Key of the entity.</span></span> <span data-ttu-id="c62cf-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c62cf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c62cf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c62cf-136">DateTimeOffset</span></span>|<span data-ttu-id="c62cf-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c62cf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c62cf-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c62cf-139">createdDateTime</span></span>|<span data-ttu-id="c62cf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c62cf-140">DateTimeOffset</span></span>|<span data-ttu-id="c62cf-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c62cf-141">DateTime the object was created.</span></span> <span data-ttu-id="c62cf-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-143">description</span><span class="sxs-lookup"><span data-stu-id="c62cf-143">description</span></span>|<span data-ttu-id="c62cf-144">String</span><span class="sxs-lookup"><span data-stu-id="c62cf-144">String</span></span>|<span data-ttu-id="c62cf-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c62cf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c62cf-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c62cf-147">displayName</span></span>|<span data-ttu-id="c62cf-148">String</span><span class="sxs-lookup"><span data-stu-id="c62cf-148">String</span></span>|<span data-ttu-id="c62cf-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c62cf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c62cf-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-151">version</span><span class="sxs-lookup"><span data-stu-id="c62cf-151">version</span></span>|<span data-ttu-id="c62cf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c62cf-152">Int32</span></span>|<span data-ttu-id="c62cf-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c62cf-153">Version of the device configuration.</span></span> <span data-ttu-id="c62cf-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c62cf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c62cf-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="c62cf-155">payloadName</span></span>|<span data-ttu-id="c62cf-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c62cf-156">String</span></span>|<span data-ttu-id="c62cf-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c62cf-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="c62cf-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c62cf-158">payloadFileName</span></span>|<span data-ttu-id="c62cf-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c62cf-159">String</span></span>|<span data-ttu-id="c62cf-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="c62cf-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="c62cf-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="c62cf-161">\*.xml).</span></span>|
|<span data-ttu-id="c62cf-162">payload</span><span class="sxs-lookup"><span data-stu-id="c62cf-162">payload</span></span>|<span data-ttu-id="c62cf-163">Binária</span><span class="sxs-lookup"><span data-stu-id="c62cf-163">Binary</span></span>|<span data-ttu-id="c62cf-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="c62cf-164">Payload.</span></span> <span data-ttu-id="c62cf-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="c62cf-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="c62cf-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="c62cf-166">Response</span></span>
<span data-ttu-id="c62cf-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c62cf-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62cf-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c62cf-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="c62cf-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c62cf-169">Request</span></span>
<span data-ttu-id="c62cf-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c62cf-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c62cf-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c62cf-171">Response</span></span>
<span data-ttu-id="c62cf-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c62cf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



