---
title: Atualizar appLogCollectionRequest
description: Atualize as propriedades de um objeto appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e69edbbc9dd874e89246223c90736bc3034acc2
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612109"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="e029f-103">Atualizar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e029f-103">Update appLogCollectionRequest</span></span>

<span data-ttu-id="e029f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e029f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e029f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e029f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e029f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e029f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e029f-107">Atualize as propriedades de um [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="e029f-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e029f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e029f-108">Prerequisites</span></span>
<span data-ttu-id="e029f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e029f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e029f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e029f-111">Permission type</span></span>|<span data-ttu-id="e029f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e029f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e029f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e029f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e029f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e029f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e029f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e029f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e029f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e029f-116">Not supported.</span></span>|
|<span data-ttu-id="e029f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e029f-117">Application</span></span>|<span data-ttu-id="e029f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e029f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e029f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e029f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="e029f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e029f-120">Request headers</span></span>
|<span data-ttu-id="e029f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e029f-121">Header</span></span>|<span data-ttu-id="e029f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e029f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e029f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e029f-123">Authorization</span></span>|<span data-ttu-id="e029f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e029f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e029f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e029f-125">Accept</span></span>|<span data-ttu-id="e029f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e029f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e029f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e029f-127">Request body</span></span>
<span data-ttu-id="e029f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="e029f-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="e029f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e029f-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="e029f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e029f-130">Property</span></span>|<span data-ttu-id="e029f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e029f-131">Type</span></span>|<span data-ttu-id="e029f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e029f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e029f-133">id</span><span class="sxs-lookup"><span data-stu-id="e029f-133">id</span></span>|<span data-ttu-id="e029f-134">String</span><span class="sxs-lookup"><span data-stu-id="e029f-134">String</span></span>|<span data-ttu-id="e029f-135">O Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="e029f-135">The unique Identifier.</span></span> <span data-ttu-id="e029f-136">Esta é userId_DeviceId_AppId id.</span><span class="sxs-lookup"><span data-stu-id="e029f-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="e029f-137">status</span><span class="sxs-lookup"><span data-stu-id="e029f-137">status</span></span>|[<span data-ttu-id="e029f-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="e029f-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="e029f-139">Status do carregamento de log.</span><span class="sxs-lookup"><span data-stu-id="e029f-139">Log upload status.</span></span> <span data-ttu-id="e029f-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e029f-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="e029f-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="e029f-141">errorMessage</span></span>|<span data-ttu-id="e029f-142">String</span><span class="sxs-lookup"><span data-stu-id="e029f-142">String</span></span>|<span data-ttu-id="e029f-143">Mensagem de erro se alguma durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="e029f-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="e029f-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="e029f-144">customLogFolders</span></span>|<span data-ttu-id="e029f-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e029f-145">String collection</span></span>|<span data-ttu-id="e029f-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="e029f-146">List of log folders.</span></span> |
|<span data-ttu-id="e029f-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e029f-147">completedDateTime</span></span>|<span data-ttu-id="e029f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e029f-148">DateTimeOffset</span></span>|<span data-ttu-id="e029f-149">Hora em que a solicitação de log de carregamento atingiu um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="e029f-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="e029f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e029f-150">Response</span></span>
<span data-ttu-id="e029f-151">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e029f-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e029f-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e029f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e029f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e029f-153">Request</span></span>
<span data-ttu-id="e029f-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e029f-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e029f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e029f-155">Response</span></span>
<span data-ttu-id="e029f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e029f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




