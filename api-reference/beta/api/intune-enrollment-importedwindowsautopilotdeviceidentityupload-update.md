---
title: Atualizar importedWindowsAutopilotDeviceIdentityUpload
description: Atualize as propriedades de um objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76e699ebf7f0704ab6a524c1c5869339e0318ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894373"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="e63ee-103">Atualizar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="e63ee-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="e63ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e63ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e63ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e63ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e63ee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e63ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e63ee-107">Atualize as propriedades de um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="e63ee-107">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e63ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e63ee-108">Prerequisites</span></span>
<span data-ttu-id="e63ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e63ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e63ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e63ee-111">Permission type</span></span>|<span data-ttu-id="e63ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e63ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e63ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e63ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e63ee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e63ee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e63ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e63ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e63ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e63ee-116">Not supported.</span></span>|
|<span data-ttu-id="e63ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e63ee-117">Application</span></span>|<span data-ttu-id="e63ee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e63ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e63ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e63ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="e63ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e63ee-120">Request headers</span></span>
|<span data-ttu-id="e63ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e63ee-121">Header</span></span>|<span data-ttu-id="e63ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e63ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e63ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e63ee-123">Authorization</span></span>|<span data-ttu-id="e63ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e63ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e63ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e63ee-125">Accept</span></span>|<span data-ttu-id="e63ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e63ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e63ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e63ee-127">Request body</span></span>
<span data-ttu-id="e63ee-128">No corpo da solicitação, fornece uma representação JSON para o objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="e63ee-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="e63ee-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="e63ee-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="e63ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e63ee-130">Property</span></span>|<span data-ttu-id="e63ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e63ee-131">Type</span></span>|<span data-ttu-id="e63ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e63ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63ee-133">id</span><span class="sxs-lookup"><span data-stu-id="e63ee-133">id</span></span>|<span data-ttu-id="e63ee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e63ee-134">String</span></span>|<span data-ttu-id="e63ee-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e63ee-135">The GUID for the object</span></span>|
|<span data-ttu-id="e63ee-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="e63ee-136">createdDateTimeUtc</span></span>|<span data-ttu-id="e63ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e63ee-137">DateTimeOffset</span></span>|<span data-ttu-id="e63ee-138">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="e63ee-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="e63ee-139">status</span><span class="sxs-lookup"><span data-stu-id="e63ee-139">status</span></span>|[<span data-ttu-id="e63ee-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e63ee-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="e63ee-141">Carrega o status.</span><span class="sxs-lookup"><span data-stu-id="e63ee-141">Upload status.</span></span> <span data-ttu-id="e63ee-142">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="e63ee-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="e63ee-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e63ee-143">Response</span></span>
<span data-ttu-id="e63ee-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e63ee-144">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e63ee-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e63ee-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="e63ee-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e63ee-146">Request</span></span>
<span data-ttu-id="e63ee-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e63ee-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="e63ee-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e63ee-148">Response</span></span>
<span data-ttu-id="e63ee-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e63ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





