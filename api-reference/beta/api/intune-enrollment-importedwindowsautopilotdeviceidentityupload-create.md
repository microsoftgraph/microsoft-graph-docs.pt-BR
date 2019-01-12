---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Crie um novo objeto de importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 414191348a6654e59a81c8e46c48bb3e7728a303
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913882"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="c687f-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="c687f-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="c687f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c687f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c687f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c687f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c687f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c687f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c687f-107">Crie um novo objeto de [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="c687f-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c687f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c687f-108">Prerequisites</span></span>
<span data-ttu-id="c687f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c687f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c687f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c687f-111">Permission type</span></span>|<span data-ttu-id="c687f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c687f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c687f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c687f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c687f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c687f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c687f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c687f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c687f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c687f-116">Not supported.</span></span>|
|<span data-ttu-id="c687f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c687f-117">Application</span></span>|<span data-ttu-id="c687f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c687f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c687f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c687f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="c687f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c687f-120">Request headers</span></span>
|<span data-ttu-id="c687f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c687f-121">Header</span></span>|<span data-ttu-id="c687f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c687f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c687f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c687f-123">Authorization</span></span>|<span data-ttu-id="c687f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c687f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c687f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c687f-125">Accept</span></span>|<span data-ttu-id="c687f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c687f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c687f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c687f-127">Request body</span></span>
<span data-ttu-id="c687f-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="c687f-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="c687f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="c687f-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="c687f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c687f-130">Property</span></span>|<span data-ttu-id="c687f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c687f-131">Type</span></span>|<span data-ttu-id="c687f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c687f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c687f-133">id</span><span class="sxs-lookup"><span data-stu-id="c687f-133">id</span></span>|<span data-ttu-id="c687f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c687f-134">String</span></span>|<span data-ttu-id="c687f-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="c687f-135">The GUID for the object</span></span>|
|<span data-ttu-id="c687f-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="c687f-136">createdDateTimeUtc</span></span>|<span data-ttu-id="c687f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c687f-137">DateTimeOffset</span></span>|<span data-ttu-id="c687f-138">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="c687f-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="c687f-139">status</span><span class="sxs-lookup"><span data-stu-id="c687f-139">status</span></span>|[<span data-ttu-id="c687f-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="c687f-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="c687f-141">Carrega o status.</span><span class="sxs-lookup"><span data-stu-id="c687f-141">Upload status.</span></span> <span data-ttu-id="c687f-142">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c687f-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="c687f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c687f-143">Response</span></span>
<span data-ttu-id="c687f-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c687f-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c687f-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c687f-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c687f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c687f-146">Request</span></span>
<span data-ttu-id="c687f-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c687f-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c687f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c687f-148">Response</span></span>
<span data-ttu-id="c687f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c687f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





