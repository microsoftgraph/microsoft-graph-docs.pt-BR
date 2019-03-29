---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f5e0941987ab2d41b53085471c3842e23c73c6e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984244"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="eb486-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="eb486-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="eb486-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb486-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb486-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb486-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb486-106">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="eb486-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb486-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb486-107">Prerequisites</span></span>
<span data-ttu-id="eb486-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb486-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb486-110">Permission type</span></span>|<span data-ttu-id="eb486-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb486-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb486-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb486-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb486-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb486-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eb486-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb486-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb486-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb486-115">Not supported.</span></span>|
|<span data-ttu-id="eb486-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb486-116">Application</span></span>|<span data-ttu-id="eb486-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb486-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb486-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb486-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="eb486-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb486-119">Request headers</span></span>
|<span data-ttu-id="eb486-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb486-120">Header</span></span>|<span data-ttu-id="eb486-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb486-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb486-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb486-122">Authorization</span></span>|<span data-ttu-id="eb486-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb486-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb486-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb486-124">Accept</span></span>|<span data-ttu-id="eb486-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb486-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb486-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb486-126">Request body</span></span>
<span data-ttu-id="eb486-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="eb486-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="eb486-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="eb486-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="eb486-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb486-129">Property</span></span>|<span data-ttu-id="eb486-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb486-130">Type</span></span>|<span data-ttu-id="eb486-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb486-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb486-132">id</span><span class="sxs-lookup"><span data-stu-id="eb486-132">id</span></span>|<span data-ttu-id="eb486-133">String</span><span class="sxs-lookup"><span data-stu-id="eb486-133">String</span></span>|<span data-ttu-id="eb486-134">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="eb486-135">eventDateTime</span></span>|<span data-ttu-id="eb486-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb486-136">DateTimeOffset</span></span>|<span data-ttu-id="eb486-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="eb486-137">Time when the event occurred .</span></span> <span data-ttu-id="eb486-138">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="eb486-139">correlationId</span></span>|<span data-ttu-id="eb486-140">String</span><span class="sxs-lookup"><span data-stu-id="eb486-140">String</span></span>|<span data-ttu-id="eb486-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="eb486-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="eb486-142">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="eb486-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="eb486-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="eb486-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="eb486-145">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="eb486-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="eb486-146">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-147">EventName</span><span class="sxs-lookup"><span data-stu-id="eb486-147">eventName</span></span>|<span data-ttu-id="eb486-148">String</span><span class="sxs-lookup"><span data-stu-id="eb486-148">String</span></span>|<span data-ttu-id="eb486-149">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="eb486-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="eb486-150">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="eb486-151">additionalInformation</span></span>|<span data-ttu-id="eb486-152">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="eb486-153">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="eb486-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="eb486-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb486-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="eb486-155">String</span><span class="sxs-lookup"><span data-stu-id="eb486-155">String</span></span>|<span data-ttu-id="eb486-156">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="eb486-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="eb486-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="eb486-157">operatingSystem</span></span>|<span data-ttu-id="eb486-158">String</span><span class="sxs-lookup"><span data-stu-id="eb486-158">String</span></span>|<span data-ttu-id="eb486-159">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="eb486-159">Operating System.</span></span>|
|<span data-ttu-id="eb486-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="eb486-160">osVersion</span></span>|<span data-ttu-id="eb486-161">String</span><span class="sxs-lookup"><span data-stu-id="eb486-161">String</span></span>|<span data-ttu-id="eb486-162">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="eb486-162">OS Version.</span></span>|
|<span data-ttu-id="eb486-163">userId</span><span class="sxs-lookup"><span data-stu-id="eb486-163">userId</span></span>|<span data-ttu-id="eb486-164">String</span><span class="sxs-lookup"><span data-stu-id="eb486-164">String</span></span>|<span data-ttu-id="eb486-165">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb486-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="eb486-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="eb486-166">deviceId</span></span>|<span data-ttu-id="eb486-167">String</span><span class="sxs-lookup"><span data-stu-id="eb486-167">String</span></span>|<span data-ttu-id="eb486-168">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb486-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="eb486-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="eb486-169">enrollmentType</span></span>|[<span data-ttu-id="eb486-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="eb486-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="eb486-171">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="eb486-171">Type of the enrollment.</span></span> <span data-ttu-id="eb486-172">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="eb486-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="eb486-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="eb486-173">failureCategory</span></span>|[<span data-ttu-id="eb486-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="eb486-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="eb486-175">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="eb486-175">Highlevel failure category.</span></span> <span data-ttu-id="eb486-176">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="eb486-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="eb486-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="eb486-177">failureReason</span></span>|<span data-ttu-id="eb486-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb486-178">String</span></span>|<span data-ttu-id="eb486-179">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="eb486-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="eb486-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb486-180">Response</span></span>
<span data-ttu-id="eb486-181">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb486-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb486-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb486-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb486-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb486-183">Request</span></span>
<span data-ttu-id="eb486-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb486-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb486-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb486-185">Response</span></span>
<span data-ttu-id="eb486-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb486-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




