---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9768948b542a08901dcf43f728f90ab3c70535b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089102"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="bb804-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bb804-103">Update deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="bb804-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb804-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb804-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb804-106">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="bb804-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb804-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb804-107">Prerequisites</span></span>
<span data-ttu-id="bb804-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb804-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb804-110">Permission type</span></span>|<span data-ttu-id="bb804-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb804-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb804-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb804-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb804-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb804-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb804-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb804-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb804-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb804-115">Not supported.</span></span>|
|<span data-ttu-id="bb804-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb804-116">Application</span></span>|<span data-ttu-id="bb804-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb804-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb804-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb804-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="bb804-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb804-119">Request headers</span></span>
|<span data-ttu-id="bb804-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb804-120">Header</span></span>|<span data-ttu-id="bb804-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb804-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb804-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb804-122">Authorization</span></span>|<span data-ttu-id="bb804-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb804-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb804-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb804-124">Accept</span></span>|<span data-ttu-id="bb804-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb804-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb804-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb804-126">Request body</span></span>
<span data-ttu-id="bb804-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="bb804-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="bb804-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="bb804-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="bb804-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb804-129">Property</span></span>|<span data-ttu-id="bb804-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb804-130">Type</span></span>|<span data-ttu-id="bb804-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb804-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb804-132">id</span><span class="sxs-lookup"><span data-stu-id="bb804-132">id</span></span>|<span data-ttu-id="bb804-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb804-133">String</span></span>|<span data-ttu-id="bb804-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb804-134">UUID for the object</span></span>|
|<span data-ttu-id="bb804-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bb804-135">eventDateTime</span></span>|<span data-ttu-id="bb804-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb804-136">DateTimeOffset</span></span>|<span data-ttu-id="bb804-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="bb804-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="bb804-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="bb804-138">correlationId</span></span>|<span data-ttu-id="bb804-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb804-139">String</span></span>|<span data-ttu-id="bb804-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="bb804-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="bb804-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb804-141">Response</span></span>
<span data-ttu-id="bb804-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb804-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb804-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb804-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb804-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb804-144">Request</span></span>
<span data-ttu-id="bb804-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb804-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb804-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb804-146">Response</span></span>
<span data-ttu-id="bb804-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb804-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









