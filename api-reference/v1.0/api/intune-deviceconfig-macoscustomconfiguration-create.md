---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
ms.openlocfilehash: 41938c7f1f898d1180a979edc6b1790249ed94f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006132"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="5236e-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5236e-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="5236e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5236e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5236e-105">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5236e-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5236e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5236e-106">Prerequisites</span></span>
<span data-ttu-id="5236e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5236e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5236e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5236e-109">Permission type</span></span>|<span data-ttu-id="5236e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5236e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5236e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5236e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5236e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5236e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5236e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5236e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5236e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5236e-114">Not supported.</span></span>|
|<span data-ttu-id="5236e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5236e-115">Application</span></span>|<span data-ttu-id="5236e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5236e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5236e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5236e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5236e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5236e-118">Request headers</span></span>
|<span data-ttu-id="5236e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5236e-119">Header</span></span>|<span data-ttu-id="5236e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5236e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5236e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5236e-121">Authorization</span></span>|<span data-ttu-id="5236e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5236e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5236e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5236e-123">Accept</span></span>|<span data-ttu-id="5236e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5236e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5236e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5236e-125">Request body</span></span>
<span data-ttu-id="5236e-126">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5236e-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="5236e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5236e-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="5236e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5236e-128">Property</span></span>|<span data-ttu-id="5236e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5236e-129">Type</span></span>|<span data-ttu-id="5236e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5236e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5236e-131">id</span><span class="sxs-lookup"><span data-stu-id="5236e-131">id</span></span>|<span data-ttu-id="5236e-132">String</span><span class="sxs-lookup"><span data-stu-id="5236e-132">String</span></span>|<span data-ttu-id="5236e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5236e-133">Key of the entity.</span></span> <span data-ttu-id="5236e-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5236e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5236e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5236e-136">DateTimeOffset</span></span>|<span data-ttu-id="5236e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5236e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="5236e-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5236e-139">createdDateTime</span></span>|<span data-ttu-id="5236e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5236e-140">DateTimeOffset</span></span>|<span data-ttu-id="5236e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5236e-141">DateTime the object was created.</span></span> <span data-ttu-id="5236e-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-143">description</span><span class="sxs-lookup"><span data-stu-id="5236e-143">description</span></span>|<span data-ttu-id="5236e-144">String</span><span class="sxs-lookup"><span data-stu-id="5236e-144">String</span></span>|<span data-ttu-id="5236e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5236e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5236e-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5236e-147">displayName</span></span>|<span data-ttu-id="5236e-148">String</span><span class="sxs-lookup"><span data-stu-id="5236e-148">String</span></span>|<span data-ttu-id="5236e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5236e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5236e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-151">version</span><span class="sxs-lookup"><span data-stu-id="5236e-151">version</span></span>|<span data-ttu-id="5236e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5236e-152">Int32</span></span>|<span data-ttu-id="5236e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5236e-153">Version of the device configuration.</span></span> <span data-ttu-id="5236e-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5236e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5236e-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="5236e-155">payloadName</span></span>|<span data-ttu-id="5236e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5236e-156">String</span></span>|<span data-ttu-id="5236e-157">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5236e-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="5236e-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="5236e-158">payloadFileName</span></span>|<span data-ttu-id="5236e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5236e-159">String</span></span>|<span data-ttu-id="5236e-160">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="5236e-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="5236e-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="5236e-161">\*.xml).</span></span>|
|<span data-ttu-id="5236e-162">payload</span><span class="sxs-lookup"><span data-stu-id="5236e-162">payload</span></span>|<span data-ttu-id="5236e-163">Binária</span><span class="sxs-lookup"><span data-stu-id="5236e-163">Binary</span></span>|<span data-ttu-id="5236e-164">Carga.</span><span class="sxs-lookup"><span data-stu-id="5236e-164">Payload.</span></span> <span data-ttu-id="5236e-165">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="5236e-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="5236e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5236e-166">Response</span></span>
<span data-ttu-id="5236e-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5236e-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5236e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5236e-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5236e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5236e-169">Request</span></span>
<span data-ttu-id="5236e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5236e-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5236e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5236e-171">Response</span></span>
<span data-ttu-id="5236e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5236e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



