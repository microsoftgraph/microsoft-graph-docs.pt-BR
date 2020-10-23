---
title: Criar appLogCollectionRequest
description: Criar um novo objeto appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14c0664b7644f54a7df688f1d1448dc972385ff7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723235"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="58f3e-103">Criar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="58f3e-103">Create appLogCollectionRequest</span></span>

<span data-ttu-id="58f3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58f3e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58f3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58f3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58f3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58f3e-107">Criar um novo objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="58f3e-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58f3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58f3e-108">Prerequisites</span></span>
<span data-ttu-id="58f3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58f3e-111">Permission type</span></span>|<span data-ttu-id="58f3e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58f3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58f3e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58f3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58f3e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58f3e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58f3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58f3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58f3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58f3e-116">Not supported.</span></span>|
|<span data-ttu-id="58f3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58f3e-117">Application</span></span>|<span data-ttu-id="58f3e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58f3e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58f3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58f3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="58f3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58f3e-120">Request headers</span></span>
|<span data-ttu-id="58f3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58f3e-121">Header</span></span>|<span data-ttu-id="58f3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58f3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58f3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58f3e-123">Authorization</span></span>|<span data-ttu-id="58f3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58f3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58f3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58f3e-125">Accept</span></span>|<span data-ttu-id="58f3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58f3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58f3e-127">Request body</span></span>
<span data-ttu-id="58f3e-128">No corpo da solicitação, forneça uma representação JSON do objeto appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="58f3e-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="58f3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="58f3e-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="58f3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58f3e-130">Property</span></span>|<span data-ttu-id="58f3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58f3e-131">Type</span></span>|<span data-ttu-id="58f3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f3e-133">id</span><span class="sxs-lookup"><span data-stu-id="58f3e-133">id</span></span>|<span data-ttu-id="58f3e-134">String</span><span class="sxs-lookup"><span data-stu-id="58f3e-134">String</span></span>|<span data-ttu-id="58f3e-135">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="58f3e-135">The unique Identifier.</span></span> <span data-ttu-id="58f3e-136">É userId_DeviceId_AppId ID.</span><span class="sxs-lookup"><span data-stu-id="58f3e-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="58f3e-137">status</span><span class="sxs-lookup"><span data-stu-id="58f3e-137">status</span></span>|[<span data-ttu-id="58f3e-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="58f3e-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="58f3e-139">Status de carregamento de logs.</span><span class="sxs-lookup"><span data-stu-id="58f3e-139">Log upload status.</span></span> <span data-ttu-id="58f3e-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="58f3e-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="58f3e-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="58f3e-141">errorMessage</span></span>|<span data-ttu-id="58f3e-142">String</span><span class="sxs-lookup"><span data-stu-id="58f3e-142">String</span></span>|<span data-ttu-id="58f3e-143">Mensagem de erro se qualquer um durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="58f3e-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="58f3e-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="58f3e-144">customLogFolders</span></span>|<span data-ttu-id="58f3e-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="58f3e-145">String collection</span></span>|<span data-ttu-id="58f3e-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="58f3e-146">List of log folders.</span></span> |
|<span data-ttu-id="58f3e-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="58f3e-147">completedDateTime</span></span>|<span data-ttu-id="58f3e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58f3e-148">DateTimeOffset</span></span>|<span data-ttu-id="58f3e-149">Hora em que a solicitação de log de carregamento alcançou um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="58f3e-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="58f3e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f3e-150">Response</span></span>
<span data-ttu-id="58f3e-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58f3e-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f3e-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58f3e-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="58f3e-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58f3e-153">Request</span></span>
<span data-ttu-id="58f3e-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58f3e-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58f3e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f3e-155">Response</span></span>
<span data-ttu-id="58f3e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58f3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





