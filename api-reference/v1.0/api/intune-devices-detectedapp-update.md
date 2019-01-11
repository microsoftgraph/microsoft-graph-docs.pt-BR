---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86b8eb3bc1bac0902ce36bd763c633f06919d2fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821928"
---
# <a name="update-detectedapp"></a><span data-ttu-id="ac475-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="ac475-103">Update detectedApp</span></span>

> <span data-ttu-id="ac475-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ac475-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac475-105">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac475-105">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac475-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac475-106">Prerequisites</span></span>
<span data-ttu-id="ac475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac475-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac475-109">Permission type</span></span>|<span data-ttu-id="ac475-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac475-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac475-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac475-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac475-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac475-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ac475-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac475-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac475-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac475-114">Not supported.</span></span>|
|<span data-ttu-id="ac475-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac475-115">Application</span></span>|<span data-ttu-id="ac475-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac475-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac475-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac475-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ac475-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac475-118">Request headers</span></span>
|<span data-ttu-id="ac475-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac475-119">Header</span></span>|<span data-ttu-id="ac475-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ac475-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac475-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac475-121">Authorization</span></span>|<span data-ttu-id="ac475-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac475-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac475-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac475-123">Accept</span></span>|<span data-ttu-id="ac475-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ac475-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac475-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac475-125">Request body</span></span>
<span data-ttu-id="ac475-126">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac475-126">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="ac475-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac475-127">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="ac475-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac475-128">Property</span></span>|<span data-ttu-id="ac475-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac475-129">Type</span></span>|<span data-ttu-id="ac475-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac475-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac475-131">id</span><span class="sxs-lookup"><span data-stu-id="ac475-131">id</span></span>|<span data-ttu-id="ac475-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac475-132">String</span></span>|<span data-ttu-id="ac475-133">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="ac475-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="ac475-134">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="ac475-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="ac475-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac475-135">Read-only.</span></span>|
|<span data-ttu-id="ac475-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ac475-136">displayName</span></span>|<span data-ttu-id="ac475-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac475-137">String</span></span>|<span data-ttu-id="ac475-138">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="ac475-138">Name of the discovered application.</span></span> <span data-ttu-id="ac475-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ac475-139">Read-only</span></span>|
|<span data-ttu-id="ac475-140">version</span><span class="sxs-lookup"><span data-stu-id="ac475-140">version</span></span>|<span data-ttu-id="ac475-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac475-141">String</span></span>|<span data-ttu-id="ac475-142">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="ac475-142">Version of the discovered application.</span></span> <span data-ttu-id="ac475-143">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ac475-143">Read-only</span></span>|
|<span data-ttu-id="ac475-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="ac475-144">sizeInByte</span></span>|<span data-ttu-id="ac475-145">Int64</span><span class="sxs-lookup"><span data-stu-id="ac475-145">Int64</span></span>|<span data-ttu-id="ac475-146">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="ac475-146">Discovered application size in bytes.</span></span> <span data-ttu-id="ac475-147">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ac475-147">Read-only</span></span>|
|<span data-ttu-id="ac475-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ac475-148">deviceCount</span></span>|<span data-ttu-id="ac475-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ac475-149">Int32</span></span>|<span data-ttu-id="ac475-150">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac475-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="ac475-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac475-151">Response</span></span>
<span data-ttu-id="ac475-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac475-152">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac475-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac475-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac475-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac475-154">Request</span></span>
<span data-ttu-id="ac475-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac475-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
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

### <a name="response"></a><span data-ttu-id="ac475-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac475-156">Response</span></span>
<span data-ttu-id="ac475-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac475-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



