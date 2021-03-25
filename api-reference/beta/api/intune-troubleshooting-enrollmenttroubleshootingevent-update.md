---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac5fa06e43a83a6c8de58e1b79faa8f78a50172f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151897"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="e01a5-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e01a5-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="e01a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e01a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e01a5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e01a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e01a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e01a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e01a5-107">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e01a5-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e01a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e01a5-108">Prerequisites</span></span>
<span data-ttu-id="e01a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e01a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e01a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e01a5-111">Permission type</span></span>|<span data-ttu-id="e01a5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e01a5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e01a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e01a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e01a5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01a5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e01a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e01a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e01a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e01a5-116">Not supported.</span></span>|
|<span data-ttu-id="e01a5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e01a5-117">Application</span></span>|<span data-ttu-id="e01a5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01a5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e01a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e01a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e01a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e01a5-120">Request headers</span></span>
|<span data-ttu-id="e01a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e01a5-121">Header</span></span>|<span data-ttu-id="e01a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e01a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e01a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e01a5-123">Authorization</span></span>|<span data-ttu-id="e01a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e01a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e01a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e01a5-125">Accept</span></span>|<span data-ttu-id="e01a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e01a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e01a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e01a5-127">Request body</span></span>
<span data-ttu-id="e01a5-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e01a5-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e01a5-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e01a5-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="e01a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e01a5-130">Property</span></span>|<span data-ttu-id="e01a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e01a5-131">Type</span></span>|<span data-ttu-id="e01a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e01a5-133">id</span><span class="sxs-lookup"><span data-stu-id="e01a5-133">id</span></span>|<span data-ttu-id="e01a5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-134">String</span></span>|<span data-ttu-id="e01a5-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e01a5-136">eventDateTime</span></span>|<span data-ttu-id="e01a5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e01a5-137">DateTimeOffset</span></span>|<span data-ttu-id="e01a5-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e01a5-138">Time when the event occurred .</span></span> <span data-ttu-id="e01a5-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="e01a5-140">correlationId</span></span>|<span data-ttu-id="e01a5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-141">String</span></span>|<span data-ttu-id="e01a5-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="e01a5-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e01a5-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e01a5-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e01a5-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e01a5-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e01a5-146">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="e01a5-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="e01a5-147">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-148">eventName</span><span class="sxs-lookup"><span data-stu-id="e01a5-148">eventName</span></span>|<span data-ttu-id="e01a5-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-149">String</span></span>|<span data-ttu-id="e01a5-150">Nome do Evento correspondente ao Evento de Solução de Problemas.</span><span class="sxs-lookup"><span data-stu-id="e01a5-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e01a5-151">É um campo Opcional Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e01a5-152">additionalInformation</span></span>|<span data-ttu-id="e01a5-153">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e01a5-154">Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Troubleshooting Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e01a5-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e01a5-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e01a5-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="e01a5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-156">String</span></span>|<span data-ttu-id="e01a5-157">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="e01a5-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e01a5-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e01a5-158">operatingSystem</span></span>|<span data-ttu-id="e01a5-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-159">String</span></span>|<span data-ttu-id="e01a5-160">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e01a5-160">Operating System.</span></span>|
|<span data-ttu-id="e01a5-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="e01a5-161">osVersion</span></span>|<span data-ttu-id="e01a5-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-162">String</span></span>|<span data-ttu-id="e01a5-163">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e01a5-163">OS Version.</span></span>|
|<span data-ttu-id="e01a5-164">userId</span><span class="sxs-lookup"><span data-stu-id="e01a5-164">userId</span></span>|<span data-ttu-id="e01a5-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-165">String</span></span>|<span data-ttu-id="e01a5-166">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e01a5-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e01a5-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="e01a5-167">deviceId</span></span>|<span data-ttu-id="e01a5-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-168">String</span></span>|<span data-ttu-id="e01a5-169">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e01a5-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="e01a5-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="e01a5-170">enrollmentType</span></span>|[<span data-ttu-id="e01a5-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e01a5-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="e01a5-172">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="e01a5-172">Type of the enrollment.</span></span> <span data-ttu-id="e01a5-173">Os valores possíveis são: `unknown` , , , , , , , , `userEnrollment` , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , , , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` , `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="e01a5-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="e01a5-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="e01a5-174">failureCategory</span></span>|[<span data-ttu-id="e01a5-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e01a5-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="e01a5-176">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="e01a5-176">Highlevel failure category.</span></span> <span data-ttu-id="e01a5-177">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="e01a5-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="e01a5-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="e01a5-178">failureReason</span></span>|<span data-ttu-id="e01a5-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01a5-179">String</span></span>|<span data-ttu-id="e01a5-180">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="e01a5-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="e01a5-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01a5-181">Response</span></span>
<span data-ttu-id="e01a5-182">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e01a5-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e01a5-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e01a5-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="e01a5-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e01a5-184">Request</span></span>
<span data-ttu-id="e01a5-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e01a5-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e01a5-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01a5-186">Response</span></span>
<span data-ttu-id="e01a5-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e01a5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




