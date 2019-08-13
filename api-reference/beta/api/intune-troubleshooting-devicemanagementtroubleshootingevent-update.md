---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 942de87c14594cd4b8f08626fe69411543ad841d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350290"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b7c0a-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b7c0a-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b7c0a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7c0a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c0a-106">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7c0a-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7c0a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7c0a-107">Prerequisites</span></span>
<span data-ttu-id="b7c0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7c0a-110">Permission type</span></span>|<span data-ttu-id="b7c0a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7c0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7c0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7c0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7c0a-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="b7c0a-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="b7c0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7c0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-115">Not supported.</span></span>|
|<span data-ttu-id="b7c0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7c0a-116">Application</span></span>|<span data-ttu-id="b7c0a-117">\* \* TODO: Determine escopos ao apponly \* \*</span><span class="sxs-lookup"><span data-stu-id="b7c0a-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7c0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b7c0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7c0a-119">Request headers</span></span>
|<span data-ttu-id="b7c0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7c0a-120">Header</span></span>|<span data-ttu-id="b7c0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7c0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7c0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7c0a-122">Authorization</span></span>|<span data-ttu-id="b7c0a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7c0a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7c0a-124">Accept</span></span>|<span data-ttu-id="b7c0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7c0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7c0a-126">Request body</span></span>
<span data-ttu-id="b7c0a-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7c0a-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="b7c0a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7c0a-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="b7c0a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7c0a-129">Property</span></span>|<span data-ttu-id="b7c0a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7c0a-130">Type</span></span>|<span data-ttu-id="b7c0a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7c0a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c0a-132">id</span><span class="sxs-lookup"><span data-stu-id="b7c0a-132">id</span></span>|<span data-ttu-id="b7c0a-133">String</span><span class="sxs-lookup"><span data-stu-id="b7c0a-133">String</span></span>|<span data-ttu-id="b7c0a-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-134">UUID for the object</span></span>|
|<span data-ttu-id="b7c0a-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b7c0a-135">eventDateTime</span></span>|<span data-ttu-id="b7c0a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7c0a-136">DateTimeOffset</span></span>|<span data-ttu-id="b7c0a-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="b7c0a-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="b7c0a-138">correlationId</span></span>|<span data-ttu-id="b7c0a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7c0a-139">String</span></span>|<span data-ttu-id="b7c0a-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="b7c0a-141">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b7c0a-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b7c0a-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b7c0a-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b7c0a-143">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="b7c0a-144">EventName</span><span class="sxs-lookup"><span data-stu-id="b7c0a-144">eventName</span></span>|<span data-ttu-id="b7c0a-145">String</span><span class="sxs-lookup"><span data-stu-id="b7c0a-145">String</span></span>|<span data-ttu-id="b7c0a-146">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="b7c0a-147">É um campo opcional</span><span class="sxs-lookup"><span data-stu-id="b7c0a-147">It is an Optional field</span></span>|
|<span data-ttu-id="b7c0a-148">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="b7c0a-148">additionalInformation</span></span>|<span data-ttu-id="b7c0a-149">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b7c0a-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b7c0a-150">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b7c0a-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="b7c0a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7c0a-151">Response</span></span>
<span data-ttu-id="b7c0a-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c0a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7c0a-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7c0a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7c0a-154">Request</span></span>
<span data-ttu-id="b7c0a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b7c0a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7c0a-156">Response</span></span>
<span data-ttu-id="b7c0a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7c0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```






