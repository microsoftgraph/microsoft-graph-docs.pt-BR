---
title: Acessar deviceManagementTroubleshootingEvent
description: Leia as propriedades e as relações do objeto deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23c91f98d5f254f8a86fe1b551b223090a1e78d5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712873"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="679df-103">Acessar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="679df-103">Get deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="679df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="679df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="679df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="679df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="679df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="679df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="679df-107">Leia as propriedades e as relações do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="679df-107">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="679df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="679df-108">Prerequisites</span></span>
<span data-ttu-id="679df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="679df-111">Permission type</span></span>|<span data-ttu-id="679df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="679df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="679df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="679df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="679df-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="679df-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="679df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="679df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="679df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679df-116">Not supported.</span></span>|
|<span data-ttu-id="679df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="679df-117">Application</span></span>|<span data-ttu-id="679df-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="679df-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="679df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="679df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="679df-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="679df-120">Optional query parameters</span></span>
<span data-ttu-id="679df-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="679df-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-122">Request headers</span></span>
|<span data-ttu-id="679df-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="679df-123">Header</span></span>|<span data-ttu-id="679df-124">Valor</span><span class="sxs-lookup"><span data-stu-id="679df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="679df-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="679df-125">Authorization</span></span>|<span data-ttu-id="679df-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="679df-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="679df-127">Accept</span></span>|<span data-ttu-id="679df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="679df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="679df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-129">Request body</span></span>
<span data-ttu-id="679df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="679df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="679df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="679df-131">Response</span></span>
<span data-ttu-id="679df-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-132">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679df-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="679df-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="679df-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-134">Request</span></span>
<span data-ttu-id="679df-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="679df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="679df-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="679df-136">Response</span></span>
<span data-ttu-id="679df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="679df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 972

{
  "value": {
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
}
```





