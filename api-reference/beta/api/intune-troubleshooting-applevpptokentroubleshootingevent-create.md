---
title: Criar appleVppTokenTroubleshootingEvent
description: Criar um novo objeto appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a993f13b168d080719aaba07b3112b0ea9b0dff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457468"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="97d2e-103">Criar appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="97d2e-103">Create appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="97d2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97d2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d2e-107">Criar um novo objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="97d2e-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97d2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97d2e-108">Prerequisites</span></span>
<span data-ttu-id="97d2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97d2e-111">Permission type</span></span>|<span data-ttu-id="97d2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97d2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97d2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97d2e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d2e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="97d2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97d2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d2e-116">Not supported.</span></span>|
|<span data-ttu-id="97d2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97d2e-117">Application</span></span>|<span data-ttu-id="97d2e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d2e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97d2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="97d2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97d2e-120">Request headers</span></span>
|<span data-ttu-id="97d2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97d2e-121">Header</span></span>|<span data-ttu-id="97d2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97d2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97d2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97d2e-123">Authorization</span></span>|<span data-ttu-id="97d2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97d2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97d2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97d2e-125">Accept</span></span>|<span data-ttu-id="97d2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97d2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97d2e-127">Request body</span></span>
<span data-ttu-id="97d2e-128">No corpo da solicitação, forneça uma representação JSON do objeto appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="97d2e-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="97d2e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="97d2e-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="97d2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97d2e-130">Property</span></span>|<span data-ttu-id="97d2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97d2e-131">Type</span></span>|<span data-ttu-id="97d2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d2e-133">id</span><span class="sxs-lookup"><span data-stu-id="97d2e-133">id</span></span>|<span data-ttu-id="97d2e-134">String</span><span class="sxs-lookup"><span data-stu-id="97d2e-134">String</span></span>|<span data-ttu-id="97d2e-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="97d2e-136">eventDateTime</span></span>|<span data-ttu-id="97d2e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d2e-137">DateTimeOffset</span></span>|<span data-ttu-id="97d2e-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="97d2e-138">Time when the event occurred .</span></span> <span data-ttu-id="97d2e-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="97d2e-140">correlationId</span></span>|<span data-ttu-id="97d2e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97d2e-141">String</span></span>|<span data-ttu-id="97d2e-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="97d2e-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="97d2e-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="97d2e-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="97d2e-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="97d2e-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="97d2e-146">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="97d2e-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="97d2e-147">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-148">EventName</span><span class="sxs-lookup"><span data-stu-id="97d2e-148">eventName</span></span>|<span data-ttu-id="97d2e-149">String</span><span class="sxs-lookup"><span data-stu-id="97d2e-149">String</span></span>|<span data-ttu-id="97d2e-150">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="97d2e-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="97d2e-151">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="97d2e-152">additionalInformation</span></span>|<span data-ttu-id="97d2e-153">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="97d2e-154">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="97d2e-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="97d2e-155">tokenid</span><span class="sxs-lookup"><span data-stu-id="97d2e-155">tokenId</span></span>|<span data-ttu-id="97d2e-156">String</span><span class="sxs-lookup"><span data-stu-id="97d2e-156">String</span></span>|<span data-ttu-id="97d2e-157">Identificador de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="97d2e-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="97d2e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d2e-158">Response</span></span>
<span data-ttu-id="97d2e-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d2e-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d2e-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97d2e-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d2e-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97d2e-161">Request</span></span>
<span data-ttu-id="97d2e-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97d2e-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="97d2e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d2e-163">Response</span></span>
<span data-ttu-id="97d2e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97d2e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



