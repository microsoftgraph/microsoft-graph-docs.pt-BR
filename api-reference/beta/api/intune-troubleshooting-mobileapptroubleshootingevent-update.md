---
title: Atualizar mobileAppTroubleshootingEvent
description: Atualize as propriedades de um objeto mobileAppTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1dee1ecb19f58412acbdcf529991f2491e0deabb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862802"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="c763b-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c763b-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="c763b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c763b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c763b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c763b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c763b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c763b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c763b-107">Atualize as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c763b-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c763b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c763b-108">Prerequisites</span></span>
<span data-ttu-id="c763b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c763b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c763b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c763b-111">Permission type</span></span>|<span data-ttu-id="c763b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c763b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c763b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c763b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c763b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c763b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c763b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c763b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c763b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c763b-116">Not supported.</span></span>|
|<span data-ttu-id="c763b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c763b-117">Application</span></span>|<span data-ttu-id="c763b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c763b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c763b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c763b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c763b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c763b-120">Request headers</span></span>
|<span data-ttu-id="c763b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c763b-121">Header</span></span>|<span data-ttu-id="c763b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c763b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c763b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c763b-123">Authorization</span></span>|<span data-ttu-id="c763b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c763b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c763b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c763b-125">Accept</span></span>|<span data-ttu-id="c763b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c763b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c763b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c763b-127">Request body</span></span>
<span data-ttu-id="c763b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c763b-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c763b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c763b-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="c763b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c763b-130">Property</span></span>|<span data-ttu-id="c763b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c763b-131">Type</span></span>|<span data-ttu-id="c763b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c763b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c763b-133">id</span><span class="sxs-lookup"><span data-stu-id="c763b-133">id</span></span>|<span data-ttu-id="c763b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c763b-134">String</span></span>|<span data-ttu-id="c763b-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c763b-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c763b-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c763b-136">eventDateTime</span></span>|<span data-ttu-id="c763b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c763b-137">DateTimeOffset</span></span>|<span data-ttu-id="c763b-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c763b-138">Time when the event occurred .</span></span> <span data-ttu-id="c763b-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c763b-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c763b-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="c763b-140">correlationId</span></span>|<span data-ttu-id="c763b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c763b-141">String</span></span>|<span data-ttu-id="c763b-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="c763b-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c763b-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c763b-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c763b-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c763b-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="c763b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c763b-145">String</span></span>|<span data-ttu-id="c763b-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="c763b-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c763b-147">userId</span><span class="sxs-lookup"><span data-stu-id="c763b-147">userId</span></span>|<span data-ttu-id="c763b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c763b-148">String</span></span>|<span data-ttu-id="c763b-149">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c763b-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c763b-150">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c763b-150">applicationId</span></span>|<span data-ttu-id="c763b-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c763b-151">String</span></span>|<span data-ttu-id="c763b-152">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="c763b-152">Intune application identifier.</span></span>|
|<span data-ttu-id="c763b-153">histórico</span><span class="sxs-lookup"><span data-stu-id="c763b-153">history</span></span>|<span data-ttu-id="c763b-154">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c763b-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="c763b-155">Aplicativo móvel Intune Item do histórico de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="c763b-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="c763b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c763b-156">Response</span></span>
<span data-ttu-id="c763b-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c763b-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c763b-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c763b-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="c763b-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c763b-159">Request</span></span>
<span data-ttu-id="c763b-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c763b-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 421

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c763b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c763b-161">Response</span></span>
<span data-ttu-id="c763b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c763b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 538

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```





