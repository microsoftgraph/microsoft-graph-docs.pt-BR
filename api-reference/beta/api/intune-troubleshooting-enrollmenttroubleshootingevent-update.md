---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 33f4a789834ee7fdc84c000d065df932203efb0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914469"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="13a21-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="13a21-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="13a21-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13a21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13a21-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13a21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13a21-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13a21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13a21-107">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="13a21-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13a21-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13a21-108">Prerequisites</span></span>
<span data-ttu-id="13a21-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a21-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13a21-111">Permission type</span></span>|<span data-ttu-id="13a21-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13a21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13a21-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13a21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13a21-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13a21-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13a21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13a21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13a21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a21-116">Not supported.</span></span>|
|<span data-ttu-id="13a21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13a21-117">Application</span></span>|<span data-ttu-id="13a21-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13a21-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13a21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="13a21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13a21-120">Request headers</span></span>
|<span data-ttu-id="13a21-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13a21-121">Header</span></span>|<span data-ttu-id="13a21-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13a21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13a21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13a21-123">Authorization</span></span>|<span data-ttu-id="13a21-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13a21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13a21-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13a21-125">Accept</span></span>|<span data-ttu-id="13a21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13a21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13a21-127">Request body</span></span>
<span data-ttu-id="13a21-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="13a21-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="13a21-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="13a21-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="13a21-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13a21-130">Property</span></span>|<span data-ttu-id="13a21-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13a21-131">Type</span></span>|<span data-ttu-id="13a21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13a21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a21-133">id</span><span class="sxs-lookup"><span data-stu-id="13a21-133">id</span></span>|<span data-ttu-id="13a21-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-134">String</span></span>|<span data-ttu-id="13a21-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="13a21-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="13a21-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="13a21-136">eventDateTime</span></span>|<span data-ttu-id="13a21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13a21-137">DateTimeOffset</span></span>|<span data-ttu-id="13a21-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="13a21-138">Time when the event occurred .</span></span> <span data-ttu-id="13a21-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="13a21-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="13a21-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="13a21-140">correlationId</span></span>|<span data-ttu-id="13a21-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-141">String</span></span>|<span data-ttu-id="13a21-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="13a21-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="13a21-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="13a21-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="13a21-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="13a21-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="13a21-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-145">String</span></span>|<span data-ttu-id="13a21-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="13a21-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="13a21-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="13a21-147">operatingSystem</span></span>|<span data-ttu-id="13a21-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-148">String</span></span>|<span data-ttu-id="13a21-149">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="13a21-149">Operating System.</span></span>|
|<span data-ttu-id="13a21-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="13a21-150">osVersion</span></span>|<span data-ttu-id="13a21-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-151">String</span></span>|<span data-ttu-id="13a21-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="13a21-152">OS Version.</span></span>|
|<span data-ttu-id="13a21-153">userId</span><span class="sxs-lookup"><span data-stu-id="13a21-153">userId</span></span>|<span data-ttu-id="13a21-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-154">String</span></span>|<span data-ttu-id="13a21-155">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13a21-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="13a21-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="13a21-156">deviceId</span></span>|<span data-ttu-id="13a21-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-157">String</span></span>|<span data-ttu-id="13a21-158">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13a21-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="13a21-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="13a21-159">enrollmentType</span></span>|[<span data-ttu-id="13a21-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13a21-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="13a21-161">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="13a21-161">Type of the enrollment.</span></span> <span data-ttu-id="13a21-162">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="13a21-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="13a21-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="13a21-163">failureCategory</span></span>|[<span data-ttu-id="13a21-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="13a21-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="13a21-165">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="13a21-165">Highlevel failure category.</span></span> <span data-ttu-id="13a21-166">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="13a21-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="13a21-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="13a21-167">failureReason</span></span>|<span data-ttu-id="13a21-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13a21-168">String</span></span>|<span data-ttu-id="13a21-169">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="13a21-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="13a21-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a21-170">Response</span></span>
<span data-ttu-id="13a21-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13a21-171">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a21-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13a21-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="13a21-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13a21-173">Request</span></span>
<span data-ttu-id="13a21-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13a21-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="13a21-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a21-175">Response</span></span>
<span data-ttu-id="13a21-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13a21-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





