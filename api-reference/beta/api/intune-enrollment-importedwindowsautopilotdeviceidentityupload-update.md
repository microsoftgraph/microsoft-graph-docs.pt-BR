---
title: Atualizar importedWindowsAutopilotDeviceIdentityUpload
description: Atualiza as propriedades de um objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa2c38224d57dc7750b95b2a339ba0bb10b29f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145581"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="fabbb-103">Atualizar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="fabbb-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="fabbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fabbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fabbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fabbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabbb-106">Atualiza as propriedades de um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="fabbb-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fabbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fabbb-107">Prerequisites</span></span>
<span data-ttu-id="fabbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fabbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fabbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fabbb-110">Permission type</span></span>|<span data-ttu-id="fabbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fabbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fabbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fabbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fabbb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabbb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fabbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fabbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fabbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fabbb-115">Not supported.</span></span>|
|<span data-ttu-id="fabbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fabbb-116">Application</span></span>|<span data-ttu-id="fabbb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fabbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fabbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fabbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="fabbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fabbb-119">Request headers</span></span>
|<span data-ttu-id="fabbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fabbb-120">Header</span></span>|<span data-ttu-id="fabbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fabbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fabbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fabbb-122">Authorization</span></span>|<span data-ttu-id="fabbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fabbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fabbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fabbb-124">Accept</span></span>|<span data-ttu-id="fabbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fabbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fabbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fabbb-126">Request body</span></span>
<span data-ttu-id="fabbb-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="fabbb-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="fabbb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="fabbb-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="fabbb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fabbb-129">Property</span></span>|<span data-ttu-id="fabbb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fabbb-130">Type</span></span>|<span data-ttu-id="fabbb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fabbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabbb-132">id</span><span class="sxs-lookup"><span data-stu-id="fabbb-132">id</span></span>|<span data-ttu-id="fabbb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fabbb-133">String</span></span>|<span data-ttu-id="fabbb-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="fabbb-134">The GUID for the object</span></span>|
|<span data-ttu-id="fabbb-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="fabbb-135">createdDateTimeUtc</span></span>|<span data-ttu-id="fabbb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fabbb-136">DateTimeOffset</span></span>|<span data-ttu-id="fabbb-137">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="fabbb-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="fabbb-138">status</span><span class="sxs-lookup"><span data-stu-id="fabbb-138">status</span></span>|[<span data-ttu-id="fabbb-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="fabbb-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="fabbb-140">Status de upload.</span><span class="sxs-lookup"><span data-stu-id="fabbb-140">Upload status.</span></span> <span data-ttu-id="fabbb-141">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="fabbb-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="fabbb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabbb-142">Response</span></span>
<span data-ttu-id="fabbb-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fabbb-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fabbb-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fabbb-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="fabbb-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fabbb-145">Request</span></span>
<span data-ttu-id="fabbb-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fabbb-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="fabbb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabbb-147">Response</span></span>
<span data-ttu-id="fabbb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fabbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




