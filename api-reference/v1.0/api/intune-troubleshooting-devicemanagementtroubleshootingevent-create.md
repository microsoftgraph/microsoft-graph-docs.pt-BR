---
title: Criar deviceManagementTroubleshootingEvent
description: Criar um novo objeto deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf2c339f69897b44512dc7317441aacf44f851d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511898"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="5d34e-103">Criar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="5d34e-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="5d34e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d34e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d34e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d34e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d34e-106">Criar um novo objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5d34e-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d34e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d34e-107">Prerequisites</span></span>
<span data-ttu-id="5d34e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d34e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d34e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d34e-110">Permission type</span></span>|<span data-ttu-id="5d34e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d34e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d34e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d34e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d34e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d34e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5d34e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d34e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d34e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d34e-115">Not supported.</span></span>|
|<span data-ttu-id="5d34e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d34e-116">Application</span></span>|<span data-ttu-id="5d34e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d34e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d34e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d34e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="5d34e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d34e-119">Request headers</span></span>
|<span data-ttu-id="5d34e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d34e-120">Header</span></span>|<span data-ttu-id="5d34e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5d34e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d34e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d34e-122">Authorization</span></span>|<span data-ttu-id="5d34e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d34e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d34e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d34e-124">Accept</span></span>|<span data-ttu-id="5d34e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d34e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d34e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d34e-126">Request body</span></span>
<span data-ttu-id="5d34e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="5d34e-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="5d34e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="5d34e-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="5d34e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d34e-129">Property</span></span>|<span data-ttu-id="5d34e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d34e-130">Type</span></span>|<span data-ttu-id="5d34e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d34e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d34e-132">id</span><span class="sxs-lookup"><span data-stu-id="5d34e-132">id</span></span>|<span data-ttu-id="5d34e-133">String</span><span class="sxs-lookup"><span data-stu-id="5d34e-133">String</span></span>|<span data-ttu-id="5d34e-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="5d34e-134">UUID for the object</span></span>|
|<span data-ttu-id="5d34e-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5d34e-135">eventDateTime</span></span>|<span data-ttu-id="5d34e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d34e-136">DateTimeOffset</span></span>|<span data-ttu-id="5d34e-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="5d34e-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="5d34e-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="5d34e-138">correlationId</span></span>|<span data-ttu-id="5d34e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d34e-139">String</span></span>|<span data-ttu-id="5d34e-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="5d34e-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="5d34e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d34e-141">Response</span></span>
<span data-ttu-id="5d34e-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d34e-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d34e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d34e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d34e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d34e-144">Request</span></span>
<span data-ttu-id="5d34e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d34e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="5d34e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d34e-146">Response</span></span>
<span data-ttu-id="5d34e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d34e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```




