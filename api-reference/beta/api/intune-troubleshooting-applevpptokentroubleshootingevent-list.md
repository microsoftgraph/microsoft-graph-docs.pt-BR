---
title: Listar appleVppTokenTroubleshootingEvents
description: Listar Propriedades e relações dos objetos appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfcaacf8dce192b7d8cb2288e19c0ea6fe725a57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999626"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="cf5f4-103">Listar appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="cf5f4-103">List appleVppTokenTroubleshootingEvents</span></span>

<span data-ttu-id="cf5f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf5f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf5f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf5f4-107">Listar Propriedades e relações dos objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="cf5f4-107">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf5f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf5f4-108">Prerequisites</span></span>
<span data-ttu-id="cf5f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf5f4-111">Permission type</span></span>|<span data-ttu-id="cf5f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf5f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf5f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf5f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf5f4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf5f4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cf5f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf5f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf5f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-116">Not supported.</span></span>|
|<span data-ttu-id="cf5f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf5f4-117">Application</span></span>|<span data-ttu-id="cf5f4-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf5f4-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf5f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf5f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="cf5f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f4-120">Request headers</span></span>
|<span data-ttu-id="cf5f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf5f4-121">Header</span></span>|<span data-ttu-id="cf5f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf5f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf5f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf5f4-123">Authorization</span></span>|<span data-ttu-id="cf5f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf5f4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf5f4-125">Accept</span></span>|<span data-ttu-id="cf5f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf5f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf5f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f4-127">Request body</span></span>
<span data-ttu-id="cf5f4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf5f4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5f4-129">Response</span></span>
<span data-ttu-id="cf5f4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-130">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5f4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf5f4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf5f4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f4-132">Request</span></span>
<span data-ttu-id="cf5f4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="cf5f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5f4-134">Response</span></span>
<span data-ttu-id="cf5f4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf5f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1071

{
  "value": [
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
  ]
}
```






