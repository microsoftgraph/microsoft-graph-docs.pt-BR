---
title: Atualizar appleVppTokenTroubleshootingEvent
description: Atualize as propriedades de um objeto appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57bd6638e03dea35a47fc894c3789ea2004a21f5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123416"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="d66fa-103">Atualizar appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="d66fa-103">Update appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="d66fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d66fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d66fa-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d66fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d66fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d66fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d66fa-107">Atualize as propriedades de um [objeto appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d66fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d66fa-108">Prerequisites</span></span>
<span data-ttu-id="d66fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d66fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d66fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d66fa-111">Permission type</span></span>|<span data-ttu-id="d66fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d66fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d66fa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d66fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d66fa-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d66fa-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d66fa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d66fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d66fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d66fa-116">Not supported.</span></span>|
|<span data-ttu-id="d66fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d66fa-117">Application</span></span>|<span data-ttu-id="d66fa-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d66fa-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d66fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d66fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="d66fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d66fa-120">Request headers</span></span>
|<span data-ttu-id="d66fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d66fa-121">Header</span></span>|<span data-ttu-id="d66fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d66fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d66fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d66fa-123">Authorization</span></span>|<span data-ttu-id="d66fa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d66fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d66fa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d66fa-125">Accept</span></span>|<span data-ttu-id="d66fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d66fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d66fa-127">Request body</span></span>
<span data-ttu-id="d66fa-128">No corpo da solicitação, fornece uma representação JSON para o [objeto appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="d66fa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66fa-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="d66fa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d66fa-130">Property</span></span>|<span data-ttu-id="d66fa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d66fa-131">Type</span></span>|<span data-ttu-id="d66fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d66fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d66fa-133">id</span><span class="sxs-lookup"><span data-stu-id="d66fa-133">id</span></span>|<span data-ttu-id="d66fa-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d66fa-134">String</span></span>|<span data-ttu-id="d66fa-135">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d66fa-136">eventDateTime</span></span>|<span data-ttu-id="d66fa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d66fa-137">DateTimeOffset</span></span>|<span data-ttu-id="d66fa-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="d66fa-138">Time when the event occurred .</span></span> <span data-ttu-id="d66fa-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="d66fa-140">correlationId</span></span>|<span data-ttu-id="d66fa-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d66fa-141">String</span></span>|<span data-ttu-id="d66fa-142">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="d66fa-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="d66fa-143">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d66fa-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="d66fa-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d66fa-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="d66fa-146">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="d66fa-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="d66fa-147">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-148">eventName</span><span class="sxs-lookup"><span data-stu-id="d66fa-148">eventName</span></span>|<span data-ttu-id="d66fa-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d66fa-149">String</span></span>|<span data-ttu-id="d66fa-150">Nome do Evento correspondente ao Evento de Solução de Problemas.</span><span class="sxs-lookup"><span data-stu-id="d66fa-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="d66fa-151">É um campo Opcional Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="d66fa-152">additionalInformation</span></span>|<span data-ttu-id="d66fa-153">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d66fa-154">Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Troubleshooting Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66fa-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66fa-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="d66fa-155">tokenId</span></span>|<span data-ttu-id="d66fa-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d66fa-156">String</span></span>|<span data-ttu-id="d66fa-157">Identificador de Token de Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="d66fa-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="d66fa-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d66fa-158">Response</span></span>
<span data-ttu-id="d66fa-159">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d66fa-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d66fa-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d66fa-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="d66fa-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d66fa-161">Request</span></span>
<span data-ttu-id="d66fa-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d66fa-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d66fa-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d66fa-163">Response</span></span>
<span data-ttu-id="d66fa-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d66fa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




