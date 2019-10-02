---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentityUpload.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00866c4648377e66cc56887af2ac4398d31b733f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364078"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="184d3-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="184d3-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="184d3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="184d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="184d3-105">Criar um novo objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="184d3-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="184d3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="184d3-106">Prerequisites</span></span>
<span data-ttu-id="184d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="184d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="184d3-109">Permission type</span></span>|<span data-ttu-id="184d3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="184d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="184d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="184d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="184d3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184d3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="184d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="184d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="184d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184d3-114">Not supported.</span></span>|
|<span data-ttu-id="184d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="184d3-115">Application</span></span>|<span data-ttu-id="184d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="184d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="184d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="184d3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="184d3-118">Request headers</span></span>
|<span data-ttu-id="184d3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="184d3-119">Header</span></span>|<span data-ttu-id="184d3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="184d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="184d3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="184d3-121">Authorization</span></span>|<span data-ttu-id="184d3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="184d3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="184d3-123">Accept</span></span>|<span data-ttu-id="184d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="184d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="184d3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="184d3-125">Request body</span></span>
<span data-ttu-id="184d3-126">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="184d3-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="184d3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="184d3-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="184d3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="184d3-128">Property</span></span>|<span data-ttu-id="184d3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="184d3-129">Type</span></span>|<span data-ttu-id="184d3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="184d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184d3-131">id</span><span class="sxs-lookup"><span data-stu-id="184d3-131">id</span></span>|<span data-ttu-id="184d3-132">String</span><span class="sxs-lookup"><span data-stu-id="184d3-132">String</span></span>|<span data-ttu-id="184d3-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="184d3-133">The GUID for the object</span></span>|
|<span data-ttu-id="184d3-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="184d3-134">createdDateTimeUtc</span></span>|<span data-ttu-id="184d3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="184d3-135">DateTimeOffset</span></span>|<span data-ttu-id="184d3-136">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="184d3-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="184d3-137">status</span><span class="sxs-lookup"><span data-stu-id="184d3-137">status</span></span>|[<span data-ttu-id="184d3-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="184d3-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="184d3-139">Status de upload.</span><span class="sxs-lookup"><span data-stu-id="184d3-139">Upload status.</span></span> <span data-ttu-id="184d3-140">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="184d3-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="184d3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="184d3-141">Response</span></span>
<span data-ttu-id="184d3-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="184d3-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="184d3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="184d3-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="184d3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="184d3-144">Request</span></span>
<span data-ttu-id="184d3-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="184d3-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="184d3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="184d3-146">Response</span></span>
<span data-ttu-id="184d3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="184d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```




