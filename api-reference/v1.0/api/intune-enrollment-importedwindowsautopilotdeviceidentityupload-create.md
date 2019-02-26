---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fd4230b0ecdb4279380255b1fa62cbe697a4843
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264390"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="39382-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="39382-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="39382-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39382-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39382-105">Criar um novo objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="39382-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39382-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39382-106">Prerequisites</span></span>
<span data-ttu-id="39382-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39382-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39382-109">Permission type</span></span>|<span data-ttu-id="39382-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39382-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39382-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39382-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39382-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39382-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="39382-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39382-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39382-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39382-114">Not supported.</span></span>|
|<span data-ttu-id="39382-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39382-115">Application</span></span>|<span data-ttu-id="39382-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39382-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39382-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39382-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="39382-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39382-118">Request headers</span></span>
|<span data-ttu-id="39382-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39382-119">Header</span></span>|<span data-ttu-id="39382-120">Valor</span><span class="sxs-lookup"><span data-stu-id="39382-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39382-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39382-121">Authorization</span></span>|<span data-ttu-id="39382-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39382-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39382-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39382-123">Accept</span></span>|<span data-ttu-id="39382-124">application/json</span><span class="sxs-lookup"><span data-stu-id="39382-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39382-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39382-125">Request body</span></span>
<span data-ttu-id="39382-126">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="39382-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="39382-127">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="39382-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="39382-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39382-128">Property</span></span>|<span data-ttu-id="39382-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="39382-129">Type</span></span>|<span data-ttu-id="39382-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="39382-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39382-131">id</span><span class="sxs-lookup"><span data-stu-id="39382-131">id</span></span>|<span data-ttu-id="39382-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39382-132">String</span></span>|<span data-ttu-id="39382-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="39382-133">The GUID for the object</span></span>|
|<span data-ttu-id="39382-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="39382-134">createdDateTimeUtc</span></span>|<span data-ttu-id="39382-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39382-135">DateTimeOffset</span></span>|<span data-ttu-id="39382-136">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="39382-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="39382-137">status</span><span class="sxs-lookup"><span data-stu-id="39382-137">status</span></span>|[<span data-ttu-id="39382-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="39382-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="39382-139">Status de upload.</span><span class="sxs-lookup"><span data-stu-id="39382-139">Upload status.</span></span> <span data-ttu-id="39382-140">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="39382-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="39382-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="39382-141">Response</span></span>
<span data-ttu-id="39382-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39382-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39382-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39382-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="39382-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39382-144">Request</span></span>
<span data-ttu-id="39382-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39382-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39382-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="39382-146">Response</span></span>
<span data-ttu-id="39382-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39382-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



