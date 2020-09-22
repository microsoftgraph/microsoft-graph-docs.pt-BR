---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08ba36bedae02a7b2749601c69412aaf9a5eb450
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028732"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="8a881-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8a881-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="8a881-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a881-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a881-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a881-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a881-106">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8a881-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a881-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a881-107">Prerequisites</span></span>
<span data-ttu-id="8a881-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a881-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a881-110">Permission type</span></span>|<span data-ttu-id="8a881-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a881-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a881-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a881-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a881-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a881-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a881-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a881-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a881-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a881-115">Not supported.</span></span>|
|<span data-ttu-id="8a881-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a881-116">Application</span></span>|<span data-ttu-id="8a881-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a881-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a881-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a881-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="8a881-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a881-119">Request headers</span></span>
|<span data-ttu-id="8a881-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a881-120">Header</span></span>|<span data-ttu-id="8a881-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8a881-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a881-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a881-122">Authorization</span></span>|<span data-ttu-id="8a881-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a881-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a881-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a881-124">Accept</span></span>|<span data-ttu-id="8a881-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a881-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a881-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a881-126">Request body</span></span>
<span data-ttu-id="8a881-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8a881-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="8a881-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8a881-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="8a881-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a881-129">Property</span></span>|<span data-ttu-id="8a881-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a881-130">Type</span></span>|<span data-ttu-id="8a881-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a881-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a881-132">id</span><span class="sxs-lookup"><span data-stu-id="8a881-132">id</span></span>|<span data-ttu-id="8a881-133">String</span><span class="sxs-lookup"><span data-stu-id="8a881-133">String</span></span>|<span data-ttu-id="8a881-134">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8a881-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8a881-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8a881-135">eventDateTime</span></span>|<span data-ttu-id="8a881-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a881-136">DateTimeOffset</span></span>|<span data-ttu-id="8a881-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="8a881-137">Time when the event occurred .</span></span> <span data-ttu-id="8a881-138">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8a881-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8a881-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="8a881-139">correlationId</span></span>|<span data-ttu-id="8a881-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-140">String</span></span>|<span data-ttu-id="8a881-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="8a881-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8a881-142">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8a881-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8a881-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a881-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="8a881-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-144">String</span></span>|<span data-ttu-id="8a881-145">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="8a881-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8a881-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8a881-146">operatingSystem</span></span>|<span data-ttu-id="8a881-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-147">String</span></span>|<span data-ttu-id="8a881-148">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="8a881-148">Operating System.</span></span>|
|<span data-ttu-id="8a881-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="8a881-149">osVersion</span></span>|<span data-ttu-id="8a881-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-150">String</span></span>|<span data-ttu-id="8a881-151">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="8a881-151">OS Version.</span></span>|
|<span data-ttu-id="8a881-152">userId</span><span class="sxs-lookup"><span data-stu-id="8a881-152">userId</span></span>|<span data-ttu-id="8a881-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-153">String</span></span>|<span data-ttu-id="8a881-154">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a881-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8a881-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="8a881-155">deviceId</span></span>|<span data-ttu-id="8a881-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-156">String</span></span>|<span data-ttu-id="8a881-157">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a881-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8a881-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8a881-158">enrollmentType</span></span>|[<span data-ttu-id="8a881-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8a881-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8a881-160">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="8a881-160">Type of the enrollment.</span></span> <span data-ttu-id="8a881-161">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="8a881-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="8a881-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8a881-162">failureCategory</span></span>|[<span data-ttu-id="8a881-163">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="8a881-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="8a881-164">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="8a881-164">Highlevel failure category.</span></span> <span data-ttu-id="8a881-165">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="8a881-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="8a881-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="8a881-166">failureReason</span></span>|<span data-ttu-id="8a881-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a881-167">String</span></span>|<span data-ttu-id="8a881-168">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="8a881-168">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8a881-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a881-169">Response</span></span>
<span data-ttu-id="8a881-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a881-170">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a881-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a881-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a881-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a881-172">Request</span></span>
<span data-ttu-id="8a881-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a881-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="8a881-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a881-174">Response</span></span>
<span data-ttu-id="8a881-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a881-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```









