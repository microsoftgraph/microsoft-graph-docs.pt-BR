---
title: Atualizar appleVppTokenTroubleshootingEvent
description: Atualiza as propriedades de um objeto appleVppTokenTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ce92f73e3aaa8b9f7a1442e3088c221266ff299
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986534"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="0c1bb-103">Atualizar appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="0c1bb-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="0c1bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c1bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c1bb-106">Atualiza as propriedades de um objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0c1bb-106">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c1bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c1bb-107">Prerequisites</span></span>
<span data-ttu-id="0c1bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c1bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c1bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c1bb-110">Permission type</span></span>|<span data-ttu-id="0c1bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c1bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c1bb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c1bb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c1bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c1bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-115">Not supported.</span></span>|
|<span data-ttu-id="0c1bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c1bb-116">Application</span></span>|<span data-ttu-id="0c1bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c1bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c1bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="0c1bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1bb-119">Request headers</span></span>
|<span data-ttu-id="0c1bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c1bb-120">Header</span></span>|<span data-ttu-id="0c1bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c1bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c1bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c1bb-122">Authorization</span></span>|<span data-ttu-id="0c1bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c1bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c1bb-124">Accept</span></span>|<span data-ttu-id="0c1bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c1bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c1bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1bb-126">Request body</span></span>
<span data-ttu-id="0c1bb-127">No corpo da solicitação, forneça uma representação JSON do objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0c1bb-127">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="0c1bb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="0c1bb-128">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="0c1bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c1bb-129">Property</span></span>|<span data-ttu-id="0c1bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c1bb-130">Type</span></span>|<span data-ttu-id="0c1bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c1bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c1bb-132">id</span><span class="sxs-lookup"><span data-stu-id="0c1bb-132">id</span></span>|<span data-ttu-id="0c1bb-133">String</span><span class="sxs-lookup"><span data-stu-id="0c1bb-133">String</span></span>|<span data-ttu-id="0c1bb-134">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0c1bb-135">eventDateTime</span></span>|<span data-ttu-id="0c1bb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c1bb-136">DateTimeOffset</span></span>|<span data-ttu-id="0c1bb-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-137">Time when the event occurred .</span></span> <span data-ttu-id="0c1bb-138">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="0c1bb-139">correlationId</span></span>|<span data-ttu-id="0c1bb-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c1bb-140">String</span></span>|<span data-ttu-id="0c1bb-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="0c1bb-142">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0c1bb-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="0c1bb-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0c1bb-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="0c1bb-145">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="0c1bb-146">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-147">EventName</span><span class="sxs-lookup"><span data-stu-id="0c1bb-147">eventName</span></span>|<span data-ttu-id="0c1bb-148">String</span><span class="sxs-lookup"><span data-stu-id="0c1bb-148">String</span></span>|<span data-ttu-id="0c1bb-149">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="0c1bb-150">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="0c1bb-151">additionalInformation</span></span>|<span data-ttu-id="0c1bb-152">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0c1bb-153">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0c1bb-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0c1bb-154">tokenid</span><span class="sxs-lookup"><span data-stu-id="0c1bb-154">tokenId</span></span>|<span data-ttu-id="0c1bb-155">String</span><span class="sxs-lookup"><span data-stu-id="0c1bb-155">String</span></span>|<span data-ttu-id="0c1bb-156">Identificador de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="0c1bb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c1bb-157">Response</span></span>
<span data-ttu-id="0c1bb-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-158">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c1bb-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c1bb-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c1bb-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1bb-160">Request</span></span>
<span data-ttu-id="0c1bb-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="0c1bb-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c1bb-162">Response</span></span>
<span data-ttu-id="0c1bb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c1bb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
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
  ],
  "tokenId": "Token Id value"
}
```




