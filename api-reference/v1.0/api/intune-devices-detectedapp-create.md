---
title: Criar detectedApp
description: Criar um novo objeto detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7135b3ee02e0bf6b4c8d7a8cd4fe62a658b5f961
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542085"
---
# <a name="create-detectedapp"></a><span data-ttu-id="be73b-103">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="be73b-103">Create detectedApp</span></span>

> <span data-ttu-id="be73b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be73b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be73b-105">Criar um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="be73b-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be73b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be73b-106">Prerequisites</span></span>
<span data-ttu-id="be73b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be73b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be73b-109">Permission type</span></span>|<span data-ttu-id="be73b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be73b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be73b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be73b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be73b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be73b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be73b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be73b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be73b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be73b-114">Not supported.</span></span>|
|<span data-ttu-id="be73b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be73b-115">Application</span></span>|<span data-ttu-id="be73b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be73b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be73b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be73b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="be73b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be73b-118">Request headers</span></span>
|<span data-ttu-id="be73b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be73b-119">Header</span></span>|<span data-ttu-id="be73b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="be73b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be73b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be73b-121">Authorization</span></span>|<span data-ttu-id="be73b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be73b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be73b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be73b-123">Accept</span></span>|<span data-ttu-id="be73b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be73b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be73b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be73b-125">Request body</span></span>
<span data-ttu-id="be73b-126">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="be73b-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="be73b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="be73b-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="be73b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be73b-128">Property</span></span>|<span data-ttu-id="be73b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="be73b-129">Type</span></span>|<span data-ttu-id="be73b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="be73b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be73b-131">id</span><span class="sxs-lookup"><span data-stu-id="be73b-131">id</span></span>|<span data-ttu-id="be73b-132">String</span><span class="sxs-lookup"><span data-stu-id="be73b-132">String</span></span>|<span data-ttu-id="be73b-133">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="be73b-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="be73b-134">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="be73b-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="be73b-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be73b-135">Read-only.</span></span>|
|<span data-ttu-id="be73b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="be73b-136">displayName</span></span>|<span data-ttu-id="be73b-137">String</span><span class="sxs-lookup"><span data-stu-id="be73b-137">String</span></span>|<span data-ttu-id="be73b-138">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="be73b-138">Name of the discovered application.</span></span> <span data-ttu-id="be73b-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="be73b-139">Read-only</span></span>|
|<span data-ttu-id="be73b-140">version</span><span class="sxs-lookup"><span data-stu-id="be73b-140">version</span></span>|<span data-ttu-id="be73b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be73b-141">String</span></span>|<span data-ttu-id="be73b-142">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="be73b-142">Version of the discovered application.</span></span> <span data-ttu-id="be73b-143">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="be73b-143">Read-only</span></span>|
|<span data-ttu-id="be73b-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="be73b-144">sizeInByte</span></span>|<span data-ttu-id="be73b-145">Int64</span><span class="sxs-lookup"><span data-stu-id="be73b-145">Int64</span></span>|<span data-ttu-id="be73b-146">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="be73b-146">Discovered application size in bytes.</span></span> <span data-ttu-id="be73b-147">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="be73b-147">Read-only</span></span>|
|<span data-ttu-id="be73b-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="be73b-148">deviceCount</span></span>|<span data-ttu-id="be73b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="be73b-149">Int32</span></span>|<span data-ttu-id="be73b-150">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="be73b-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="be73b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="be73b-151">Response</span></span>
<span data-ttu-id="be73b-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be73b-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be73b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be73b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="be73b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be73b-154">Request</span></span>
<span data-ttu-id="be73b-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be73b-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be73b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="be73b-156">Response</span></span>
<span data-ttu-id="be73b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be73b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



