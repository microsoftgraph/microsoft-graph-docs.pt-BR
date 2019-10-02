---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f53296202b3bfddb7632ff951258f269cdb11bd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360990"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="519e2-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="519e2-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="519e2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="519e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="519e2-105">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="519e2-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="519e2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="519e2-106">Prerequisites</span></span>
<span data-ttu-id="519e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="519e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="519e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="519e2-109">Permission type</span></span>|<span data-ttu-id="519e2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="519e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="519e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="519e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="519e2-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="519e2-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="519e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="519e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="519e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="519e2-114">Not supported.</span></span>|
|<span data-ttu-id="519e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="519e2-115">Application</span></span>|<span data-ttu-id="519e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="519e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="519e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="519e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="519e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="519e2-118">Request headers</span></span>
|<span data-ttu-id="519e2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="519e2-119">Header</span></span>|<span data-ttu-id="519e2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="519e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="519e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="519e2-121">Authorization</span></span>|<span data-ttu-id="519e2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="519e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="519e2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="519e2-123">Accept</span></span>|<span data-ttu-id="519e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="519e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="519e2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="519e2-125">Request body</span></span>
<span data-ttu-id="519e2-126">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="519e2-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="519e2-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="519e2-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="519e2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="519e2-128">Property</span></span>|<span data-ttu-id="519e2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="519e2-129">Type</span></span>|<span data-ttu-id="519e2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="519e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="519e2-131">id</span><span class="sxs-lookup"><span data-stu-id="519e2-131">id</span></span>|<span data-ttu-id="519e2-132">String</span><span class="sxs-lookup"><span data-stu-id="519e2-132">String</span></span>|<span data-ttu-id="519e2-133">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="519e2-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="519e2-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="519e2-134">eventDateTime</span></span>|<span data-ttu-id="519e2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="519e2-135">DateTimeOffset</span></span>|<span data-ttu-id="519e2-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="519e2-136">Time when the event occurred .</span></span> <span data-ttu-id="519e2-137">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="519e2-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="519e2-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="519e2-138">correlationId</span></span>|<span data-ttu-id="519e2-139">String</span><span class="sxs-lookup"><span data-stu-id="519e2-139">String</span></span>|<span data-ttu-id="519e2-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="519e2-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="519e2-141">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="519e2-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="519e2-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="519e2-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="519e2-143">String</span><span class="sxs-lookup"><span data-stu-id="519e2-143">String</span></span>|<span data-ttu-id="519e2-144">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="519e2-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="519e2-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="519e2-145">operatingSystem</span></span>|<span data-ttu-id="519e2-146">String</span><span class="sxs-lookup"><span data-stu-id="519e2-146">String</span></span>|<span data-ttu-id="519e2-147">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="519e2-147">Operating System.</span></span>|
|<span data-ttu-id="519e2-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="519e2-148">osVersion</span></span>|<span data-ttu-id="519e2-149">String</span><span class="sxs-lookup"><span data-stu-id="519e2-149">String</span></span>|<span data-ttu-id="519e2-150">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="519e2-150">OS Version.</span></span>|
|<span data-ttu-id="519e2-151">userId</span><span class="sxs-lookup"><span data-stu-id="519e2-151">userId</span></span>|<span data-ttu-id="519e2-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="519e2-152">String</span></span>|<span data-ttu-id="519e2-153">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="519e2-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="519e2-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="519e2-154">deviceId</span></span>|<span data-ttu-id="519e2-155">String</span><span class="sxs-lookup"><span data-stu-id="519e2-155">String</span></span>|<span data-ttu-id="519e2-156">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="519e2-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="519e2-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="519e2-157">enrollmentType</span></span>|[<span data-ttu-id="519e2-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="519e2-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="519e2-159">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="519e2-159">Type of the enrollment.</span></span> <span data-ttu-id="519e2-160">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="519e2-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="519e2-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="519e2-161">failureCategory</span></span>|[<span data-ttu-id="519e2-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="519e2-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="519e2-163">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="519e2-163">Highlevel failure category.</span></span> <span data-ttu-id="519e2-164">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="519e2-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="519e2-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="519e2-165">failureReason</span></span>|<span data-ttu-id="519e2-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="519e2-166">String</span></span>|<span data-ttu-id="519e2-167">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="519e2-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="519e2-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="519e2-168">Response</span></span>
<span data-ttu-id="519e2-169">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="519e2-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="519e2-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="519e2-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="519e2-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="519e2-171">Request</span></span>
<span data-ttu-id="519e2-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="519e2-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="519e2-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="519e2-173">Response</span></span>
<span data-ttu-id="519e2-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="519e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




