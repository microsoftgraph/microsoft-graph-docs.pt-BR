---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 516233827c6d4a03b15ccb8a498df189464c6f9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884676"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="ff642-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ff642-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="ff642-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ff642-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff642-105">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ff642-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff642-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff642-106">Prerequisites</span></span>
<span data-ttu-id="ff642-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff642-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff642-109">Permission type</span></span>|<span data-ttu-id="ff642-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff642-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff642-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff642-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff642-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff642-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff642-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff642-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff642-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff642-114">Not supported.</span></span>|
|<span data-ttu-id="ff642-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff642-115">Application</span></span>|<span data-ttu-id="ff642-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff642-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff642-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff642-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="ff642-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff642-118">Request headers</span></span>
|<span data-ttu-id="ff642-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff642-119">Header</span></span>|<span data-ttu-id="ff642-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ff642-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff642-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff642-121">Authorization</span></span>|<span data-ttu-id="ff642-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff642-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff642-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff642-123">Accept</span></span>|<span data-ttu-id="ff642-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff642-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff642-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff642-125">Request body</span></span>
<span data-ttu-id="ff642-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ff642-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="ff642-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ff642-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="ff642-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff642-128">Property</span></span>|<span data-ttu-id="ff642-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff642-129">Type</span></span>|<span data-ttu-id="ff642-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff642-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff642-131">id</span><span class="sxs-lookup"><span data-stu-id="ff642-131">id</span></span>|<span data-ttu-id="ff642-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff642-132">String</span></span>|<span data-ttu-id="ff642-133">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ff642-133">UUID for the object</span></span>|
|<span data-ttu-id="ff642-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ff642-134">eventDateTime</span></span>|<span data-ttu-id="ff642-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff642-135">DateTimeOffset</span></span>|<span data-ttu-id="ff642-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ff642-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="ff642-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="ff642-137">correlationId</span></span>|<span data-ttu-id="ff642-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff642-138">String</span></span>|<span data-ttu-id="ff642-139">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="ff642-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="ff642-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff642-140">Response</span></span>
<span data-ttu-id="ff642-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff642-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff642-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff642-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff642-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff642-143">Request</span></span>
<span data-ttu-id="ff642-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff642-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="ff642-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff642-145">Response</span></span>
<span data-ttu-id="ff642-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff642-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



