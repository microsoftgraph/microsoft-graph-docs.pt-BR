---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
ms.openlocfilehash: 58fa37603b583a4ccf0579d2c6021ed5c1e60cc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035110"
---
# <a name="update-detectedapp"></a><span data-ttu-id="0ffa0-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="0ffa0-103">Update detectedApp</span></span>

> <span data-ttu-id="0ffa0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ffa0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ffa0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ffa0-107">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ffa0-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ffa0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ffa0-108">Prerequisites</span></span>
<span data-ttu-id="0ffa0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ffa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ffa0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ffa0-111">Permission type</span></span>|<span data-ttu-id="0ffa0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ffa0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ffa0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ffa0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ffa0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ffa0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ffa0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ffa0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ffa0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-116">Not supported.</span></span>|
|<span data-ttu-id="0ffa0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ffa0-117">Application</span></span>|<span data-ttu-id="0ffa0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ffa0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ffa0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0ffa0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ffa0-120">Request headers</span></span>
|<span data-ttu-id="0ffa0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ffa0-121">Header</span></span>|<span data-ttu-id="0ffa0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ffa0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ffa0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ffa0-123">Authorization</span></span>|<span data-ttu-id="0ffa0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ffa0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ffa0-125">Accept</span></span>|<span data-ttu-id="0ffa0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ffa0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ffa0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ffa0-127">Request body</span></span>
<span data-ttu-id="0ffa0-128">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ffa0-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="0ffa0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ffa0-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="0ffa0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ffa0-130">Property</span></span>|<span data-ttu-id="0ffa0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ffa0-131">Type</span></span>|<span data-ttu-id="0ffa0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ffa0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ffa0-133">id</span><span class="sxs-lookup"><span data-stu-id="0ffa0-133">id</span></span>|<span data-ttu-id="0ffa0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ffa0-134">String</span></span>|<span data-ttu-id="0ffa0-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="0ffa0-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="0ffa0-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-137">Read-only.</span></span>|
|<span data-ttu-id="0ffa0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0ffa0-138">displayName</span></span>|<span data-ttu-id="0ffa0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ffa0-139">String</span></span>|<span data-ttu-id="0ffa0-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-140">Name of the discovered application.</span></span> <span data-ttu-id="0ffa0-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0ffa0-141">Read-only</span></span>|
|<span data-ttu-id="0ffa0-142">version</span><span class="sxs-lookup"><span data-stu-id="0ffa0-142">version</span></span>|<span data-ttu-id="0ffa0-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ffa0-143">String</span></span>|<span data-ttu-id="0ffa0-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-144">Version of the discovered application.</span></span> <span data-ttu-id="0ffa0-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0ffa0-145">Read-only</span></span>|
|<span data-ttu-id="0ffa0-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="0ffa0-146">sizeInByte</span></span>|<span data-ttu-id="0ffa0-147">Int64</span><span class="sxs-lookup"><span data-stu-id="0ffa0-147">Int64</span></span>|<span data-ttu-id="0ffa0-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-148">Discovered application size in bytes.</span></span> <span data-ttu-id="0ffa0-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0ffa0-149">Read-only</span></span>|
|<span data-ttu-id="0ffa0-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="0ffa0-150">deviceCount</span></span>|<span data-ttu-id="0ffa0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0ffa0-151">Int32</span></span>|<span data-ttu-id="0ffa0-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ffa0-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="0ffa0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ffa0-153">Response</span></span>
<span data-ttu-id="0ffa0-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ffa0-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ffa0-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ffa0-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ffa0-156">Request</span></span>
<span data-ttu-id="0ffa0-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 117

{
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="0ffa0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ffa0-158">Response</span></span>
<span data-ttu-id="0ffa0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ffa0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```





