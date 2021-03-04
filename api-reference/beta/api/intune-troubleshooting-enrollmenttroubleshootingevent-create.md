---
title: Criar enrollmentTroubleshootingEvent
description: Cria um novo objeto enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1aaa9daedd9ea9306871b17f5833063569b7879b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448001"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="d6202-103">Criar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="d6202-103">Create enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="d6202-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6202-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6202-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6202-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6202-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6202-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6202-107">Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d6202-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6202-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6202-108">Prerequisites</span></span>
<span data-ttu-id="d6202-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6202-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6202-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6202-111">Permission type</span></span>|<span data-ttu-id="d6202-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6202-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6202-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6202-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6202-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6202-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6202-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6202-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6202-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6202-116">Not supported.</span></span>|
|<span data-ttu-id="d6202-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6202-117">Application</span></span>|<span data-ttu-id="d6202-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6202-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6202-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6202-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d6202-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6202-120">Request headers</span></span>
|<span data-ttu-id="d6202-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6202-121">Header</span></span>|<span data-ttu-id="d6202-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6202-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6202-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6202-123">Authorization</span></span>|<span data-ttu-id="d6202-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6202-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6202-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6202-125">Accept</span></span>|<span data-ttu-id="d6202-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6202-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6202-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6202-127">Request body</span></span>
<span data-ttu-id="d6202-128">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="d6202-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="d6202-129">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="d6202-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="d6202-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6202-130">Property</span></span>|<span data-ttu-id="d6202-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6202-131">Type</span></span>|<span data-ttu-id="d6202-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6202-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6202-133">id</span><span class="sxs-lookup"><span data-stu-id="d6202-133">id</span></span>|<span data-ttu-id="d6202-134">String</span><span class="sxs-lookup"><span data-stu-id="d6202-134">String</span></span>|<span data-ttu-id="d6202-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d6202-136">eventDateTime</span></span>|<span data-ttu-id="d6202-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6202-137">DateTimeOffset</span></span>|<span data-ttu-id="d6202-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="d6202-138">Time when the event occurred .</span></span> <span data-ttu-id="d6202-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="d6202-140">correlationId</span></span>|<span data-ttu-id="d6202-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-141">String</span></span>|<span data-ttu-id="d6202-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="d6202-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="d6202-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d6202-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="d6202-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d6202-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="d6202-146">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="d6202-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="d6202-147">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-148">eventName</span><span class="sxs-lookup"><span data-stu-id="d6202-148">eventName</span></span>|<span data-ttu-id="d6202-149">String</span><span class="sxs-lookup"><span data-stu-id="d6202-149">String</span></span>|<span data-ttu-id="d6202-150">Nome do Evento correspondente ao Evento de Solução de Problemas.</span><span class="sxs-lookup"><span data-stu-id="d6202-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="d6202-151">É um campo Opcional Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="d6202-152">additionalInformation</span></span>|<span data-ttu-id="d6202-153">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d6202-154">Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Troubleshooting Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d6202-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d6202-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6202-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="d6202-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-156">String</span></span>|<span data-ttu-id="d6202-157">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="d6202-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="d6202-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d6202-158">operatingSystem</span></span>|<span data-ttu-id="d6202-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-159">String</span></span>|<span data-ttu-id="d6202-160">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="d6202-160">Operating System.</span></span>|
|<span data-ttu-id="d6202-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="d6202-161">osVersion</span></span>|<span data-ttu-id="d6202-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-162">String</span></span>|<span data-ttu-id="d6202-163">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="d6202-163">OS Version.</span></span>|
|<span data-ttu-id="d6202-164">userId</span><span class="sxs-lookup"><span data-stu-id="d6202-164">userId</span></span>|<span data-ttu-id="d6202-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-165">String</span></span>|<span data-ttu-id="d6202-166">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6202-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="d6202-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="d6202-167">deviceId</span></span>|<span data-ttu-id="d6202-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-168">String</span></span>|<span data-ttu-id="d6202-169">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6202-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="d6202-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="d6202-170">enrollmentType</span></span>|[<span data-ttu-id="d6202-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d6202-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d6202-172">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="d6202-172">Type of the enrollment.</span></span> <span data-ttu-id="d6202-173">Os valores possíveis são: `unknown` , , , , , , , , `userEnrollment` , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , , , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` , `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="d6202-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="d6202-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="d6202-174">failureCategory</span></span>|[<span data-ttu-id="d6202-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="d6202-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="d6202-176">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="d6202-176">Highlevel failure category.</span></span> <span data-ttu-id="d6202-177">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="d6202-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="d6202-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="d6202-178">failureReason</span></span>|<span data-ttu-id="d6202-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6202-179">String</span></span>|<span data-ttu-id="d6202-180">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="d6202-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="d6202-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6202-181">Response</span></span>
<span data-ttu-id="d6202-182">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6202-182">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6202-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6202-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6202-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6202-184">Request</span></span>
<span data-ttu-id="d6202-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6202-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="d6202-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6202-186">Response</span></span>
<span data-ttu-id="d6202-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6202-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




