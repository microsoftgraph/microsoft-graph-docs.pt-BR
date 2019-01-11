---
title: Criar enrollmentTroubleshootingEvent
description: Cria um novo objeto enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94e3f1f98a8400d7794863e7b3852d50be97b712
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872685"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="de7eb-103">Criar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="de7eb-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="de7eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de7eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de7eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de7eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de7eb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de7eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de7eb-107">Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="de7eb-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de7eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de7eb-108">Prerequisites</span></span>
<span data-ttu-id="de7eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de7eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de7eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de7eb-111">Permission type</span></span>|<span data-ttu-id="de7eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de7eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de7eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de7eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de7eb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de7eb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="de7eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de7eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de7eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de7eb-116">Not supported.</span></span>|
|<span data-ttu-id="de7eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de7eb-117">Application</span></span>|<span data-ttu-id="de7eb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de7eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de7eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de7eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="de7eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de7eb-120">Request headers</span></span>
|<span data-ttu-id="de7eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de7eb-121">Header</span></span>|<span data-ttu-id="de7eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="de7eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de7eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de7eb-123">Authorization</span></span>|<span data-ttu-id="de7eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de7eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de7eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de7eb-125">Accept</span></span>|<span data-ttu-id="de7eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de7eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de7eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de7eb-127">Request body</span></span>
<span data-ttu-id="de7eb-128">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="de7eb-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="de7eb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="de7eb-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="de7eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de7eb-130">Property</span></span>|<span data-ttu-id="de7eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="de7eb-131">Type</span></span>|<span data-ttu-id="de7eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="de7eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de7eb-133">id</span><span class="sxs-lookup"><span data-stu-id="de7eb-133">id</span></span>|<span data-ttu-id="de7eb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-134">String</span></span>|<span data-ttu-id="de7eb-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="de7eb-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="de7eb-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="de7eb-136">eventDateTime</span></span>|<span data-ttu-id="de7eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de7eb-137">DateTimeOffset</span></span>|<span data-ttu-id="de7eb-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="de7eb-138">Time when the event occurred .</span></span> <span data-ttu-id="de7eb-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="de7eb-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="de7eb-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="de7eb-140">correlationId</span></span>|<span data-ttu-id="de7eb-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-141">String</span></span>|<span data-ttu-id="de7eb-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="de7eb-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="de7eb-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="de7eb-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="de7eb-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="de7eb-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="de7eb-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-145">String</span></span>|<span data-ttu-id="de7eb-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="de7eb-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="de7eb-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="de7eb-147">operatingSystem</span></span>|<span data-ttu-id="de7eb-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-148">String</span></span>|<span data-ttu-id="de7eb-149">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="de7eb-149">Operating System.</span></span>|
|<span data-ttu-id="de7eb-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="de7eb-150">osVersion</span></span>|<span data-ttu-id="de7eb-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-151">String</span></span>|<span data-ttu-id="de7eb-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="de7eb-152">OS Version.</span></span>|
|<span data-ttu-id="de7eb-153">userId</span><span class="sxs-lookup"><span data-stu-id="de7eb-153">userId</span></span>|<span data-ttu-id="de7eb-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-154">String</span></span>|<span data-ttu-id="de7eb-155">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de7eb-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="de7eb-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="de7eb-156">deviceId</span></span>|<span data-ttu-id="de7eb-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-157">String</span></span>|<span data-ttu-id="de7eb-158">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de7eb-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="de7eb-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="de7eb-159">enrollmentType</span></span>|[<span data-ttu-id="de7eb-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="de7eb-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="de7eb-161">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="de7eb-161">Type of the enrollment.</span></span> <span data-ttu-id="de7eb-162">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="de7eb-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="de7eb-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="de7eb-163">failureCategory</span></span>|[<span data-ttu-id="de7eb-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="de7eb-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="de7eb-165">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="de7eb-165">Highlevel failure category.</span></span> <span data-ttu-id="de7eb-166">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="de7eb-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="de7eb-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="de7eb-167">failureReason</span></span>|<span data-ttu-id="de7eb-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de7eb-168">String</span></span>|<span data-ttu-id="de7eb-169">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="de7eb-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="de7eb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="de7eb-170">Response</span></span>
<span data-ttu-id="de7eb-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de7eb-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de7eb-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de7eb-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="de7eb-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de7eb-173">Request</span></span>
<span data-ttu-id="de7eb-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de7eb-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="de7eb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="de7eb-175">Response</span></span>
<span data-ttu-id="de7eb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de7eb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





