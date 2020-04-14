---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bba20ae613457012a3577991afb10480ec428cfe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380992"
---
# <a name="update-detectedapp"></a><span data-ttu-id="1a1d5-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="1a1d5-103">Update detectedApp</span></span>

<span data-ttu-id="1a1d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a1d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a1d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a1d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1d5-107">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1d5-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a1d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a1d5-108">Prerequisites</span></span>
<span data-ttu-id="1a1d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a1d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a1d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a1d5-111">Permission type</span></span>|<span data-ttu-id="1a1d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a1d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a1d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a1d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a1d5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1d5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a1d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a1d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a1d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-116">Not supported.</span></span>|
|<span data-ttu-id="1a1d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a1d5-117">Application</span></span>|<span data-ttu-id="1a1d5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1d5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a1d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a1d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1a1d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d5-120">Request headers</span></span>
|<span data-ttu-id="1a1d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a1d5-121">Header</span></span>|<span data-ttu-id="1a1d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1a1d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a1d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a1d5-123">Authorization</span></span>|<span data-ttu-id="1a1d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a1d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a1d5-125">Accept</span></span>|<span data-ttu-id="1a1d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a1d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a1d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d5-127">Request body</span></span>
<span data-ttu-id="1a1d5-128">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1d5-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="1a1d5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1d5-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="1a1d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a1d5-130">Property</span></span>|<span data-ttu-id="1a1d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1d5-131">Type</span></span>|<span data-ttu-id="1a1d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1d5-133">id</span><span class="sxs-lookup"><span data-stu-id="1a1d5-133">id</span></span>|<span data-ttu-id="1a1d5-134">String</span><span class="sxs-lookup"><span data-stu-id="1a1d5-134">String</span></span>|<span data-ttu-id="1a1d5-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="1a1d5-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="1a1d5-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-137">Read-only.</span></span>|
|<span data-ttu-id="1a1d5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1a1d5-138">displayName</span></span>|<span data-ttu-id="1a1d5-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1d5-139">String</span></span>|<span data-ttu-id="1a1d5-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-140">Name of the discovered application.</span></span> <span data-ttu-id="1a1d5-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1a1d5-141">Read-only</span></span>|
|<span data-ttu-id="1a1d5-142">version</span><span class="sxs-lookup"><span data-stu-id="1a1d5-142">version</span></span>|<span data-ttu-id="1a1d5-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1d5-143">String</span></span>|<span data-ttu-id="1a1d5-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-144">Version of the discovered application.</span></span> <span data-ttu-id="1a1d5-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1a1d5-145">Read-only</span></span>|
|<span data-ttu-id="1a1d5-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="1a1d5-146">sizeInByte</span></span>|<span data-ttu-id="1a1d5-147">Int64</span><span class="sxs-lookup"><span data-stu-id="1a1d5-147">Int64</span></span>|<span data-ttu-id="1a1d5-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-148">Discovered application size in bytes.</span></span> <span data-ttu-id="1a1d5-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1a1d5-149">Read-only</span></span>|
|<span data-ttu-id="1a1d5-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1a1d5-150">deviceCount</span></span>|<span data-ttu-id="1a1d5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1a1d5-151">Int32</span></span>|<span data-ttu-id="1a1d5-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a1d5-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="1a1d5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1d5-153">Response</span></span>
<span data-ttu-id="1a1d5-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1d5-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a1d5-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a1d5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1d5-156">Request</span></span>
<span data-ttu-id="1a1d5-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a1d5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1d5-158">Response</span></span>
<span data-ttu-id="1a1d5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a1d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



