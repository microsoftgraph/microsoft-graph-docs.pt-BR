---
title: Criar detectedApp
description: Criar um novo objeto detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4542c9e675751cd20f2cd5739ae73b4110f97ef9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753766"
---
# <a name="create-detectedapp"></a><span data-ttu-id="bd914-103">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="bd914-103">Create detectedApp</span></span>

<span data-ttu-id="bd914-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd914-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd914-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd914-106">Criar um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd914-106">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd914-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd914-107">Prerequisites</span></span>
<span data-ttu-id="bd914-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd914-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd914-110">Permission type</span></span>|<span data-ttu-id="bd914-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd914-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd914-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd914-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd914-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bd914-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd914-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd914-115">Not supported.</span></span>|
|<span data-ttu-id="bd914-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd914-116">Application</span></span>|<span data-ttu-id="bd914-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd914-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd914-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="bd914-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd914-119">Request headers</span></span>
|<span data-ttu-id="bd914-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd914-120">Header</span></span>|<span data-ttu-id="bd914-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bd914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd914-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd914-122">Authorization</span></span>|<span data-ttu-id="bd914-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd914-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd914-124">Accept</span></span>|<span data-ttu-id="bd914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd914-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd914-126">Request body</span></span>
<span data-ttu-id="bd914-127">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="bd914-127">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="bd914-128">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="bd914-128">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="bd914-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd914-129">Property</span></span>|<span data-ttu-id="bd914-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd914-130">Type</span></span>|<span data-ttu-id="bd914-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd914-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd914-132">id</span><span class="sxs-lookup"><span data-stu-id="bd914-132">id</span></span>|<span data-ttu-id="bd914-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd914-133">String</span></span>|<span data-ttu-id="bd914-134">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="bd914-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="bd914-135">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="bd914-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="bd914-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd914-136">Read-only.</span></span>|
|<span data-ttu-id="bd914-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bd914-137">displayName</span></span>|<span data-ttu-id="bd914-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd914-138">String</span></span>|<span data-ttu-id="bd914-139">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="bd914-139">Name of the discovered application.</span></span> <span data-ttu-id="bd914-140">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bd914-140">Read-only</span></span>|
|<span data-ttu-id="bd914-141">version</span><span class="sxs-lookup"><span data-stu-id="bd914-141">version</span></span>|<span data-ttu-id="bd914-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd914-142">String</span></span>|<span data-ttu-id="bd914-143">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="bd914-143">Version of the discovered application.</span></span> <span data-ttu-id="bd914-144">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bd914-144">Read-only</span></span>|
|<span data-ttu-id="bd914-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="bd914-145">sizeInByte</span></span>|<span data-ttu-id="bd914-146">Int64</span><span class="sxs-lookup"><span data-stu-id="bd914-146">Int64</span></span>|<span data-ttu-id="bd914-147">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="bd914-147">Discovered application size in bytes.</span></span> <span data-ttu-id="bd914-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bd914-148">Read-only</span></span>|
|<span data-ttu-id="bd914-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bd914-149">deviceCount</span></span>|<span data-ttu-id="bd914-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bd914-150">Int32</span></span>|<span data-ttu-id="bd914-151">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd914-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="bd914-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd914-152">Response</span></span>
<span data-ttu-id="bd914-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd914-153">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd914-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd914-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd914-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd914-155">Request</span></span>
<span data-ttu-id="bd914-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd914-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="bd914-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd914-157">Response</span></span>
<span data-ttu-id="bd914-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd914-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




