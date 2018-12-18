---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Crie um novo objeto de importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
ms.openlocfilehash: 16c3b83d81eb43362c3d2ffb091579efd6e5b598
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316762"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="e72cd-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="e72cd-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="e72cd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e72cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e72cd-105">Crie um novo objeto de [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="e72cd-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e72cd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e72cd-106">Prerequisites</span></span>
<span data-ttu-id="e72cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e72cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e72cd-109">Permission type</span></span>|<span data-ttu-id="e72cd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e72cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e72cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e72cd-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72cd-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e72cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e72cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e72cd-114">Not supported.</span></span>|
|<span data-ttu-id="e72cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e72cd-115">Application</span></span>|<span data-ttu-id="e72cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e72cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72cd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e72cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="e72cd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e72cd-118">Request headers</span></span>
|<span data-ttu-id="e72cd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e72cd-119">Header</span></span>|<span data-ttu-id="e72cd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e72cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72cd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e72cd-121">Authorization</span></span>|<span data-ttu-id="e72cd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e72cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72cd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e72cd-123">Accept</span></span>|<span data-ttu-id="e72cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e72cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72cd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e72cd-125">Request body</span></span>
<span data-ttu-id="e72cd-126">No corpo da solicitação, fornece uma representação JSON para o objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="e72cd-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="e72cd-127">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="e72cd-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="e72cd-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e72cd-128">Property</span></span>|<span data-ttu-id="e72cd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e72cd-129">Type</span></span>|<span data-ttu-id="e72cd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e72cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e72cd-131">id</span><span class="sxs-lookup"><span data-stu-id="e72cd-131">id</span></span>|<span data-ttu-id="e72cd-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e72cd-132">String</span></span>|<span data-ttu-id="e72cd-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e72cd-133">The GUID for the object</span></span>|
|<span data-ttu-id="e72cd-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="e72cd-134">createdDateTimeUtc</span></span>|<span data-ttu-id="e72cd-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72cd-135">DateTimeOffset</span></span>|<span data-ttu-id="e72cd-136">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="e72cd-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="e72cd-137">status</span><span class="sxs-lookup"><span data-stu-id="e72cd-137">status</span></span>|[<span data-ttu-id="e72cd-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e72cd-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="e72cd-139">Carrega o status.</span><span class="sxs-lookup"><span data-stu-id="e72cd-139">Upload status.</span></span> <span data-ttu-id="e72cd-140">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="e72cd-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="e72cd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e72cd-141">Response</span></span>
<span data-ttu-id="e72cd-142">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e72cd-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72cd-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e72cd-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="e72cd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e72cd-144">Request</span></span>
<span data-ttu-id="e72cd-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e72cd-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e72cd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e72cd-146">Response</span></span>
<span data-ttu-id="e72cd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e72cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



