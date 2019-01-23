---
title: Criar appLogCollectionRequest
description: Crie um novo objeto de appLogCollectionRequest.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c3afd1cf00ba706e3fbc1e960e649fc010ae582f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429150"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="d5bea-103">Criar appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="d5bea-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="d5bea-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5bea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5bea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5bea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5bea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d5bea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5bea-107">Crie um novo objeto de [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d5bea-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5bea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5bea-108">Prerequisites</span></span>
<span data-ttu-id="d5bea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d5bea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d5bea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5bea-111">Permission type</span></span>|<span data-ttu-id="d5bea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5bea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5bea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5bea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5bea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5bea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d5bea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5bea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5bea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bea-116">Not supported.</span></span>|
|<span data-ttu-id="d5bea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5bea-117">Application</span></span>|<span data-ttu-id="d5bea-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5bea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="d5bea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bea-120">Request headers</span></span>
|<span data-ttu-id="d5bea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5bea-121">Header</span></span>|<span data-ttu-id="d5bea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5bea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5bea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5bea-123">Authorization</span></span>|<span data-ttu-id="d5bea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5bea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5bea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5bea-125">Accept</span></span>|<span data-ttu-id="d5bea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5bea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bea-127">Request body</span></span>
<span data-ttu-id="d5bea-128">No corpo da solicitação, fornece uma representação JSON para o objeto appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="d5bea-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="d5bea-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="d5bea-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="d5bea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5bea-130">Property</span></span>|<span data-ttu-id="d5bea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5bea-131">Type</span></span>|<span data-ttu-id="d5bea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5bea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5bea-133">id</span><span class="sxs-lookup"><span data-stu-id="d5bea-133">id</span></span>|<span data-ttu-id="d5bea-134">String</span><span class="sxs-lookup"><span data-stu-id="d5bea-134">String</span></span>|<span data-ttu-id="d5bea-135">O identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d5bea-135">The unique Identifier.</span></span> <span data-ttu-id="d5bea-136">Esse é o id de userId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="d5bea-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="d5bea-137">status</span><span class="sxs-lookup"><span data-stu-id="d5bea-137">status</span></span>|[<span data-ttu-id="d5bea-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="d5bea-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="d5bea-139">Status de carregamento de log.</span><span class="sxs-lookup"><span data-stu-id="d5bea-139">Log upload status.</span></span> <span data-ttu-id="d5bea-140">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d5bea-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="d5bea-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="d5bea-141">errorMessage</span></span>|<span data-ttu-id="d5bea-142">String</span><span class="sxs-lookup"><span data-stu-id="d5bea-142">String</span></span>|<span data-ttu-id="d5bea-143">Mensagem de erro, se houver algum durante o processo de carregamento</span><span class="sxs-lookup"><span data-stu-id="d5bea-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="d5bea-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="d5bea-144">customLogFolders</span></span>|<span data-ttu-id="d5bea-145">String collection</span><span class="sxs-lookup"><span data-stu-id="d5bea-145">String collection</span></span>|<span data-ttu-id="d5bea-146">Lista de pastas de log.</span><span class="sxs-lookup"><span data-stu-id="d5bea-146">List of log folders.</span></span> |
|<span data-ttu-id="d5bea-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5bea-147">completedDateTime</span></span>|<span data-ttu-id="d5bea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5bea-148">DateTimeOffset</span></span>|<span data-ttu-id="d5bea-149">Hora em que a solicitação de log de carregamento atingido um estado de terminal</span><span class="sxs-lookup"><span data-stu-id="d5bea-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="d5bea-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bea-150">Response</span></span>
<span data-ttu-id="d5bea-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bea-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5bea-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5bea-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5bea-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bea-153">Request</span></span>
<span data-ttu-id="d5bea-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5bea-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5bea-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bea-155">Response</span></span>
<span data-ttu-id="d5bea-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5bea-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




