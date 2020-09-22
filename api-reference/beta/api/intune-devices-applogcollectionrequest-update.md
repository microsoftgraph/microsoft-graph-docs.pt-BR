---
title: Atualizar appLogCollectionRequest
description: Atualiza as propriedades de um objeto appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 260f08af0ecb68383c61856c62d6cdcd442c5c3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062663"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="59575-103">Atualizar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="59575-103">Update appLogCollectionRequest</span></span>

<span data-ttu-id="59575-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59575-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59575-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59575-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59575-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59575-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59575-107">Atualiza as propriedades de um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="59575-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59575-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59575-108">Prerequisites</span></span>
<span data-ttu-id="59575-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59575-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59575-111">Permission type</span></span>|<span data-ttu-id="59575-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59575-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59575-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59575-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59575-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59575-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="59575-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59575-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59575-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59575-116">Not supported.</span></span>|
|<span data-ttu-id="59575-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59575-117">Application</span></span>|<span data-ttu-id="59575-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59575-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59575-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59575-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="59575-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59575-120">Request headers</span></span>
|<span data-ttu-id="59575-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59575-121">Header</span></span>|<span data-ttu-id="59575-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59575-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59575-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59575-123">Authorization</span></span>|<span data-ttu-id="59575-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59575-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59575-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59575-125">Accept</span></span>|<span data-ttu-id="59575-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59575-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59575-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59575-127">Request body</span></span>
<span data-ttu-id="59575-128">No corpo da solicitação, forneça uma representação JSON do objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="59575-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="59575-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="59575-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="59575-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59575-130">Property</span></span>|<span data-ttu-id="59575-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59575-131">Type</span></span>|<span data-ttu-id="59575-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59575-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59575-133">id</span><span class="sxs-lookup"><span data-stu-id="59575-133">id</span></span>|<span data-ttu-id="59575-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59575-134">String</span></span>|<span data-ttu-id="59575-135">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="59575-135">The unique Identifier.</span></span> <span data-ttu-id="59575-136">É userId_DeviceId_AppId ID.</span><span class="sxs-lookup"><span data-stu-id="59575-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="59575-137">status</span><span class="sxs-lookup"><span data-stu-id="59575-137">status</span></span>|[<span data-ttu-id="59575-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="59575-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="59575-139">Status de carregamento de logs.</span><span class="sxs-lookup"><span data-stu-id="59575-139">Log upload status.</span></span> <span data-ttu-id="59575-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="59575-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="59575-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="59575-141">errorMessage</span></span>|<span data-ttu-id="59575-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59575-142">String</span></span>|<span data-ttu-id="59575-143">Mensagem de erro se qualquer um durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="59575-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="59575-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="59575-144">customLogFolders</span></span>|<span data-ttu-id="59575-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="59575-145">String collection</span></span>|<span data-ttu-id="59575-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="59575-146">List of log folders.</span></span> |
|<span data-ttu-id="59575-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="59575-147">completedDateTime</span></span>|<span data-ttu-id="59575-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59575-148">DateTimeOffset</span></span>|<span data-ttu-id="59575-149">Hora em que a solicitação de log de carregamento alcançou um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="59575-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="59575-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="59575-150">Response</span></span>
<span data-ttu-id="59575-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59575-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59575-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59575-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="59575-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59575-153">Request</span></span>
<span data-ttu-id="59575-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59575-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59575-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="59575-155">Response</span></span>
<span data-ttu-id="59575-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59575-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






