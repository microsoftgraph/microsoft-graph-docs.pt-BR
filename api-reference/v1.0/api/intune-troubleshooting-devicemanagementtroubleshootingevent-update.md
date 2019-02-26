---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3219a86b2d7788217b26d640443807a4818c66a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251710"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="f0184-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f0184-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="f0184-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0184-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0184-105">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="f0184-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0184-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0184-106">Prerequisites</span></span>
<span data-ttu-id="f0184-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0184-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0184-109">Permission type</span></span>|<span data-ttu-id="f0184-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0184-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0184-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0184-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0184-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0184-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0184-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0184-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0184-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0184-114">Not supported.</span></span>|
|<span data-ttu-id="f0184-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0184-115">Application</span></span>|<span data-ttu-id="f0184-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0184-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0184-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0184-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="f0184-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0184-118">Request headers</span></span>
|<span data-ttu-id="f0184-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0184-119">Header</span></span>|<span data-ttu-id="f0184-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f0184-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0184-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0184-121">Authorization</span></span>|<span data-ttu-id="f0184-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0184-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0184-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0184-123">Accept</span></span>|<span data-ttu-id="f0184-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0184-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0184-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0184-125">Request body</span></span>
<span data-ttu-id="f0184-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="f0184-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="f0184-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="f0184-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="f0184-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0184-128">Property</span></span>|<span data-ttu-id="f0184-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0184-129">Type</span></span>|<span data-ttu-id="f0184-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0184-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0184-131">id</span><span class="sxs-lookup"><span data-stu-id="f0184-131">id</span></span>|<span data-ttu-id="f0184-132">String</span><span class="sxs-lookup"><span data-stu-id="f0184-132">String</span></span>|<span data-ttu-id="f0184-133">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0184-133">UUID for the object</span></span>|
|<span data-ttu-id="f0184-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f0184-134">eventDateTime</span></span>|<span data-ttu-id="f0184-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0184-135">DateTimeOffset</span></span>|<span data-ttu-id="f0184-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f0184-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="f0184-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="f0184-137">correlationId</span></span>|<span data-ttu-id="f0184-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0184-138">String</span></span>|<span data-ttu-id="f0184-139">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="f0184-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="f0184-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0184-140">Response</span></span>
<span data-ttu-id="f0184-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0184-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0184-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0184-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0184-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0184-143">Request</span></span>
<span data-ttu-id="f0184-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0184-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="f0184-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0184-145">Response</span></span>
<span data-ttu-id="f0184-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0184-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



