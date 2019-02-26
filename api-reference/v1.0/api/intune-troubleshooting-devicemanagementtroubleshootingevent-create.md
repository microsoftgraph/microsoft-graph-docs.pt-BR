---
title: Criar deviceManagementTroubleshootingEvent
description: Criar um novo objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d222ddfa480072baefd943ca38ea8ade6d61641
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258447"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="11c99-103">Criar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="11c99-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="11c99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11c99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11c99-105">Criar um novo objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="11c99-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11c99-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11c99-106">Prerequisites</span></span>
<span data-ttu-id="11c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="11c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="11c99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c99-109">Permission type</span></span>|<span data-ttu-id="11c99-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11c99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11c99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11c99-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11c99-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="11c99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11c99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c99-114">Not supported.</span></span>|
|<span data-ttu-id="11c99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c99-115">Application</span></span>|<span data-ttu-id="11c99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11c99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11c99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="11c99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11c99-118">Request headers</span></span>
|<span data-ttu-id="11c99-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11c99-119">Header</span></span>|<span data-ttu-id="11c99-120">Valor</span><span class="sxs-lookup"><span data-stu-id="11c99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11c99-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11c99-121">Authorization</span></span>|<span data-ttu-id="11c99-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11c99-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11c99-123">Accept</span></span>|<span data-ttu-id="11c99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11c99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11c99-125">Request body</span></span>
<span data-ttu-id="11c99-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="11c99-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="11c99-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="11c99-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="11c99-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11c99-128">Property</span></span>|<span data-ttu-id="11c99-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c99-129">Type</span></span>|<span data-ttu-id="11c99-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c99-131">id</span><span class="sxs-lookup"><span data-stu-id="11c99-131">id</span></span>|<span data-ttu-id="11c99-132">String</span><span class="sxs-lookup"><span data-stu-id="11c99-132">String</span></span>|<span data-ttu-id="11c99-133">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="11c99-133">UUID for the object</span></span>|
|<span data-ttu-id="11c99-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="11c99-134">eventDateTime</span></span>|<span data-ttu-id="11c99-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c99-135">DateTimeOffset</span></span>|<span data-ttu-id="11c99-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="11c99-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="11c99-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="11c99-137">correlationId</span></span>|<span data-ttu-id="11c99-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11c99-138">String</span></span>|<span data-ttu-id="11c99-139">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="11c99-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="11c99-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c99-140">Response</span></span>
<span data-ttu-id="11c99-141">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11c99-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c99-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11c99-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="11c99-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c99-143">Request</span></span>
<span data-ttu-id="11c99-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11c99-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11c99-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c99-145">Response</span></span>
<span data-ttu-id="11c99-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11c99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



