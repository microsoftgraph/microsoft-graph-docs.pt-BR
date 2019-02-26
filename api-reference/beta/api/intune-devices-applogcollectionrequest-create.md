---
title: Criar appLogCollectionRequest
description: Criar um novo objeto appLogCollectionRequest.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da12791aab74c59d82b8efb4c98629ac1d809112
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144993"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="ad0d7-103">Criar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="ad0d7-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="ad0d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad0d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad0d7-106">Criar um novo objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ad0d7-106">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad0d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad0d7-107">Prerequisites</span></span>
<span data-ttu-id="ad0d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ad0d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad0d7-110">Permission type</span></span>|<span data-ttu-id="ad0d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad0d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad0d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad0d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad0d7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0d7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad0d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad0d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad0d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-115">Not supported.</span></span>|
|<span data-ttu-id="ad0d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad0d7-116">Application</span></span>|<span data-ttu-id="ad0d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad0d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad0d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="ad0d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad0d7-119">Request headers</span></span>
|<span data-ttu-id="ad0d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad0d7-120">Header</span></span>|<span data-ttu-id="ad0d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ad0d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad0d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad0d7-122">Authorization</span></span>|<span data-ttu-id="ad0d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad0d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad0d7-124">Accept</span></span>|<span data-ttu-id="ad0d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad0d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad0d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad0d7-126">Request body</span></span>
<span data-ttu-id="ad0d7-127">No corpo da solicitação, forneça uma representação JSON do objeto appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-127">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="ad0d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-128">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="ad0d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad0d7-129">Property</span></span>|<span data-ttu-id="ad0d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad0d7-130">Type</span></span>|<span data-ttu-id="ad0d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad0d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad0d7-132">id</span><span class="sxs-lookup"><span data-stu-id="ad0d7-132">id</span></span>|<span data-ttu-id="ad0d7-133">String</span><span class="sxs-lookup"><span data-stu-id="ad0d7-133">String</span></span>|<span data-ttu-id="ad0d7-134">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-134">The unique Identifier.</span></span> <span data-ttu-id="ad0d7-135">Esta é a ID do userId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="ad0d7-136">status</span><span class="sxs-lookup"><span data-stu-id="ad0d7-136">status</span></span>|[<span data-ttu-id="ad0d7-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="ad0d7-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="ad0d7-138">Status de carregamento de logs.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-138">Log upload status.</span></span> <span data-ttu-id="ad0d7-139">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ad0d7-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="ad0d7-140">errorMessage</span></span>|<span data-ttu-id="ad0d7-141">String</span><span class="sxs-lookup"><span data-stu-id="ad0d7-141">String</span></span>|<span data-ttu-id="ad0d7-142">Mensagem de erro se qualquer um durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="ad0d7-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="ad0d7-143">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="ad0d7-143">customLogFolders</span></span>|<span data-ttu-id="ad0d7-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad0d7-144">String collection</span></span>|<span data-ttu-id="ad0d7-145">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-145">List of log folders.</span></span> |
|<span data-ttu-id="ad0d7-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad0d7-146">completedDateTime</span></span>|<span data-ttu-id="ad0d7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad0d7-147">DateTimeOffset</span></span>|<span data-ttu-id="ad0d7-148">Hora em que a solicitação de log de carregamento alcançou um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="ad0d7-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="ad0d7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad0d7-149">Response</span></span>
<span data-ttu-id="ad0d7-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-150">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad0d7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad0d7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad0d7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad0d7-152">Request</span></span>
<span data-ttu-id="ad0d7-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
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

### <a name="response"></a><span data-ttu-id="ad0d7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad0d7-154">Response</span></span>
<span data-ttu-id="ad0d7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad0d7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




