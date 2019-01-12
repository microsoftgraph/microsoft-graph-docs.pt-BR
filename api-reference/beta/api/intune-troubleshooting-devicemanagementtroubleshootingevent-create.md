---
title: Criar deviceManagementTroubleshootingEvent
description: Criar um novo objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 108827de4760ad8573d34dccba8403cc34d40a63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934167"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="8071b-103">Criar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8071b-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="8071b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8071b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8071b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8071b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8071b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8071b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8071b-107">Criar um novo objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8071b-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8071b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8071b-108">Prerequisites</span></span>
<span data-ttu-id="8071b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8071b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8071b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8071b-111">Permission type</span></span>|<span data-ttu-id="8071b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8071b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8071b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8071b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8071b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8071b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8071b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8071b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8071b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8071b-116">Not supported.</span></span>|
|<span data-ttu-id="8071b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8071b-117">Application</span></span>|<span data-ttu-id="8071b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8071b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8071b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8071b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8071b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8071b-120">Request headers</span></span>
|<span data-ttu-id="8071b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8071b-121">Header</span></span>|<span data-ttu-id="8071b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8071b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8071b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8071b-123">Authorization</span></span>|<span data-ttu-id="8071b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8071b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8071b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8071b-125">Accept</span></span>|<span data-ttu-id="8071b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8071b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8071b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8071b-127">Request body</span></span>
<span data-ttu-id="8071b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="8071b-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="8071b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="8071b-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="8071b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8071b-130">Property</span></span>|<span data-ttu-id="8071b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8071b-131">Type</span></span>|<span data-ttu-id="8071b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8071b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8071b-133">id</span><span class="sxs-lookup"><span data-stu-id="8071b-133">id</span></span>|<span data-ttu-id="8071b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8071b-134">String</span></span>|<span data-ttu-id="8071b-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="8071b-135">UUID for the object</span></span>|
|<span data-ttu-id="8071b-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8071b-136">eventDateTime</span></span>|<span data-ttu-id="8071b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8071b-137">DateTimeOffset</span></span>|<span data-ttu-id="8071b-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="8071b-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="8071b-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="8071b-139">correlationId</span></span>|<span data-ttu-id="8071b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8071b-140">String</span></span>|<span data-ttu-id="8071b-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="8071b-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="8071b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8071b-142">Response</span></span>
<span data-ttu-id="8071b-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8071b-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8071b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8071b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="8071b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8071b-145">Request</span></span>
<span data-ttu-id="8071b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8071b-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="8071b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8071b-147">Response</span></span>
<span data-ttu-id="8071b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8071b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





