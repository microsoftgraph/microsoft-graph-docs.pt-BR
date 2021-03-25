---
title: Atualizar deviceLogCollectionResponse
description: Atualize as propriedades de um objeto deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed85268897942ba953ccdd5240d120829f6ea400
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154361"
---
# <a name="update-devicelogcollectionresponse"></a><span data-ttu-id="91430-103">Atualizar deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="91430-103">Update deviceLogCollectionResponse</span></span>

<span data-ttu-id="91430-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91430-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91430-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91430-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91430-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91430-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91430-107">Atualize as propriedades de um [objeto deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="91430-107">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91430-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91430-108">Prerequisites</span></span>
<span data-ttu-id="91430-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91430-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91430-111">Permission type</span></span>|<span data-ttu-id="91430-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91430-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91430-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91430-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91430-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91430-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="91430-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91430-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91430-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91430-116">Not supported.</span></span>|
|<span data-ttu-id="91430-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91430-117">Application</span></span>|<span data-ttu-id="91430-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91430-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91430-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91430-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="91430-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91430-120">Request headers</span></span>
|<span data-ttu-id="91430-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91430-121">Header</span></span>|<span data-ttu-id="91430-122">Valor</span><span class="sxs-lookup"><span data-stu-id="91430-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91430-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91430-123">Authorization</span></span>|<span data-ttu-id="91430-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91430-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91430-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91430-125">Accept</span></span>|<span data-ttu-id="91430-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91430-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91430-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91430-127">Request body</span></span>
<span data-ttu-id="91430-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="91430-128">In the request body, supply a JSON representation for the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

<span data-ttu-id="91430-129">A tabela a seguir mostra as propriedades necessárias ao criar [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span><span class="sxs-lookup"><span data-stu-id="91430-129">The following table shows the properties that are required when you create the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>

|<span data-ttu-id="91430-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91430-130">Property</span></span>|<span data-ttu-id="91430-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="91430-131">Type</span></span>|<span data-ttu-id="91430-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="91430-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91430-133">id</span><span class="sxs-lookup"><span data-stu-id="91430-133">id</span></span>|<span data-ttu-id="91430-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91430-134">String</span></span>|<span data-ttu-id="91430-135">O identificador exclusivo na forma de tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="91430-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="91430-136">status</span><span class="sxs-lookup"><span data-stu-id="91430-136">status</span></span>|<span data-ttu-id="91430-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91430-137">String</span></span>|<span data-ttu-id="91430-138">O status da solicitação do conjunto de log</span><span class="sxs-lookup"><span data-stu-id="91430-138">The status of the log collection request</span></span>|
|<span data-ttu-id="91430-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="91430-139">managedDeviceId</span></span>|<span data-ttu-id="91430-140">Guid</span><span class="sxs-lookup"><span data-stu-id="91430-140">Guid</span></span>|<span data-ttu-id="91430-141">A ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91430-141">The device Id</span></span>|
|<span data-ttu-id="91430-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="91430-142">errorCode</span></span>|<span data-ttu-id="91430-143">Int64</span><span class="sxs-lookup"><span data-stu-id="91430-143">Int64</span></span>|<span data-ttu-id="91430-144">O código de erro, se for o caso.</span><span class="sxs-lookup"><span data-stu-id="91430-144">The error code, if any.</span></span> <span data-ttu-id="91430-145">Valores válidos -9.22337203685478E+18 a 9.22337203685478E+18</span><span class="sxs-lookup"><span data-stu-id="91430-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="91430-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="91430-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="91430-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91430-147">DateTimeOffset</span></span>|<span data-ttu-id="91430-148">DateTime da solicitação</span><span class="sxs-lookup"><span data-stu-id="91430-148">The DateTime of the request</span></span>|
|<span data-ttu-id="91430-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="91430-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="91430-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91430-150">DateTimeOffset</span></span>|<span data-ttu-id="91430-151">DateTime a solicitação foi recebida</span><span class="sxs-lookup"><span data-stu-id="91430-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="91430-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="91430-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="91430-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91430-153">String</span></span>|<span data-ttu-id="91430-154">O UPN para quem iniciou a solicitação</span><span class="sxs-lookup"><span data-stu-id="91430-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="91430-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="91430-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="91430-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91430-156">DateTimeOffset</span></span>|<span data-ttu-id="91430-157">DateTime da expiração dos logs</span><span class="sxs-lookup"><span data-stu-id="91430-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="91430-158">size</span><span class="sxs-lookup"><span data-stu-id="91430-158">size</span></span>|<span data-ttu-id="91430-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="91430-159">Double</span></span>|<span data-ttu-id="91430-160">O tamanho dos logs.</span><span class="sxs-lookup"><span data-stu-id="91430-160">The size of the logs.</span></span> <span data-ttu-id="91430-161">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="91430-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="91430-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="91430-162">Response</span></span>
<span data-ttu-id="91430-163">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91430-163">If successful, this method returns a `200 OK` response code and an updated [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91430-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91430-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="91430-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91430-165">Request</span></span>
<span data-ttu-id="91430-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91430-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91430-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="91430-167">Response</span></span>
<span data-ttu-id="91430-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91430-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




