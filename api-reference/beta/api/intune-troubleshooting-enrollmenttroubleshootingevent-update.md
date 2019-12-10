---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 882358073cbf0a7ffe124ed5dddff03898ff4e60
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938941"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="08a8b-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="08a8b-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="08a8b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08a8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08a8b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08a8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08a8b-106">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="08a8b-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08a8b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08a8b-107">Prerequisites</span></span>
<span data-ttu-id="08a8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08a8b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08a8b-110">Permission type</span></span>|<span data-ttu-id="08a8b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08a8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08a8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08a8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08a8b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a8b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08a8b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08a8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08a8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08a8b-115">Not supported.</span></span>|
|<span data-ttu-id="08a8b-116">Application</span><span class="sxs-lookup"><span data-stu-id="08a8b-116">Application</span></span>|<span data-ttu-id="08a8b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a8b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08a8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="08a8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a8b-119">Request headers</span></span>
|<span data-ttu-id="08a8b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08a8b-120">Header</span></span>|<span data-ttu-id="08a8b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="08a8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08a8b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a8b-122">Authorization</span></span>|<span data-ttu-id="08a8b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08a8b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08a8b-124">Accept</span></span>|<span data-ttu-id="08a8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08a8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08a8b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08a8b-126">Request body</span></span>
<span data-ttu-id="08a8b-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="08a8b-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="08a8b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="08a8b-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="08a8b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08a8b-129">Property</span></span>|<span data-ttu-id="08a8b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a8b-130">Type</span></span>|<span data-ttu-id="08a8b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08a8b-132">id</span><span class="sxs-lookup"><span data-stu-id="08a8b-132">id</span></span>|<span data-ttu-id="08a8b-133">String</span><span class="sxs-lookup"><span data-stu-id="08a8b-133">String</span></span>|<span data-ttu-id="08a8b-134">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="08a8b-135">eventDateTime</span></span>|<span data-ttu-id="08a8b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a8b-136">DateTimeOffset</span></span>|<span data-ttu-id="08a8b-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="08a8b-137">Time when the event occurred .</span></span> <span data-ttu-id="08a8b-138">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="08a8b-139">correlationId</span></span>|<span data-ttu-id="08a8b-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-140">String</span></span>|<span data-ttu-id="08a8b-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="08a8b-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="08a8b-142">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="08a8b-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="08a8b-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="08a8b-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="08a8b-145">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="08a8b-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="08a8b-146">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-147">EventName</span><span class="sxs-lookup"><span data-stu-id="08a8b-147">eventName</span></span>|<span data-ttu-id="08a8b-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-148">String</span></span>|<span data-ttu-id="08a8b-149">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="08a8b-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="08a8b-150">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="08a8b-151">additionalInformation</span></span>|<span data-ttu-id="08a8b-152">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="08a8b-153">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="08a8b-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="08a8b-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="08a8b-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="08a8b-155">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-155">String</span></span>|<span data-ttu-id="08a8b-156">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="08a8b-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="08a8b-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="08a8b-157">operatingSystem</span></span>|<span data-ttu-id="08a8b-158">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-158">String</span></span>|<span data-ttu-id="08a8b-159">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="08a8b-159">Operating System.</span></span>|
|<span data-ttu-id="08a8b-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="08a8b-160">osVersion</span></span>|<span data-ttu-id="08a8b-161">String</span><span class="sxs-lookup"><span data-stu-id="08a8b-161">String</span></span>|<span data-ttu-id="08a8b-162">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="08a8b-162">OS Version.</span></span>|
|<span data-ttu-id="08a8b-163">userId</span><span class="sxs-lookup"><span data-stu-id="08a8b-163">userId</span></span>|<span data-ttu-id="08a8b-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-164">String</span></span>|<span data-ttu-id="08a8b-165">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08a8b-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="08a8b-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="08a8b-166">deviceId</span></span>|<span data-ttu-id="08a8b-167">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-167">String</span></span>|<span data-ttu-id="08a8b-168">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08a8b-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="08a8b-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="08a8b-169">enrollmentType</span></span>|[<span data-ttu-id="08a8b-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="08a8b-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="08a8b-171">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="08a8b-171">Type of the enrollment.</span></span> <span data-ttu-id="08a8b-172">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="08a8b-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="08a8b-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="08a8b-173">failureCategory</span></span>|[<span data-ttu-id="08a8b-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="08a8b-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="08a8b-175">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="08a8b-175">Highlevel failure category.</span></span> <span data-ttu-id="08a8b-176">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="08a8b-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="08a8b-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="08a8b-177">failureReason</span></span>|<span data-ttu-id="08a8b-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08a8b-178">String</span></span>|<span data-ttu-id="08a8b-179">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="08a8b-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="08a8b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a8b-180">Response</span></span>
<span data-ttu-id="08a8b-181">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a8b-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a8b-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08a8b-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="08a8b-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a8b-183">Request</span></span>
<span data-ttu-id="08a8b-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a8b-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="08a8b-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a8b-185">Response</span></span>
<span data-ttu-id="08a8b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08a8b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1231

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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





