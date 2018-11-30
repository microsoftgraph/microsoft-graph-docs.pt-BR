---
title: Criar deviceManagementTroubleshootingEvent
description: Criar um novo objeto deviceManagementTroubleshootingEvent.
ms.openlocfilehash: d1fef87009c0797511adef5204cbc5ab4d99c291
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039145"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="1e1e8-103">Criar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="1e1e8-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="1e1e8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e1e8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e1e8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e1e8-107">Criar um novo objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="1e1e8-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e1e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e1e8-108">Prerequisites</span></span>
<span data-ttu-id="1e1e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e1e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e1e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e1e8-111">Permission type</span></span>|<span data-ttu-id="1e1e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e1e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e1e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e1e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e1e8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e1e8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1e1e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e1e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e1e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-116">Not supported.</span></span>|
|<span data-ttu-id="1e1e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e1e8-117">Application</span></span>|<span data-ttu-id="1e1e8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e1e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e1e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="1e1e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e1e8-120">Request headers</span></span>
|<span data-ttu-id="1e1e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e1e8-121">Header</span></span>|<span data-ttu-id="1e1e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e1e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e1e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e1e8-123">Authorization</span></span>|<span data-ttu-id="1e1e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e1e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e1e8-125">Accept</span></span>|<span data-ttu-id="1e1e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e1e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e1e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e1e8-127">Request body</span></span>
<span data-ttu-id="1e1e8-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="1e1e8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="1e1e8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e1e8-130">Property</span></span>|<span data-ttu-id="1e1e8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e1e8-131">Type</span></span>|<span data-ttu-id="1e1e8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e1e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e1e8-133">id</span><span class="sxs-lookup"><span data-stu-id="1e1e8-133">id</span></span>|<span data-ttu-id="1e1e8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e1e8-134">String</span></span>|<span data-ttu-id="1e1e8-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-135">UUID for the object</span></span>|
|<span data-ttu-id="1e1e8-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="1e1e8-136">eventDateTime</span></span>|<span data-ttu-id="1e1e8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e1e8-137">DateTimeOffset</span></span>|<span data-ttu-id="1e1e8-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="1e1e8-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="1e1e8-139">correlationId</span></span>|<span data-ttu-id="1e1e8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e1e8-140">String</span></span>|<span data-ttu-id="1e1e8-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="1e1e8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1e8-142">Response</span></span>
<span data-ttu-id="1e1e8-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e1e8-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e1e8-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e1e8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e1e8-145">Request</span></span>
<span data-ttu-id="1e1e8-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e1e8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e1e8-147">Response</span></span>
<span data-ttu-id="1e1e8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e1e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





