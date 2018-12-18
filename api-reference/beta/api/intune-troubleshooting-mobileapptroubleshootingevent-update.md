---
title: Atualizar mobileAppTroubleshootingEvent
description: Atualize as propriedades de um objeto mobileAppTroubleshootingEvent.
author: tfitzmac
ms.openlocfilehash: 58e5b67329fb044f19c6f216fbb25f60ada44e9d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333590"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="02d07-103">Atualizar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="02d07-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="02d07-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="02d07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02d07-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="02d07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02d07-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="02d07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02d07-107">Atualize as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="02d07-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02d07-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02d07-108">Prerequisites</span></span>
<span data-ttu-id="02d07-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d07-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02d07-111">Permission type</span></span>|<span data-ttu-id="02d07-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02d07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02d07-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02d07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02d07-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d07-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="02d07-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02d07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02d07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d07-116">Not supported.</span></span>|
|<span data-ttu-id="02d07-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02d07-117">Application</span></span>|<span data-ttu-id="02d07-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02d07-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02d07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="02d07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02d07-120">Request headers</span></span>
|<span data-ttu-id="02d07-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02d07-121">Header</span></span>|<span data-ttu-id="02d07-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02d07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02d07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02d07-123">Authorization</span></span>|<span data-ttu-id="02d07-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02d07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02d07-125">Accept</span></span>|<span data-ttu-id="02d07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02d07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02d07-127">Request body</span></span>
<span data-ttu-id="02d07-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="02d07-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="02d07-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="02d07-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="02d07-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d07-130">Property</span></span>|<span data-ttu-id="02d07-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d07-131">Type</span></span>|<span data-ttu-id="02d07-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02d07-133">id</span><span class="sxs-lookup"><span data-stu-id="02d07-133">id</span></span>|<span data-ttu-id="02d07-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d07-134">String</span></span>|<span data-ttu-id="02d07-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="02d07-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="02d07-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="02d07-136">eventDateTime</span></span>|<span data-ttu-id="02d07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d07-137">DateTimeOffset</span></span>|<span data-ttu-id="02d07-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="02d07-138">Time when the event occurred .</span></span> <span data-ttu-id="02d07-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="02d07-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="02d07-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="02d07-140">correlationId</span></span>|<span data-ttu-id="02d07-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d07-141">String</span></span>|<span data-ttu-id="02d07-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="02d07-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="02d07-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="02d07-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="02d07-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="02d07-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="02d07-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d07-145">String</span></span>|<span data-ttu-id="02d07-146">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="02d07-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="02d07-147">userId</span><span class="sxs-lookup"><span data-stu-id="02d07-147">userId</span></span>|<span data-ttu-id="02d07-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d07-148">String</span></span>|<span data-ttu-id="02d07-149">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02d07-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="02d07-150">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="02d07-150">applicationId</span></span>|<span data-ttu-id="02d07-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d07-151">String</span></span>|<span data-ttu-id="02d07-152">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="02d07-152">Intune application identifier.</span></span>|
|<span data-ttu-id="02d07-153">histórico</span><span class="sxs-lookup"><span data-stu-id="02d07-153">history</span></span>|<span data-ttu-id="02d07-154">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="02d07-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="02d07-155">Aplicativo móvel Intune Item do histórico de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="02d07-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="02d07-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d07-156">Response</span></span>
<span data-ttu-id="02d07-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02d07-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d07-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02d07-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="02d07-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02d07-159">Request</span></span>
<span data-ttu-id="02d07-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02d07-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02d07-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d07-161">Response</span></span>
<span data-ttu-id="02d07-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02d07-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





