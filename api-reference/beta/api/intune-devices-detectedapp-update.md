---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77bfb3880db9b7e36c8e6b9e8d2a8b53ab3450d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914994"
---
# <a name="update-detectedapp"></a><span data-ttu-id="9cc7f-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="9cc7f-103">Update detectedApp</span></span>

> <span data-ttu-id="9cc7f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cc7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cc7f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cc7f-107">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7f-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cc7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cc7f-108">Prerequisites</span></span>
<span data-ttu-id="9cc7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc7f-111">Permission type</span></span>|<span data-ttu-id="9cc7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cc7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc7f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc7f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9cc7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-116">Not supported.</span></span>|
|<span data-ttu-id="9cc7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc7f-117">Application</span></span>|<span data-ttu-id="9cc7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9cc7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7f-120">Request headers</span></span>
|<span data-ttu-id="9cc7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cc7f-121">Header</span></span>|<span data-ttu-id="9cc7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9cc7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc7f-123">Authorization</span></span>|<span data-ttu-id="9cc7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cc7f-125">Accept</span></span>|<span data-ttu-id="9cc7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7f-127">Request body</span></span>
<span data-ttu-id="9cc7f-128">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7f-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="9cc7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7f-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="9cc7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cc7f-130">Property</span></span>|<span data-ttu-id="9cc7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc7f-131">Type</span></span>|<span data-ttu-id="9cc7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cc7f-133">id</span><span class="sxs-lookup"><span data-stu-id="9cc7f-133">id</span></span>|<span data-ttu-id="9cc7f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cc7f-134">String</span></span>|<span data-ttu-id="9cc7f-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="9cc7f-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="9cc7f-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-137">Read-only.</span></span>|
|<span data-ttu-id="9cc7f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9cc7f-138">displayName</span></span>|<span data-ttu-id="9cc7f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cc7f-139">String</span></span>|<span data-ttu-id="9cc7f-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-140">Name of the discovered application.</span></span> <span data-ttu-id="9cc7f-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9cc7f-141">Read-only</span></span>|
|<span data-ttu-id="9cc7f-142">version</span><span class="sxs-lookup"><span data-stu-id="9cc7f-142">version</span></span>|<span data-ttu-id="9cc7f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cc7f-143">String</span></span>|<span data-ttu-id="9cc7f-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-144">Version of the discovered application.</span></span> <span data-ttu-id="9cc7f-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9cc7f-145">Read-only</span></span>|
|<span data-ttu-id="9cc7f-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="9cc7f-146">sizeInByte</span></span>|<span data-ttu-id="9cc7f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="9cc7f-147">Int64</span></span>|<span data-ttu-id="9cc7f-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-148">Discovered application size in bytes.</span></span> <span data-ttu-id="9cc7f-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9cc7f-149">Read-only</span></span>|
|<span data-ttu-id="9cc7f-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9cc7f-150">deviceCount</span></span>|<span data-ttu-id="9cc7f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc7f-151">Int32</span></span>|<span data-ttu-id="9cc7f-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc7f-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="9cc7f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7f-153">Response</span></span>
<span data-ttu-id="9cc7f-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc7f-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cc7f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cc7f-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7f-156">Request</span></span>
<span data-ttu-id="9cc7f-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9cc7f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7f-158">Response</span></span>
<span data-ttu-id="9cc7f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc7f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





