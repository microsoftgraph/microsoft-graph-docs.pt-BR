---
title: Atualizar importedWindowsAutopilotDeviceIdentityUpload
description: Atualiza as propriedades de um objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 558cc0552694ad40f3088fbac8a3b3c60b73fd9a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250716"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="8ac5e-103">Atualizar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="8ac5e-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="8ac5e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac5e-105">Atualiza as propriedades de um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="8ac5e-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ac5e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ac5e-106">Prerequisites</span></span>
<span data-ttu-id="8ac5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ac5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8ac5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ac5e-109">Permission type</span></span>|<span data-ttu-id="8ac5e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ac5e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ac5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ac5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ac5e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ac5e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8ac5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ac5e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ac5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-114">Not supported.</span></span>|
|<span data-ttu-id="8ac5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ac5e-115">Application</span></span>|<span data-ttu-id="8ac5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ac5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ac5e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="8ac5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5e-118">Request headers</span></span>
|<span data-ttu-id="8ac5e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ac5e-119">Header</span></span>|<span data-ttu-id="8ac5e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8ac5e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ac5e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ac5e-121">Authorization</span></span>|<span data-ttu-id="8ac5e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ac5e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ac5e-123">Accept</span></span>|<span data-ttu-id="8ac5e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8ac5e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ac5e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5e-125">Request body</span></span>
<span data-ttu-id="8ac5e-126">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="8ac5e-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="8ac5e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="8ac5e-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="8ac5e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ac5e-128">Property</span></span>|<span data-ttu-id="8ac5e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ac5e-129">Type</span></span>|<span data-ttu-id="8ac5e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ac5e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac5e-131">id</span><span class="sxs-lookup"><span data-stu-id="8ac5e-131">id</span></span>|<span data-ttu-id="8ac5e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ac5e-132">String</span></span>|<span data-ttu-id="8ac5e-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-133">The GUID for the object</span></span>|
|<span data-ttu-id="8ac5e-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="8ac5e-134">createdDateTimeUtc</span></span>|<span data-ttu-id="8ac5e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac5e-135">DateTimeOffset</span></span>|<span data-ttu-id="8ac5e-136">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="8ac5e-137">status</span><span class="sxs-lookup"><span data-stu-id="8ac5e-137">status</span></span>|[<span data-ttu-id="8ac5e-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="8ac5e-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="8ac5e-139">Status de upload.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-139">Upload status.</span></span> <span data-ttu-id="8ac5e-140">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="8ac5e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac5e-141">Response</span></span>
<span data-ttu-id="8ac5e-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ac5e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ac5e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ac5e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5e-144">Request</span></span>
<span data-ttu-id="8ac5e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="8ac5e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac5e-146">Response</span></span>
<span data-ttu-id="8ac5e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ac5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```



