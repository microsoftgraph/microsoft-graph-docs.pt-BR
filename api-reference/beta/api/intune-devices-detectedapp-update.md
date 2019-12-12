---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7774a4501343b4740faf64d2a9605256cc19f3f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945169"
---
# <a name="update-detectedapp"></a><span data-ttu-id="626da-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="626da-103">Update detectedApp</span></span>

> <span data-ttu-id="626da-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="626da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="626da-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="626da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626da-106">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="626da-106">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="626da-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="626da-107">Prerequisites</span></span>
<span data-ttu-id="626da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="626da-110">Permission type</span></span>|<span data-ttu-id="626da-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="626da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="626da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="626da-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626da-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="626da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="626da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="626da-115">Not supported.</span></span>|
|<span data-ttu-id="626da-116">Application</span><span class="sxs-lookup"><span data-stu-id="626da-116">Application</span></span>|<span data-ttu-id="626da-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626da-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="626da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="626da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="626da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="626da-119">Request headers</span></span>
|<span data-ttu-id="626da-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="626da-120">Header</span></span>|<span data-ttu-id="626da-121">Valor</span><span class="sxs-lookup"><span data-stu-id="626da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="626da-122">Authorization</span></span>|<span data-ttu-id="626da-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="626da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626da-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="626da-124">Accept</span></span>|<span data-ttu-id="626da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="626da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="626da-126">Request body</span></span>
<span data-ttu-id="626da-127">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="626da-127">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="626da-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="626da-128">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="626da-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="626da-129">Property</span></span>|<span data-ttu-id="626da-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="626da-130">Type</span></span>|<span data-ttu-id="626da-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="626da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626da-132">id</span><span class="sxs-lookup"><span data-stu-id="626da-132">id</span></span>|<span data-ttu-id="626da-133">String</span><span class="sxs-lookup"><span data-stu-id="626da-133">String</span></span>|<span data-ttu-id="626da-134">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="626da-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="626da-135">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="626da-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="626da-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="626da-136">Read-only.</span></span>|
|<span data-ttu-id="626da-137">displayName</span><span class="sxs-lookup"><span data-stu-id="626da-137">displayName</span></span>|<span data-ttu-id="626da-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626da-138">String</span></span>|<span data-ttu-id="626da-139">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="626da-139">Name of the discovered application.</span></span> <span data-ttu-id="626da-140">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="626da-140">Read-only</span></span>|
|<span data-ttu-id="626da-141">version</span><span class="sxs-lookup"><span data-stu-id="626da-141">version</span></span>|<span data-ttu-id="626da-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626da-142">String</span></span>|<span data-ttu-id="626da-143">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="626da-143">Version of the discovered application.</span></span> <span data-ttu-id="626da-144">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="626da-144">Read-only</span></span>|
|<span data-ttu-id="626da-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="626da-145">sizeInByte</span></span>|<span data-ttu-id="626da-146">Int64</span><span class="sxs-lookup"><span data-stu-id="626da-146">Int64</span></span>|<span data-ttu-id="626da-147">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="626da-147">Discovered application size in bytes.</span></span> <span data-ttu-id="626da-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="626da-148">Read-only</span></span>|
|<span data-ttu-id="626da-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="626da-149">deviceCount</span></span>|<span data-ttu-id="626da-150">Int32</span><span class="sxs-lookup"><span data-stu-id="626da-150">Int32</span></span>|<span data-ttu-id="626da-151">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="626da-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="626da-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="626da-152">Response</span></span>
<span data-ttu-id="626da-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="626da-153">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626da-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="626da-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="626da-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="626da-155">Request</span></span>
<span data-ttu-id="626da-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="626da-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="626da-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="626da-157">Response</span></span>
<span data-ttu-id="626da-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="626da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





