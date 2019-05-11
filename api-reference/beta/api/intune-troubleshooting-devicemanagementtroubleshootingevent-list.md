---
title: Listar deviceManagementTroubleshootingEvents
description: Listar propriedades e relações de objetos de deviceManagementTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef6fedfefba10b9e20a8c89c30c5dfb33d15623f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899267"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="6be51-103">Listar deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="6be51-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="6be51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6be51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6be51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be51-106">Listar propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6be51-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6be51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6be51-107">Prerequisites</span></span>
<span data-ttu-id="6be51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6be51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6be51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6be51-110">Permission type</span></span>|<span data-ttu-id="6be51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6be51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6be51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6be51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6be51-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be51-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6be51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6be51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6be51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6be51-115">Not supported.</span></span>|
|<span data-ttu-id="6be51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6be51-116">Application</span></span>|<span data-ttu-id="6be51-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6be51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6be51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6be51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="6be51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6be51-119">Request headers</span></span>
|<span data-ttu-id="6be51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6be51-120">Header</span></span>|<span data-ttu-id="6be51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6be51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6be51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6be51-122">Authorization</span></span>|<span data-ttu-id="6be51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6be51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6be51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6be51-124">Accept</span></span>|<span data-ttu-id="6be51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6be51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6be51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6be51-126">Request body</span></span>
<span data-ttu-id="6be51-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6be51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6be51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6be51-128">Response</span></span>
<span data-ttu-id="6be51-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6be51-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6be51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6be51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6be51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6be51-131">Request</span></span>
<span data-ttu-id="6be51-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6be51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="6be51-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6be51-133">Response</span></span>
<span data-ttu-id="6be51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6be51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
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
  ]
}
```




