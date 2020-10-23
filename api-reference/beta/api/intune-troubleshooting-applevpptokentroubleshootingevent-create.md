---
title: Criar appleVppTokenTroubleshootingEvent
description: Criar um novo objeto appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29f84ba4727f8bd5dce33a999f47fc29f620b079
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692776"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="bdacb-103">Criar appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bdacb-103">Create appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="bdacb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdacb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdacb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bdacb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdacb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdacb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdacb-107">Criar um novo objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="bdacb-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdacb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bdacb-108">Prerequisites</span></span>
<span data-ttu-id="bdacb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdacb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdacb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdacb-111">Permission type</span></span>|<span data-ttu-id="bdacb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bdacb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdacb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdacb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdacb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdacb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bdacb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdacb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdacb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdacb-116">Not supported.</span></span>|
|<span data-ttu-id="bdacb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdacb-117">Application</span></span>|<span data-ttu-id="bdacb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdacb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdacb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdacb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="bdacb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdacb-120">Request headers</span></span>
|<span data-ttu-id="bdacb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdacb-121">Header</span></span>|<span data-ttu-id="bdacb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bdacb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdacb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdacb-123">Authorization</span></span>|<span data-ttu-id="bdacb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdacb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdacb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bdacb-125">Accept</span></span>|<span data-ttu-id="bdacb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdacb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdacb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdacb-127">Request body</span></span>
<span data-ttu-id="bdacb-128">No corpo da solicitação, forneça uma representação JSON do objeto appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="bdacb-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="bdacb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="bdacb-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="bdacb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdacb-130">Property</span></span>|<span data-ttu-id="bdacb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdacb-131">Type</span></span>|<span data-ttu-id="bdacb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdacb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdacb-133">id</span><span class="sxs-lookup"><span data-stu-id="bdacb-133">id</span></span>|<span data-ttu-id="bdacb-134">String</span><span class="sxs-lookup"><span data-stu-id="bdacb-134">String</span></span>|<span data-ttu-id="bdacb-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bdacb-136">eventDateTime</span></span>|<span data-ttu-id="bdacb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdacb-137">DateTimeOffset</span></span>|<span data-ttu-id="bdacb-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="bdacb-138">Time when the event occurred .</span></span> <span data-ttu-id="bdacb-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="bdacb-140">correlationId</span></span>|<span data-ttu-id="bdacb-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdacb-141">String</span></span>|<span data-ttu-id="bdacb-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="bdacb-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="bdacb-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bdacb-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="bdacb-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bdacb-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="bdacb-146">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="bdacb-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="bdacb-147">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-148">EventName</span><span class="sxs-lookup"><span data-stu-id="bdacb-148">eventName</span></span>|<span data-ttu-id="bdacb-149">String</span><span class="sxs-lookup"><span data-stu-id="bdacb-149">String</span></span>|<span data-ttu-id="bdacb-150">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="bdacb-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="bdacb-151">É um campo opcional herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="bdacb-152">additionalInformation</span></span>|<span data-ttu-id="bdacb-153">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bdacb-154">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bdacb-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bdacb-155">tokenid</span><span class="sxs-lookup"><span data-stu-id="bdacb-155">tokenId</span></span>|<span data-ttu-id="bdacb-156">String</span><span class="sxs-lookup"><span data-stu-id="bdacb-156">String</span></span>|<span data-ttu-id="bdacb-157">Identificador de token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="bdacb-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="bdacb-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdacb-158">Response</span></span>
<span data-ttu-id="bdacb-159">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdacb-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdacb-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdacb-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdacb-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdacb-161">Request</span></span>
<span data-ttu-id="bdacb-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdacb-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bdacb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdacb-163">Response</span></span>
<span data-ttu-id="bdacb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdacb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





