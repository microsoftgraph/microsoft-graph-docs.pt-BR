---
title: Criar deviceManagementTroubleshootingEvent
description: Criar um novo objeto deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdc73c027bdaf8cefabc738620331c8102a63830
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732286"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="20b65-103">Criar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="20b65-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="20b65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20b65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20b65-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20b65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b65-106">Criar um novo objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="20b65-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20b65-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20b65-107">Prerequisites</span></span>
<span data-ttu-id="20b65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20b65-110">Permission type</span></span>|<span data-ttu-id="20b65-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20b65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20b65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20b65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20b65-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20b65-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20b65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20b65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20b65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20b65-115">Not supported.</span></span>|
|<span data-ttu-id="20b65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20b65-116">Application</span></span>|<span data-ttu-id="20b65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20b65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20b65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20b65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="20b65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20b65-119">Request headers</span></span>
|<span data-ttu-id="20b65-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20b65-120">Header</span></span>|<span data-ttu-id="20b65-121">Valor</span><span class="sxs-lookup"><span data-stu-id="20b65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20b65-122">Authorization</span></span>|<span data-ttu-id="20b65-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b65-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20b65-124">Accept</span></span>|<span data-ttu-id="20b65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20b65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b65-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20b65-126">Request body</span></span>
<span data-ttu-id="20b65-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="20b65-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="20b65-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="20b65-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="20b65-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20b65-129">Property</span></span>|<span data-ttu-id="20b65-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20b65-130">Type</span></span>|<span data-ttu-id="20b65-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b65-132">id</span><span class="sxs-lookup"><span data-stu-id="20b65-132">id</span></span>|<span data-ttu-id="20b65-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b65-133">String</span></span>|<span data-ttu-id="20b65-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="20b65-134">UUID for the object</span></span>|
|<span data-ttu-id="20b65-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="20b65-135">eventDateTime</span></span>|<span data-ttu-id="20b65-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b65-136">DateTimeOffset</span></span>|<span data-ttu-id="20b65-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="20b65-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="20b65-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="20b65-138">correlationId</span></span>|<span data-ttu-id="20b65-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b65-139">String</span></span>|<span data-ttu-id="20b65-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="20b65-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="20b65-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="20b65-141">Response</span></span>
<span data-ttu-id="20b65-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20b65-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b65-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20b65-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="20b65-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20b65-144">Request</span></span>
<span data-ttu-id="20b65-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20b65-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20b65-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="20b65-146">Response</span></span>
<span data-ttu-id="20b65-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20b65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









