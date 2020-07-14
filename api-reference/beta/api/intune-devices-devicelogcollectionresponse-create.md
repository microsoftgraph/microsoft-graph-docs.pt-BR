---
title: Criar deviceLogCollectionResponse
description: Criar um novo objeto deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c11917ab1501aeebf7629cddf96ec9ea7f6d0fa
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124168"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="5c650-103">Criar deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="5c650-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="5c650-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c650-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c650-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c650-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c650-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c650-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c650-107">Criar um novo objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="5c650-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c650-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c650-108">Prerequisites</span></span>
<span data-ttu-id="5c650-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5c650-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5c650-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c650-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c650-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c650-111">Permission type</span></span>|<span data-ttu-id="5c650-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c650-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c650-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c650-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c650-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c650-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c650-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c650-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c650-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c650-116">Not supported.</span></span>|
|<span data-ttu-id="5c650-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c650-117">Application</span></span>|<span data-ttu-id="5c650-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c650-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c650-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c650-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="5c650-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c650-120">Request headers</span></span>
|<span data-ttu-id="5c650-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c650-121">Header</span></span>|<span data-ttu-id="5c650-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c650-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c650-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c650-123">Authorization</span></span>|<span data-ttu-id="5c650-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c650-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c650-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c650-125">Accept</span></span>|<span data-ttu-id="5c650-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c650-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c650-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c650-127">Request body</span></span>
<span data-ttu-id="5c650-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="5c650-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="5c650-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="5c650-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="5c650-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c650-130">Property</span></span>|<span data-ttu-id="5c650-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c650-131">Type</span></span>|<span data-ttu-id="5c650-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c650-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c650-133">id</span><span class="sxs-lookup"><span data-stu-id="5c650-133">id</span></span>|<span data-ttu-id="5c650-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c650-134">String</span></span>|<span data-ttu-id="5c650-135">O identificador exclusivo no formato de tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="5c650-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="5c650-136">status</span><span class="sxs-lookup"><span data-stu-id="5c650-136">status</span></span>|<span data-ttu-id="5c650-137">String</span><span class="sxs-lookup"><span data-stu-id="5c650-137">String</span></span>|<span data-ttu-id="5c650-138">O status da solicitação de coleção de logs</span><span class="sxs-lookup"><span data-stu-id="5c650-138">The status of the log collection request</span></span>|
|<span data-ttu-id="5c650-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5c650-139">managedDeviceId</span></span>|<span data-ttu-id="5c650-140">Guid</span><span class="sxs-lookup"><span data-stu-id="5c650-140">Guid</span></span>|<span data-ttu-id="5c650-141">A ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c650-141">The device Id</span></span>|
|<span data-ttu-id="5c650-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="5c650-142">errorCode</span></span>|<span data-ttu-id="5c650-143">Int64</span><span class="sxs-lookup"><span data-stu-id="5c650-143">Int64</span></span>|<span data-ttu-id="5c650-144">O código de erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="5c650-144">The error code, if any.</span></span> <span data-ttu-id="5c650-145">Valores válidos-9.22337203685478 E + 18 para 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="5c650-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="5c650-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="5c650-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="5c650-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c650-147">DateTimeOffset</span></span>|<span data-ttu-id="5c650-148">O DateTime da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c650-148">The DateTime of the request</span></span>|
|<span data-ttu-id="5c650-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="5c650-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="5c650-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c650-150">DateTimeOffset</span></span>|<span data-ttu-id="5c650-151">O DateTime que a solicitação foi recebida</span><span class="sxs-lookup"><span data-stu-id="5c650-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="5c650-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5c650-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="5c650-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c650-153">String</span></span>|<span data-ttu-id="5c650-154">O UPN para quem iniciou a solicitação</span><span class="sxs-lookup"><span data-stu-id="5c650-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="5c650-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="5c650-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="5c650-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c650-156">DateTimeOffset</span></span>|<span data-ttu-id="5c650-157">O DateTime do vencimento dos logs</span><span class="sxs-lookup"><span data-stu-id="5c650-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="5c650-158">size</span><span class="sxs-lookup"><span data-stu-id="5c650-158">size</span></span>|<span data-ttu-id="5c650-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="5c650-159">Double</span></span>|<span data-ttu-id="5c650-160">O tamanho dos logs.</span><span class="sxs-lookup"><span data-stu-id="5c650-160">The size of the logs.</span></span> <span data-ttu-id="5c650-161">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="5c650-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="5c650-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c650-162">Response</span></span>
<span data-ttu-id="5c650-163">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c650-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c650-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c650-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c650-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c650-165">Request</span></span>
<span data-ttu-id="5c650-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c650-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```

### <a name="response"></a><span data-ttu-id="5c650-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c650-167">Response</span></span>
<span data-ttu-id="5c650-168">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5c650-168">Here is an example of the response.</span></span> <span data-ttu-id="5c650-169">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5c650-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5c650-170">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5c650-170">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```



