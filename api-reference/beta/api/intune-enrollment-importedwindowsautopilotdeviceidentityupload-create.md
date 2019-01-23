---
title: Criar importedWindowsAutopilotDeviceIdentityUpload
description: Crie um novo objeto de importedWindowsAutopilotDeviceIdentityUpload.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e47e3c8545335f0f34511e7d0b87bf2bd54d2162
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396809"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="9be33-103">Criar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="9be33-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="9be33-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9be33-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9be33-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9be33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9be33-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9be33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9be33-107">Crie um novo objeto de [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="9be33-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9be33-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9be33-108">Prerequisites</span></span>
<span data-ttu-id="9be33-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9be33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9be33-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be33-111">Permission type</span></span>|<span data-ttu-id="9be33-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9be33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9be33-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9be33-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be33-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9be33-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9be33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be33-116">Not supported.</span></span>|
|<span data-ttu-id="9be33-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be33-117">Application</span></span>|<span data-ttu-id="9be33-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be33-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9be33-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="9be33-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be33-120">Request headers</span></span>
|<span data-ttu-id="9be33-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9be33-121">Header</span></span>|<span data-ttu-id="9be33-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9be33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9be33-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9be33-123">Authorization</span></span>|<span data-ttu-id="9be33-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9be33-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9be33-125">Accept</span></span>|<span data-ttu-id="9be33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9be33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9be33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be33-127">Request body</span></span>
<span data-ttu-id="9be33-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="9be33-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="9be33-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="9be33-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="9be33-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9be33-130">Property</span></span>|<span data-ttu-id="9be33-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9be33-131">Type</span></span>|<span data-ttu-id="9be33-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9be33-133">id</span><span class="sxs-lookup"><span data-stu-id="9be33-133">id</span></span>|<span data-ttu-id="9be33-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9be33-134">String</span></span>|<span data-ttu-id="9be33-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="9be33-135">The GUID for the object</span></span>|
|<span data-ttu-id="9be33-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="9be33-136">createdDateTimeUtc</span></span>|<span data-ttu-id="9be33-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9be33-137">DateTimeOffset</span></span>|<span data-ttu-id="9be33-138">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="9be33-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="9be33-139">status</span><span class="sxs-lookup"><span data-stu-id="9be33-139">status</span></span>|[<span data-ttu-id="9be33-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="9be33-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="9be33-141">Carrega o status.</span><span class="sxs-lookup"><span data-stu-id="9be33-141">Upload status.</span></span> <span data-ttu-id="9be33-142">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="9be33-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="9be33-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be33-143">Response</span></span>
<span data-ttu-id="9be33-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be33-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9be33-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9be33-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="9be33-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be33-146">Request</span></span>
<span data-ttu-id="9be33-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9be33-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9be33-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be33-148">Response</span></span>
<span data-ttu-id="9be33-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9be33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




