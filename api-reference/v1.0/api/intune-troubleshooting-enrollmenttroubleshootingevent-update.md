---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a16a24a27a56ab1a733b46fa9ad9b7469f0a8ee3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975767"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="9710d-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9710d-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="9710d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9710d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9710d-105">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9710d-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9710d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9710d-106">Prerequisites</span></span>
<span data-ttu-id="9710d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9710d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9710d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9710d-109">Permission type</span></span>|<span data-ttu-id="9710d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9710d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9710d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9710d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9710d-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9710d-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9710d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9710d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9710d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9710d-114">Not supported.</span></span>|
|<span data-ttu-id="9710d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9710d-115">Application</span></span>|<span data-ttu-id="9710d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9710d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9710d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9710d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="9710d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9710d-118">Request headers</span></span>
|<span data-ttu-id="9710d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9710d-119">Header</span></span>|<span data-ttu-id="9710d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9710d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9710d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9710d-121">Authorization</span></span>|<span data-ttu-id="9710d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9710d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9710d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9710d-123">Accept</span></span>|<span data-ttu-id="9710d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9710d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9710d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9710d-125">Request body</span></span>
<span data-ttu-id="9710d-126">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9710d-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="9710d-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9710d-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="9710d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9710d-128">Property</span></span>|<span data-ttu-id="9710d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9710d-129">Type</span></span>|<span data-ttu-id="9710d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9710d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9710d-131">id</span><span class="sxs-lookup"><span data-stu-id="9710d-131">id</span></span>|<span data-ttu-id="9710d-132">String</span><span class="sxs-lookup"><span data-stu-id="9710d-132">String</span></span>|<span data-ttu-id="9710d-133">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9710d-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9710d-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9710d-134">eventDateTime</span></span>|<span data-ttu-id="9710d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9710d-135">DateTimeOffset</span></span>|<span data-ttu-id="9710d-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="9710d-136">Time when the event occurred .</span></span> <span data-ttu-id="9710d-137">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9710d-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9710d-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="9710d-138">correlationId</span></span>|<span data-ttu-id="9710d-139">String</span><span class="sxs-lookup"><span data-stu-id="9710d-139">String</span></span>|<span data-ttu-id="9710d-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="9710d-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="9710d-141">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9710d-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9710d-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9710d-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="9710d-143">String</span><span class="sxs-lookup"><span data-stu-id="9710d-143">String</span></span>|<span data-ttu-id="9710d-144">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="9710d-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="9710d-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9710d-145">operatingSystem</span></span>|<span data-ttu-id="9710d-146">String</span><span class="sxs-lookup"><span data-stu-id="9710d-146">String</span></span>|<span data-ttu-id="9710d-147">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9710d-147">Operating System.</span></span>|
|<span data-ttu-id="9710d-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="9710d-148">osVersion</span></span>|<span data-ttu-id="9710d-149">String</span><span class="sxs-lookup"><span data-stu-id="9710d-149">String</span></span>|<span data-ttu-id="9710d-150">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9710d-150">OS Version.</span></span>|
|<span data-ttu-id="9710d-151">userId</span><span class="sxs-lookup"><span data-stu-id="9710d-151">userId</span></span>|<span data-ttu-id="9710d-152">String</span><span class="sxs-lookup"><span data-stu-id="9710d-152">String</span></span>|<span data-ttu-id="9710d-153">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9710d-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="9710d-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="9710d-154">deviceId</span></span>|<span data-ttu-id="9710d-155">String</span><span class="sxs-lookup"><span data-stu-id="9710d-155">String</span></span>|<span data-ttu-id="9710d-156">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9710d-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="9710d-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="9710d-157">enrollmentType</span></span>|[<span data-ttu-id="9710d-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9710d-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="9710d-159">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="9710d-159">Type of the enrollment.</span></span> <span data-ttu-id="9710d-160">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="9710d-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="9710d-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="9710d-161">failureCategory</span></span>|[<span data-ttu-id="9710d-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="9710d-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="9710d-163">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="9710d-163">Highlevel failure category.</span></span> <span data-ttu-id="9710d-164">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="9710d-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="9710d-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="9710d-165">failureReason</span></span>|<span data-ttu-id="9710d-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9710d-166">String</span></span>|<span data-ttu-id="9710d-167">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="9710d-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="9710d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="9710d-168">Response</span></span>
<span data-ttu-id="9710d-169">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9710d-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9710d-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9710d-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="9710d-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9710d-171">Request</span></span>
<span data-ttu-id="9710d-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9710d-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9710d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9710d-173">Response</span></span>
<span data-ttu-id="9710d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9710d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



