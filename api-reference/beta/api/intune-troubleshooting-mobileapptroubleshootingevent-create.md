---
title: Criar mobileAppTroubleshootingEvent
description: Crie um novo objeto de mobileAppTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59eea166285f55de32df2728f9bbc834e0eecac8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978141"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="16262-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="16262-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="16262-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16262-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16262-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16262-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16262-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16262-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16262-107">Crie um novo objeto de [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="16262-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16262-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16262-108">Prerequisites</span></span>
<span data-ttu-id="16262-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16262-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16262-111">Permission type</span></span>|<span data-ttu-id="16262-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16262-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16262-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16262-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16262-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16262-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="16262-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16262-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16262-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16262-116">Not supported.</span></span>|
|<span data-ttu-id="16262-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16262-117">Application</span></span>|<span data-ttu-id="16262-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16262-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16262-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16262-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="16262-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16262-120">Request headers</span></span>
|<span data-ttu-id="16262-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16262-121">Header</span></span>|<span data-ttu-id="16262-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16262-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16262-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16262-123">Authorization</span></span>|<span data-ttu-id="16262-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16262-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16262-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16262-125">Accept</span></span>|<span data-ttu-id="16262-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16262-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16262-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16262-127">Request body</span></span>
<span data-ttu-id="16262-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="16262-128">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="16262-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="16262-129">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="16262-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16262-130">Property</span></span>|<span data-ttu-id="16262-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16262-131">Type</span></span>|<span data-ttu-id="16262-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16262-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16262-133">id</span><span class="sxs-lookup"><span data-stu-id="16262-133">id</span></span>|<span data-ttu-id="16262-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16262-134">String</span></span>|<span data-ttu-id="16262-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="16262-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="16262-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="16262-136">eventDateTime</span></span>|<span data-ttu-id="16262-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16262-137">DateTimeOffset</span></span>|<span data-ttu-id="16262-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="16262-138">Time when the event occurred .</span></span> <span data-ttu-id="16262-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="16262-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="16262-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="16262-140">correlationId</span></span>|<span data-ttu-id="16262-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16262-141">String</span></span>|<span data-ttu-id="16262-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="16262-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="16262-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="16262-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="16262-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="16262-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="16262-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16262-145">String</span></span>|<span data-ttu-id="16262-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="16262-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="16262-147">userId</span><span class="sxs-lookup"><span data-stu-id="16262-147">userId</span></span>|<span data-ttu-id="16262-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16262-148">String</span></span>|<span data-ttu-id="16262-149">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16262-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="16262-150">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="16262-150">applicationId</span></span>|<span data-ttu-id="16262-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16262-151">String</span></span>|<span data-ttu-id="16262-152">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="16262-152">Intune application identifier.</span></span>|
|<span data-ttu-id="16262-153">histórico</span><span class="sxs-lookup"><span data-stu-id="16262-153">history</span></span>|<span data-ttu-id="16262-154">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="16262-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="16262-155">Aplicativo móvel Intune Item do histórico de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="16262-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="16262-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="16262-156">Response</span></span>
<span data-ttu-id="16262-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16262-157">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16262-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16262-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="16262-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16262-159">Request</span></span>
<span data-ttu-id="16262-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16262-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
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

### <a name="response"></a><span data-ttu-id="16262-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="16262-161">Response</span></span>
<span data-ttu-id="16262-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16262-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





