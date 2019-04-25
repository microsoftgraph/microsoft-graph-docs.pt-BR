---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa8e18a8635be0a8955b3e2c7400a5884cf8d3c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532454"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="ae21a-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="ae21a-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="ae21a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae21a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae21a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae21a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae21a-106">Criar um novo objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="ae21a-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae21a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae21a-107">Prerequisites</span></span>
<span data-ttu-id="ae21a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae21a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae21a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae21a-110">Permission type</span></span>|<span data-ttu-id="ae21a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae21a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae21a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae21a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae21a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae21a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae21a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae21a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae21a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae21a-115">Not supported.</span></span>|
|<span data-ttu-id="ae21a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae21a-116">Application</span></span>|<span data-ttu-id="ae21a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae21a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae21a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae21a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="ae21a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae21a-119">Request headers</span></span>
|<span data-ttu-id="ae21a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae21a-120">Header</span></span>|<span data-ttu-id="ae21a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ae21a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae21a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae21a-122">Authorization</span></span>|<span data-ttu-id="ae21a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae21a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae21a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae21a-124">Accept</span></span>|<span data-ttu-id="ae21a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae21a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae21a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae21a-126">Request body</span></span>
<span data-ttu-id="ae21a-127">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="ae21a-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="ae21a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="ae21a-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="ae21a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae21a-129">Property</span></span>|<span data-ttu-id="ae21a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae21a-130">Type</span></span>|<span data-ttu-id="ae21a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae21a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae21a-132">id</span><span class="sxs-lookup"><span data-stu-id="ae21a-132">id</span></span>|<span data-ttu-id="ae21a-133">String</span><span class="sxs-lookup"><span data-stu-id="ae21a-133">String</span></span>|<span data-ttu-id="ae21a-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ae21a-134">The GUID for the object</span></span>|
|<span data-ttu-id="ae21a-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="ae21a-135">createdDateTimeUtc</span></span>|<span data-ttu-id="ae21a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae21a-136">DateTimeOffset</span></span>|<span data-ttu-id="ae21a-137">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="ae21a-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="ae21a-138">status</span><span class="sxs-lookup"><span data-stu-id="ae21a-138">status</span></span>|[<span data-ttu-id="ae21a-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="ae21a-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="ae21a-140">Status de upload.</span><span class="sxs-lookup"><span data-stu-id="ae21a-140">Upload status.</span></span> <span data-ttu-id="ae21a-141">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="ae21a-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="ae21a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae21a-142">Response</span></span>
<span data-ttu-id="ae21a-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae21a-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae21a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae21a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae21a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae21a-145">Request</span></span>
<span data-ttu-id="ae21a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae21a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="ae21a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae21a-147">Response</span></span>
<span data-ttu-id="ae21a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae21a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





