---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Crie um novo objeto de importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7c175b87258067fe4781316fe4287da9bdd1a66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861380"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="775c3-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="775c3-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="775c3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="775c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="775c3-105">Crie um novo objeto de [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="775c3-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="775c3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="775c3-106">Prerequisites</span></span>
<span data-ttu-id="775c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="775c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="775c3-109">Permission type</span></span>|<span data-ttu-id="775c3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="775c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="775c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="775c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="775c3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775c3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="775c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="775c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="775c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775c3-114">Not supported.</span></span>|
|<span data-ttu-id="775c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="775c3-115">Application</span></span>|<span data-ttu-id="775c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="775c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="775c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="775c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="775c3-118">Request headers</span></span>
|<span data-ttu-id="775c3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="775c3-119">Header</span></span>|<span data-ttu-id="775c3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="775c3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="775c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="775c3-121">Authorization</span></span>|<span data-ttu-id="775c3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="775c3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="775c3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="775c3-123">Accept</span></span>|<span data-ttu-id="775c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="775c3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="775c3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="775c3-125">Request body</span></span>
<span data-ttu-id="775c3-126">No corpo da solicitação, fornece uma representação JSON para o objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="775c3-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="775c3-127">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="775c3-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="775c3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="775c3-128">Property</span></span>|<span data-ttu-id="775c3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="775c3-129">Type</span></span>|<span data-ttu-id="775c3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="775c3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775c3-131">id</span><span class="sxs-lookup"><span data-stu-id="775c3-131">id</span></span>|<span data-ttu-id="775c3-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="775c3-132">String</span></span>|<span data-ttu-id="775c3-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="775c3-133">The GUID for the object</span></span>|
|<span data-ttu-id="775c3-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="775c3-134">createdDateTimeUtc</span></span>|<span data-ttu-id="775c3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="775c3-135">DateTimeOffset</span></span>|<span data-ttu-id="775c3-136">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="775c3-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="775c3-137">status</span><span class="sxs-lookup"><span data-stu-id="775c3-137">status</span></span>|[<span data-ttu-id="775c3-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="775c3-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="775c3-139">Carrega o status.</span><span class="sxs-lookup"><span data-stu-id="775c3-139">Upload status.</span></span> <span data-ttu-id="775c3-140">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="775c3-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="775c3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="775c3-141">Response</span></span>
<span data-ttu-id="775c3-142">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="775c3-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775c3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="775c3-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="775c3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="775c3-144">Request</span></span>
<span data-ttu-id="775c3-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="775c3-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="775c3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="775c3-146">Response</span></span>
<span data-ttu-id="775c3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="775c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



