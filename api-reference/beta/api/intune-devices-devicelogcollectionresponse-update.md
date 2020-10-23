---
title: Atualizar deviceLogCollectionResponse
description: Atualiza as propriedades de um objeto deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6dade84eeb03fbfedc846d6ef7740579146fff8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696836"
---
# <a name="update-devicelogcollectionresponse"></a><span data-ttu-id="aa85d-103">Atualizar deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="aa85d-103">Update deviceLogCollectionResponse</span></span>

<span data-ttu-id="aa85d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa85d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa85d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa85d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa85d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa85d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa85d-107">Atualiza as propriedades de um objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="aa85d-107">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa85d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa85d-108">Prerequisites</span></span>
<span data-ttu-id="aa85d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa85d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa85d-111">Permission type</span></span>|<span data-ttu-id="aa85d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa85d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa85d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa85d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa85d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa85d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aa85d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa85d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa85d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa85d-116">Not supported.</span></span>|
|<span data-ttu-id="aa85d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa85d-117">Application</span></span>|<span data-ttu-id="aa85d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa85d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa85d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa85d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="aa85d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa85d-120">Request headers</span></span>
|<span data-ttu-id="aa85d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa85d-121">Header</span></span>|<span data-ttu-id="aa85d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aa85d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa85d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa85d-123">Authorization</span></span>|<span data-ttu-id="aa85d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa85d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa85d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa85d-125">Accept</span></span>|<span data-ttu-id="aa85d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa85d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa85d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa85d-127">Request body</span></span>
<span data-ttu-id="aa85d-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="aa85d-128">In the request body, supply a JSON representation for the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

<span data-ttu-id="aa85d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span><span class="sxs-lookup"><span data-stu-id="aa85d-129">The following table shows the properties that are required when you create the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>

|<span data-ttu-id="aa85d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa85d-130">Property</span></span>|<span data-ttu-id="aa85d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa85d-131">Type</span></span>|<span data-ttu-id="aa85d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa85d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa85d-133">id</span><span class="sxs-lookup"><span data-stu-id="aa85d-133">id</span></span>|<span data-ttu-id="aa85d-134">String</span><span class="sxs-lookup"><span data-stu-id="aa85d-134">String</span></span>|<span data-ttu-id="aa85d-135">O identificador exclusivo no formato de tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="aa85d-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="aa85d-136">status</span><span class="sxs-lookup"><span data-stu-id="aa85d-136">status</span></span>|<span data-ttu-id="aa85d-137">String</span><span class="sxs-lookup"><span data-stu-id="aa85d-137">String</span></span>|<span data-ttu-id="aa85d-138">O status da solicitação de coleção de logs</span><span class="sxs-lookup"><span data-stu-id="aa85d-138">The status of the log collection request</span></span>|
|<span data-ttu-id="aa85d-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="aa85d-139">managedDeviceId</span></span>|<span data-ttu-id="aa85d-140">Guid</span><span class="sxs-lookup"><span data-stu-id="aa85d-140">Guid</span></span>|<span data-ttu-id="aa85d-141">A ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aa85d-141">The device Id</span></span>|
|<span data-ttu-id="aa85d-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="aa85d-142">errorCode</span></span>|<span data-ttu-id="aa85d-143">Int64</span><span class="sxs-lookup"><span data-stu-id="aa85d-143">Int64</span></span>|<span data-ttu-id="aa85d-144">O código de erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="aa85d-144">The error code, if any.</span></span> <span data-ttu-id="aa85d-145">Valores válidos-9.22337203685478 E + 18 para 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="aa85d-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="aa85d-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="aa85d-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="aa85d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa85d-147">DateTimeOffset</span></span>|<span data-ttu-id="aa85d-148">O DateTime da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa85d-148">The DateTime of the request</span></span>|
|<span data-ttu-id="aa85d-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="aa85d-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="aa85d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa85d-150">DateTimeOffset</span></span>|<span data-ttu-id="aa85d-151">O DateTime que a solicitação foi recebida</span><span class="sxs-lookup"><span data-stu-id="aa85d-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="aa85d-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa85d-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="aa85d-153">String</span><span class="sxs-lookup"><span data-stu-id="aa85d-153">String</span></span>|<span data-ttu-id="aa85d-154">O UPN para quem iniciou a solicitação</span><span class="sxs-lookup"><span data-stu-id="aa85d-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="aa85d-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="aa85d-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="aa85d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa85d-156">DateTimeOffset</span></span>|<span data-ttu-id="aa85d-157">O DateTime do vencimento dos logs</span><span class="sxs-lookup"><span data-stu-id="aa85d-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="aa85d-158">size</span><span class="sxs-lookup"><span data-stu-id="aa85d-158">size</span></span>|<span data-ttu-id="aa85d-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="aa85d-159">Double</span></span>|<span data-ttu-id="aa85d-160">O tamanho dos logs.</span><span class="sxs-lookup"><span data-stu-id="aa85d-160">The size of the logs.</span></span> <span data-ttu-id="aa85d-161">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="aa85d-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="aa85d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa85d-162">Response</span></span>
<span data-ttu-id="aa85d-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa85d-163">If successful, this method returns a `200 OK` response code and an updated [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa85d-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa85d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa85d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa85d-165">Request</span></span>
<span data-ttu-id="aa85d-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa85d-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
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

### <a name="response"></a><span data-ttu-id="aa85d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa85d-167">Response</span></span>
<span data-ttu-id="aa85d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa85d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





