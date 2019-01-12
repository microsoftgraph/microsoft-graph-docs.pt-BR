---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 496404d4a12080c9809d47f834e18e7cd5c793df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978344"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="2cd30-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2cd30-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="2cd30-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2cd30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cd30-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2cd30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cd30-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2cd30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cd30-107">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="2cd30-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cd30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cd30-108">Prerequisites</span></span>
<span data-ttu-id="2cd30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cd30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cd30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cd30-111">Permission type</span></span>|<span data-ttu-id="2cd30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2cd30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cd30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cd30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cd30-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cd30-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2cd30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cd30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cd30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cd30-116">Not supported.</span></span>|
|<span data-ttu-id="2cd30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cd30-117">Application</span></span>|<span data-ttu-id="2cd30-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cd30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cd30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cd30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="2cd30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cd30-120">Request headers</span></span>
|<span data-ttu-id="2cd30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cd30-121">Header</span></span>|<span data-ttu-id="2cd30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2cd30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cd30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cd30-123">Authorization</span></span>|<span data-ttu-id="2cd30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cd30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cd30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cd30-125">Accept</span></span>|<span data-ttu-id="2cd30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cd30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cd30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cd30-127">Request body</span></span>
<span data-ttu-id="2cd30-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="2cd30-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="2cd30-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="2cd30-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="2cd30-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cd30-130">Property</span></span>|<span data-ttu-id="2cd30-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cd30-131">Type</span></span>|<span data-ttu-id="2cd30-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cd30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd30-133">id</span><span class="sxs-lookup"><span data-stu-id="2cd30-133">id</span></span>|<span data-ttu-id="2cd30-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cd30-134">String</span></span>|<span data-ttu-id="2cd30-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2cd30-135">UUID for the object</span></span>|
|<span data-ttu-id="2cd30-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="2cd30-136">eventDateTime</span></span>|<span data-ttu-id="2cd30-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cd30-137">DateTimeOffset</span></span>|<span data-ttu-id="2cd30-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="2cd30-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="2cd30-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="2cd30-139">correlationId</span></span>|<span data-ttu-id="2cd30-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cd30-140">String</span></span>|<span data-ttu-id="2cd30-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="2cd30-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="2cd30-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cd30-142">Response</span></span>
<span data-ttu-id="2cd30-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cd30-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cd30-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cd30-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cd30-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cd30-145">Request</span></span>
<span data-ttu-id="2cd30-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cd30-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="2cd30-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cd30-147">Response</span></span>
<span data-ttu-id="2cd30-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cd30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





