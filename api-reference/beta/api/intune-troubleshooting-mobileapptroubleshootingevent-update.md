---
title: Atualizar mobileAppTroubleshootingEvent
description: Atualize as propriedades de um objeto mobileAppTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec0c30cc2c37e65fa0a6adebf0bd3a171530640d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940068"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="e79d7-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e79d7-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="e79d7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e79d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e79d7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e79d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e79d7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e79d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e79d7-107">Atualize as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e79d7-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e79d7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e79d7-108">Prerequisites</span></span>
<span data-ttu-id="e79d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e79d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e79d7-111">Permission type</span></span>|<span data-ttu-id="e79d7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e79d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e79d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e79d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e79d7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79d7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e79d7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e79d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e79d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79d7-116">Not supported.</span></span>|
|<span data-ttu-id="e79d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e79d7-117">Application</span></span>|<span data-ttu-id="e79d7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e79d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e79d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e79d7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d7-120">Request headers</span></span>
|<span data-ttu-id="e79d7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e79d7-121">Header</span></span>|<span data-ttu-id="e79d7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e79d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e79d7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e79d7-123">Authorization</span></span>|<span data-ttu-id="e79d7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e79d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e79d7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e79d7-125">Accept</span></span>|<span data-ttu-id="e79d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e79d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d7-127">Request body</span></span>
<span data-ttu-id="e79d7-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e79d7-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e79d7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e79d7-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="e79d7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e79d7-130">Property</span></span>|<span data-ttu-id="e79d7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e79d7-131">Type</span></span>|<span data-ttu-id="e79d7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e79d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79d7-133">id</span><span class="sxs-lookup"><span data-stu-id="e79d7-133">id</span></span>|<span data-ttu-id="e79d7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79d7-134">String</span></span>|<span data-ttu-id="e79d7-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e79d7-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e79d7-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e79d7-136">eventDateTime</span></span>|<span data-ttu-id="e79d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79d7-137">DateTimeOffset</span></span>|<span data-ttu-id="e79d7-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e79d7-138">Time when the event occurred .</span></span> <span data-ttu-id="e79d7-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e79d7-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e79d7-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="e79d7-140">correlationId</span></span>|<span data-ttu-id="e79d7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79d7-141">String</span></span>|<span data-ttu-id="e79d7-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="e79d7-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e79d7-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e79d7-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e79d7-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e79d7-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="e79d7-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79d7-145">String</span></span>|<span data-ttu-id="e79d7-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="e79d7-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e79d7-147">userId</span><span class="sxs-lookup"><span data-stu-id="e79d7-147">userId</span></span>|<span data-ttu-id="e79d7-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79d7-148">String</span></span>|<span data-ttu-id="e79d7-149">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e79d7-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e79d7-150">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="e79d7-150">applicationId</span></span>|<span data-ttu-id="e79d7-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79d7-151">String</span></span>|<span data-ttu-id="e79d7-152">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="e79d7-152">Intune application identifier.</span></span>|
|<span data-ttu-id="e79d7-153">histórico</span><span class="sxs-lookup"><span data-stu-id="e79d7-153">history</span></span>|<span data-ttu-id="e79d7-154">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e79d7-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="e79d7-155">Aplicativo móvel Intune Item do histórico de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e79d7-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="e79d7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79d7-156">Response</span></span>
<span data-ttu-id="e79d7-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e79d7-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79d7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e79d7-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="e79d7-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d7-159">Request</span></span>
<span data-ttu-id="e79d7-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e79d7-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e79d7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79d7-161">Response</span></span>
<span data-ttu-id="e79d7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e79d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





