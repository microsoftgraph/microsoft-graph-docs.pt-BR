---
title: Atualizar appLogCollectionRequest
description: Atualiza as propriedades de um objeto appLogCollectionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bd90622a2062e80f16b090e5930e5cba18f405c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910599"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="5a2e8-103">Atualizar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="5a2e8-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="5a2e8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a2e8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a2e8-106">Atualiza as propriedades de um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2e8-106">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a2e8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a2e8-107">Prerequisites</span></span>
<span data-ttu-id="5a2e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a2e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a2e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a2e8-110">Permission type</span></span>|<span data-ttu-id="5a2e8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a2e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a2e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a2e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a2e8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2e8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a2e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a2e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a2e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-115">Not supported.</span></span>|
|<span data-ttu-id="5a2e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a2e8-116">Application</span></span>|<span data-ttu-id="5a2e8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a2e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a2e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="5a2e8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2e8-119">Request headers</span></span>
|<span data-ttu-id="5a2e8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a2e8-120">Header</span></span>|<span data-ttu-id="5a2e8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5a2e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a2e8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a2e8-122">Authorization</span></span>|<span data-ttu-id="5a2e8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a2e8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a2e8-124">Accept</span></span>|<span data-ttu-id="5a2e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a2e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a2e8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2e8-126">Request body</span></span>
<span data-ttu-id="5a2e8-127">No corpo da solicitação, forneça uma representação JSON do objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2e8-127">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="5a2e8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="5a2e8-128">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="5a2e8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a2e8-129">Property</span></span>|<span data-ttu-id="5a2e8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a2e8-130">Type</span></span>|<span data-ttu-id="5a2e8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2e8-132">id</span><span class="sxs-lookup"><span data-stu-id="5a2e8-132">id</span></span>|<span data-ttu-id="5a2e8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a2e8-133">String</span></span>|<span data-ttu-id="5a2e8-134">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-134">The unique Identifier.</span></span> <span data-ttu-id="5a2e8-135">Esta é a ID do userId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="5a2e8-136">status</span><span class="sxs-lookup"><span data-stu-id="5a2e8-136">status</span></span>|[<span data-ttu-id="5a2e8-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="5a2e8-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="5a2e8-138">Status de carregamento de logs.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-138">Log upload status.</span></span> <span data-ttu-id="5a2e8-139">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="5a2e8-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="5a2e8-140">errorMessage</span></span>|<span data-ttu-id="5a2e8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a2e8-141">String</span></span>|<span data-ttu-id="5a2e8-142">Mensagem de erro se qualquer um durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="5a2e8-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="5a2e8-143">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="5a2e8-143">customLogFolders</span></span>|<span data-ttu-id="5a2e8-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a2e8-144">String collection</span></span>|<span data-ttu-id="5a2e8-145">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-145">List of log folders.</span></span> |
|<span data-ttu-id="5a2e8-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2e8-146">completedDateTime</span></span>|<span data-ttu-id="5a2e8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2e8-147">DateTimeOffset</span></span>|<span data-ttu-id="5a2e8-148">Hora em que a solicitação de log de carregamento alcançou um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="5a2e8-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="5a2e8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2e8-149">Response</span></span>
<span data-ttu-id="5a2e8-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-150">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2e8-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a2e8-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a2e8-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2e8-152">Request</span></span>
<span data-ttu-id="5a2e8-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5a2e8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2e8-154">Response</span></span>
<span data-ttu-id="5a2e8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a2e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```




