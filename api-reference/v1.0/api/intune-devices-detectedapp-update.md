---
title: Atualizar detectedApp
description: Atualizar as propriedades de um objeto detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d03608902330139f3b18fe2457048099c28ecc97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009580"
---
# <a name="update-detectedapp"></a><span data-ttu-id="93f77-103">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="93f77-103">Update detectedApp</span></span>

<span data-ttu-id="93f77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93f77-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93f77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f77-106">Atualizar as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="93f77-106">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93f77-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93f77-107">Prerequisites</span></span>
<span data-ttu-id="93f77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93f77-110">Permission type</span></span>|<span data-ttu-id="93f77-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93f77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93f77-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93f77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93f77-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f77-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="93f77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93f77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93f77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f77-115">Not supported.</span></span>|
|<span data-ttu-id="93f77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f77-116">Application</span></span>|<span data-ttu-id="93f77-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93f77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93f77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="93f77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93f77-119">Request headers</span></span>
|<span data-ttu-id="93f77-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93f77-120">Header</span></span>|<span data-ttu-id="93f77-121">Valor</span><span class="sxs-lookup"><span data-stu-id="93f77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93f77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93f77-122">Authorization</span></span>|<span data-ttu-id="93f77-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93f77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93f77-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93f77-124">Accept</span></span>|<span data-ttu-id="93f77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93f77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93f77-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93f77-126">Request body</span></span>
<span data-ttu-id="93f77-127">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="93f77-127">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="93f77-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="93f77-128">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="93f77-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93f77-129">Property</span></span>|<span data-ttu-id="93f77-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="93f77-130">Type</span></span>|<span data-ttu-id="93f77-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f77-132">id</span><span class="sxs-lookup"><span data-stu-id="93f77-132">id</span></span>|<span data-ttu-id="93f77-133">String</span><span class="sxs-lookup"><span data-stu-id="93f77-133">String</span></span>|<span data-ttu-id="93f77-134">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="93f77-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="93f77-135">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="93f77-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="93f77-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93f77-136">Read-only.</span></span>|
|<span data-ttu-id="93f77-137">displayName</span><span class="sxs-lookup"><span data-stu-id="93f77-137">displayName</span></span>|<span data-ttu-id="93f77-138">String</span><span class="sxs-lookup"><span data-stu-id="93f77-138">String</span></span>|<span data-ttu-id="93f77-139">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="93f77-139">Name of the discovered application.</span></span> <span data-ttu-id="93f77-140">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="93f77-140">Read-only</span></span>|
|<span data-ttu-id="93f77-141">version</span><span class="sxs-lookup"><span data-stu-id="93f77-141">version</span></span>|<span data-ttu-id="93f77-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93f77-142">String</span></span>|<span data-ttu-id="93f77-143">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="93f77-143">Version of the discovered application.</span></span> <span data-ttu-id="93f77-144">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="93f77-144">Read-only</span></span>|
|<span data-ttu-id="93f77-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="93f77-145">sizeInByte</span></span>|<span data-ttu-id="93f77-146">Int64</span><span class="sxs-lookup"><span data-stu-id="93f77-146">Int64</span></span>|<span data-ttu-id="93f77-147">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="93f77-147">Discovered application size in bytes.</span></span> <span data-ttu-id="93f77-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="93f77-148">Read-only</span></span>|
|<span data-ttu-id="93f77-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="93f77-149">deviceCount</span></span>|<span data-ttu-id="93f77-150">Int32</span><span class="sxs-lookup"><span data-stu-id="93f77-150">Int32</span></span>|<span data-ttu-id="93f77-151">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f77-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="93f77-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f77-152">Response</span></span>
<span data-ttu-id="93f77-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93f77-153">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93f77-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93f77-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="93f77-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f77-155">Request</span></span>
<span data-ttu-id="93f77-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f77-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93f77-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f77-157">Response</span></span>
<span data-ttu-id="93f77-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93f77-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









