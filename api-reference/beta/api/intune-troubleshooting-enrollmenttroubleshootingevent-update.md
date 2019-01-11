---
title: Atualizar enrollmentTroubleshootingEvent
description: Atualiza as propriedades de um objeto enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 785835eb0daabd55add7d7d903990abd4725ab9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886202"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="184fc-103">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="184fc-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="184fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="184fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="184fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="184fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="184fc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="184fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="184fc-107">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="184fc-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="184fc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="184fc-108">Prerequisites</span></span>
<span data-ttu-id="184fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="184fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="184fc-111">Permission type</span></span>|<span data-ttu-id="184fc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="184fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="184fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="184fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="184fc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184fc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="184fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="184fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="184fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184fc-116">Not supported.</span></span>|
|<span data-ttu-id="184fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="184fc-117">Application</span></span>|<span data-ttu-id="184fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="184fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="184fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="184fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="184fc-120">Request headers</span></span>
|<span data-ttu-id="184fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="184fc-121">Header</span></span>|<span data-ttu-id="184fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="184fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="184fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="184fc-123">Authorization</span></span>|<span data-ttu-id="184fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="184fc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="184fc-125">Accept</span></span>|<span data-ttu-id="184fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="184fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="184fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="184fc-127">Request body</span></span>
<span data-ttu-id="184fc-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="184fc-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="184fc-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="184fc-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="184fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="184fc-130">Property</span></span>|<span data-ttu-id="184fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="184fc-131">Type</span></span>|<span data-ttu-id="184fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="184fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184fc-133">id</span><span class="sxs-lookup"><span data-stu-id="184fc-133">id</span></span>|<span data-ttu-id="184fc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-134">String</span></span>|<span data-ttu-id="184fc-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="184fc-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="184fc-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="184fc-136">eventDateTime</span></span>|<span data-ttu-id="184fc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="184fc-137">DateTimeOffset</span></span>|<span data-ttu-id="184fc-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="184fc-138">Time when the event occurred .</span></span> <span data-ttu-id="184fc-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="184fc-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="184fc-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="184fc-140">correlationId</span></span>|<span data-ttu-id="184fc-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-141">String</span></span>|<span data-ttu-id="184fc-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="184fc-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="184fc-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="184fc-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="184fc-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="184fc-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="184fc-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-145">String</span></span>|<span data-ttu-id="184fc-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="184fc-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="184fc-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="184fc-147">operatingSystem</span></span>|<span data-ttu-id="184fc-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-148">String</span></span>|<span data-ttu-id="184fc-149">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="184fc-149">Operating System.</span></span>|
|<span data-ttu-id="184fc-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="184fc-150">osVersion</span></span>|<span data-ttu-id="184fc-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-151">String</span></span>|<span data-ttu-id="184fc-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="184fc-152">OS Version.</span></span>|
|<span data-ttu-id="184fc-153">userId</span><span class="sxs-lookup"><span data-stu-id="184fc-153">userId</span></span>|<span data-ttu-id="184fc-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-154">String</span></span>|<span data-ttu-id="184fc-155">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="184fc-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="184fc-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="184fc-156">deviceId</span></span>|<span data-ttu-id="184fc-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-157">String</span></span>|<span data-ttu-id="184fc-158">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="184fc-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="184fc-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="184fc-159">enrollmentType</span></span>|[<span data-ttu-id="184fc-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="184fc-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="184fc-161">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="184fc-161">Type of the enrollment.</span></span> <span data-ttu-id="184fc-162">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="184fc-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="184fc-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="184fc-163">failureCategory</span></span>|[<span data-ttu-id="184fc-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="184fc-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="184fc-165">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="184fc-165">Highlevel failure category.</span></span> <span data-ttu-id="184fc-166">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="184fc-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="184fc-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="184fc-167">failureReason</span></span>|<span data-ttu-id="184fc-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="184fc-168">String</span></span>|<span data-ttu-id="184fc-169">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="184fc-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="184fc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="184fc-170">Response</span></span>
<span data-ttu-id="184fc-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="184fc-171">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="184fc-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="184fc-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="184fc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="184fc-173">Request</span></span>
<span data-ttu-id="184fc-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="184fc-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="184fc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="184fc-175">Response</span></span>
<span data-ttu-id="184fc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="184fc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





