---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a112ee345df1ebf151889aa41d7ba8edba49bbee
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800127"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="c3ac0-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c3ac0-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="c3ac0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3ac0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ac0-106">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c3ac0-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3ac0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3ac0-107">Prerequisites</span></span>
<span data-ttu-id="c3ac0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3ac0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3ac0-110">Permission type</span></span>|<span data-ttu-id="c3ac0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3ac0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3ac0-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3ac0-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c3ac0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3ac0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-115">Not supported.</span></span>|
|<span data-ttu-id="c3ac0-116">Application</span><span class="sxs-lookup"><span data-stu-id="c3ac0-116">Application</span></span>|<span data-ttu-id="c3ac0-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3ac0-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3ac0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3ac0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c3ac0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ac0-119">Request headers</span></span>
|<span data-ttu-id="c3ac0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3ac0-120">Header</span></span>|<span data-ttu-id="c3ac0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3ac0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3ac0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3ac0-122">Authorization</span></span>|<span data-ttu-id="c3ac0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3ac0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3ac0-124">Accept</span></span>|<span data-ttu-id="c3ac0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3ac0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3ac0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ac0-126">Request body</span></span>
<span data-ttu-id="c3ac0-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c3ac0-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c3ac0-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c3ac0-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="c3ac0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3ac0-129">Property</span></span>|<span data-ttu-id="c3ac0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3ac0-130">Type</span></span>|<span data-ttu-id="c3ac0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3ac0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ac0-132">id</span><span class="sxs-lookup"><span data-stu-id="c3ac0-132">id</span></span>|<span data-ttu-id="c3ac0-133">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-133">String</span></span>|<span data-ttu-id="c3ac0-134">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c3ac0-135">eventDateTime</span></span>|<span data-ttu-id="c3ac0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3ac0-136">DateTimeOffset</span></span>|<span data-ttu-id="c3ac0-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-137">Time when the event occurred .</span></span> <span data-ttu-id="c3ac0-138">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="c3ac0-139">correlationId</span></span>|<span data-ttu-id="c3ac0-140">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-140">String</span></span>|<span data-ttu-id="c3ac0-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c3ac0-142">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c3ac0-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c3ac0-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c3ac0-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c3ac0-145">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c3ac0-146">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-147">EventName</span><span class="sxs-lookup"><span data-stu-id="c3ac0-147">eventName</span></span>|<span data-ttu-id="c3ac0-148">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-148">String</span></span>|<span data-ttu-id="c3ac0-149">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c3ac0-150">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="c3ac0-151">additionalInformation</span></span>|<span data-ttu-id="c3ac0-152">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c3ac0-153">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ac0-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c3ac0-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c3ac0-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="c3ac0-155">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-155">String</span></span>|<span data-ttu-id="c3ac0-156">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c3ac0-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c3ac0-157">operatingSystem</span></span>|<span data-ttu-id="c3ac0-158">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-158">String</span></span>|<span data-ttu-id="c3ac0-159">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-159">Operating System.</span></span>|
|<span data-ttu-id="c3ac0-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="c3ac0-160">osVersion</span></span>|<span data-ttu-id="c3ac0-161">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-161">String</span></span>|<span data-ttu-id="c3ac0-162">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-162">OS Version.</span></span>|
|<span data-ttu-id="c3ac0-163">userId</span><span class="sxs-lookup"><span data-stu-id="c3ac0-163">userId</span></span>|<span data-ttu-id="c3ac0-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3ac0-164">String</span></span>|<span data-ttu-id="c3ac0-165">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c3ac0-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="c3ac0-166">deviceId</span></span>|<span data-ttu-id="c3ac0-167">String</span><span class="sxs-lookup"><span data-stu-id="c3ac0-167">String</span></span>|<span data-ttu-id="c3ac0-168">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="c3ac0-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c3ac0-169">enrollmentType</span></span>|[<span data-ttu-id="c3ac0-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c3ac0-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c3ac0-171">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-171">Type of the enrollment.</span></span> <span data-ttu-id="c3ac0-172">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="c3ac0-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="c3ac0-173">failureCategory</span></span>|[<span data-ttu-id="c3ac0-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="c3ac0-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="c3ac0-175">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-175">Highlevel failure category.</span></span> <span data-ttu-id="c3ac0-176">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="c3ac0-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="c3ac0-177">failureReason</span></span>|<span data-ttu-id="c3ac0-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3ac0-178">String</span></span>|<span data-ttu-id="c3ac0-179">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="c3ac0-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3ac0-180">Response</span></span>
<span data-ttu-id="c3ac0-181">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3ac0-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3ac0-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3ac0-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ac0-183">Request</span></span>
<span data-ttu-id="c3ac0-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3ac0-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3ac0-185">Response</span></span>
<span data-ttu-id="c3ac0-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3ac0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




