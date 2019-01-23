---
title: Atualizar appLogCollectionRequest
description: Atualize as propriedades de um objeto appLogCollectionRequest.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55974ed3c5158d4b005402fe4d6350854a197656
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429164"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="639c8-103">Atualizar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="639c8-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="639c8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="639c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="639c8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="639c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="639c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="639c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="639c8-107">Atualize as propriedades de um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="639c8-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="639c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="639c8-108">Prerequisites</span></span>
<span data-ttu-id="639c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="639c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="639c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="639c8-111">Permission type</span></span>|<span data-ttu-id="639c8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="639c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="639c8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="639c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="639c8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="639c8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="639c8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="639c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="639c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="639c8-116">Not supported.</span></span>|
|<span data-ttu-id="639c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="639c8-117">Application</span></span>|<span data-ttu-id="639c8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="639c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="639c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="639c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="639c8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="639c8-120">Request headers</span></span>
|<span data-ttu-id="639c8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="639c8-121">Header</span></span>|<span data-ttu-id="639c8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="639c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="639c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="639c8-123">Authorization</span></span>|<span data-ttu-id="639c8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="639c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="639c8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="639c8-125">Accept</span></span>|<span data-ttu-id="639c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="639c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="639c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="639c8-127">Request body</span></span>
<span data-ttu-id="639c8-128">No corpo da solicitação, fornece uma representação JSON para o objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="639c8-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="639c8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="639c8-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="639c8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="639c8-130">Property</span></span>|<span data-ttu-id="639c8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="639c8-131">Type</span></span>|<span data-ttu-id="639c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="639c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="639c8-133">id</span><span class="sxs-lookup"><span data-stu-id="639c8-133">id</span></span>|<span data-ttu-id="639c8-134">String</span><span class="sxs-lookup"><span data-stu-id="639c8-134">String</span></span>|<span data-ttu-id="639c8-135">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="639c8-135">The unique Identifier.</span></span> <span data-ttu-id="639c8-136">Esse é o id de userId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="639c8-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="639c8-137">status</span><span class="sxs-lookup"><span data-stu-id="639c8-137">status</span></span>|[<span data-ttu-id="639c8-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="639c8-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="639c8-139">Status de carregamento de log.</span><span class="sxs-lookup"><span data-stu-id="639c8-139">Log upload status.</span></span> <span data-ttu-id="639c8-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="639c8-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="639c8-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="639c8-141">errorMessage</span></span>|<span data-ttu-id="639c8-142">String</span><span class="sxs-lookup"><span data-stu-id="639c8-142">String</span></span>|<span data-ttu-id="639c8-143">Mensagem de erro, se houver algum durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="639c8-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="639c8-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="639c8-144">customLogFolders</span></span>|<span data-ttu-id="639c8-145">String collection</span><span class="sxs-lookup"><span data-stu-id="639c8-145">String collection</span></span>|<span data-ttu-id="639c8-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="639c8-146">List of log folders.</span></span> |
|<span data-ttu-id="639c8-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="639c8-147">completedDateTime</span></span>|<span data-ttu-id="639c8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="639c8-148">DateTimeOffset</span></span>|<span data-ttu-id="639c8-149">Hora em que a solicitação de log de carregamento atingido um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="639c8-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="639c8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="639c8-150">Response</span></span>
<span data-ttu-id="639c8-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="639c8-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="639c8-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="639c8-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="639c8-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="639c8-153">Request</span></span>
<span data-ttu-id="639c8-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="639c8-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="639c8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="639c8-155">Response</span></span>
<span data-ttu-id="639c8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="639c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




