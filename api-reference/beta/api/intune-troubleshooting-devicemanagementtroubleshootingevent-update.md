---
title: Atualizar deviceManagementTroubleshootingEvent
description: Atualizar as propriedades de um objeto deviceManagementTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 935a5b835669a2d87fd761d8c62ccba537022f91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415394"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="5bb90-103">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="5bb90-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="5bb90-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5bb90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5bb90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5bb90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bb90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5bb90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb90-107">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5bb90-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bb90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5bb90-108">Prerequisites</span></span>
<span data-ttu-id="5bb90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5bb90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5bb90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bb90-111">Permission type</span></span>|<span data-ttu-id="5bb90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5bb90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bb90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb90-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb90-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bb90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb90-116">Not supported.</span></span>|
|<span data-ttu-id="5bb90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bb90-117">Application</span></span>|<span data-ttu-id="5bb90-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb90-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="5bb90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb90-120">Request headers</span></span>
|<span data-ttu-id="5bb90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bb90-121">Header</span></span>|<span data-ttu-id="5bb90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5bb90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bb90-123">Authorization</span></span>|<span data-ttu-id="5bb90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bb90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5bb90-125">Accept</span></span>|<span data-ttu-id="5bb90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb90-127">Request body</span></span>
<span data-ttu-id="5bb90-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5bb90-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="5bb90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5bb90-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="5bb90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb90-130">Property</span></span>|<span data-ttu-id="5bb90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb90-131">Type</span></span>|<span data-ttu-id="5bb90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb90-133">id</span><span class="sxs-lookup"><span data-stu-id="5bb90-133">id</span></span>|<span data-ttu-id="5bb90-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb90-134">String</span></span>|<span data-ttu-id="5bb90-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="5bb90-135">UUID for the object</span></span>|
|<span data-ttu-id="5bb90-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb90-136">eventDateTime</span></span>|<span data-ttu-id="5bb90-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb90-137">DateTimeOffset</span></span>|<span data-ttu-id="5bb90-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="5bb90-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="5bb90-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="5bb90-139">correlationId</span></span>|<span data-ttu-id="5bb90-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb90-140">String</span></span>|<span data-ttu-id="5bb90-141">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="5bb90-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="5bb90-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5bb90-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="5bb90-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5bb90-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="5bb90-144">Objeto que contém informações detalhadas sobre o erro e suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="5bb90-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="5bb90-145">eventName</span><span class="sxs-lookup"><span data-stu-id="5bb90-145">eventName</span></span>|<span data-ttu-id="5bb90-146">String</span><span class="sxs-lookup"><span data-stu-id="5bb90-146">String</span></span>|<span data-ttu-id="5bb90-147">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="5bb90-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="5bb90-148">Ele é um campo opcional</span><span class="sxs-lookup"><span data-stu-id="5bb90-148">It is an Optional field</span></span>|
|<span data-ttu-id="5bb90-149">informações adicionais</span><span class="sxs-lookup"><span data-stu-id="5bb90-149">additionalInformation</span></span>|<span data-ttu-id="5bb90-150">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5bb90-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5bb90-151">Um conjunto de chave de cadeia de caracteres e pares de valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="5bb90-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="5bb90-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb90-152">Response</span></span>
<span data-ttu-id="5bb90-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bb90-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb90-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bb90-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb90-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb90-155">Request</span></span>
<span data-ttu-id="5bb90-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bb90-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bb90-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb90-157">Response</span></span>
<span data-ttu-id="5bb90-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bb90-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




