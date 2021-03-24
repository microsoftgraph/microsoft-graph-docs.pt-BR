---
title: Criar appLogCollectionRequest
description: Crie um novo objeto appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbd19f042c6dbfe80a4c02ec224fde5b1e5fb696
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136479"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="6a627-103">Criar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="6a627-103">Create appLogCollectionRequest</span></span>

<span data-ttu-id="6a627-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a627-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a627-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a627-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a627-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a627-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a627-107">Crie um novo [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="6a627-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a627-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a627-108">Prerequisites</span></span>
<span data-ttu-id="6a627-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a627-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a627-111">Permission type</span></span>|<span data-ttu-id="6a627-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a627-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a627-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a627-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a627-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a627-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6a627-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a627-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a627-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a627-116">Not supported.</span></span>|
|<span data-ttu-id="6a627-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a627-117">Application</span></span>|<span data-ttu-id="6a627-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a627-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a627-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a627-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="6a627-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a627-120">Request headers</span></span>
|<span data-ttu-id="6a627-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a627-121">Header</span></span>|<span data-ttu-id="6a627-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a627-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a627-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a627-123">Authorization</span></span>|<span data-ttu-id="6a627-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a627-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a627-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a627-125">Accept</span></span>|<span data-ttu-id="6a627-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a627-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a627-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a627-127">Request body</span></span>
<span data-ttu-id="6a627-128">No corpo da solicitação, fornece uma representação JSON para o objeto appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="6a627-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="6a627-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="6a627-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="6a627-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a627-130">Property</span></span>|<span data-ttu-id="6a627-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a627-131">Type</span></span>|<span data-ttu-id="6a627-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a627-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a627-133">id</span><span class="sxs-lookup"><span data-stu-id="6a627-133">id</span></span>|<span data-ttu-id="6a627-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a627-134">String</span></span>|<span data-ttu-id="6a627-135">O Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="6a627-135">The unique Identifier.</span></span> <span data-ttu-id="6a627-136">Esta é userId_DeviceId_AppId id.</span><span class="sxs-lookup"><span data-stu-id="6a627-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="6a627-137">status</span><span class="sxs-lookup"><span data-stu-id="6a627-137">status</span></span>|[<span data-ttu-id="6a627-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="6a627-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="6a627-139">Status do carregamento de log.</span><span class="sxs-lookup"><span data-stu-id="6a627-139">Log upload status.</span></span> <span data-ttu-id="6a627-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6a627-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="6a627-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="6a627-141">errorMessage</span></span>|<span data-ttu-id="6a627-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a627-142">String</span></span>|<span data-ttu-id="6a627-143">Mensagem de erro se alguma durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="6a627-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="6a627-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="6a627-144">customLogFolders</span></span>|<span data-ttu-id="6a627-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a627-145">String collection</span></span>|<span data-ttu-id="6a627-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="6a627-146">List of log folders.</span></span> |
|<span data-ttu-id="6a627-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a627-147">completedDateTime</span></span>|<span data-ttu-id="6a627-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a627-148">DateTimeOffset</span></span>|<span data-ttu-id="6a627-149">Hora em que a solicitação de log de carregamento atingiu um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="6a627-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="6a627-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a627-150">Response</span></span>
<span data-ttu-id="6a627-151">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a627-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a627-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a627-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a627-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a627-153">Request</span></span>
<span data-ttu-id="6a627-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a627-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a627-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a627-155">Response</span></span>
<span data-ttu-id="6a627-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a627-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




