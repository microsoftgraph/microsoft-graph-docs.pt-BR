---
title: Listar appleVppTokenTroubleshootingEvents
description: Listar Propriedades e relações dos objetos appleVppTokenTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b62a27afd14bac902d5a6f8b28c85ab3bf2f9e0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195528"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="0a5bb-103">Listar appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="0a5bb-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="0a5bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a5bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a5bb-106">Listar Propriedades e relações dos objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0a5bb-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a5bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a5bb-107">Prerequisites</span></span>
<span data-ttu-id="0a5bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a5bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a5bb-110">Permission type</span></span>|<span data-ttu-id="0a5bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a5bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a5bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a5bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a5bb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a5bb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0a5bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a5bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a5bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-115">Not supported.</span></span>|
|<span data-ttu-id="0a5bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a5bb-116">Application</span></span>|<span data-ttu-id="0a5bb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a5bb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a5bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a5bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0a5bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5bb-119">Request headers</span></span>
|<span data-ttu-id="0a5bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a5bb-120">Header</span></span>|<span data-ttu-id="0a5bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0a5bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a5bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a5bb-122">Authorization</span></span>|<span data-ttu-id="0a5bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a5bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a5bb-124">Accept</span></span>|<span data-ttu-id="0a5bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a5bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a5bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5bb-126">Request body</span></span>
<span data-ttu-id="0a5bb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a5bb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a5bb-128">Response</span></span>
<span data-ttu-id="0a5bb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a5bb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a5bb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a5bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5bb-131">Request</span></span>
<span data-ttu-id="0a5bb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="0a5bb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a5bb-133">Response</span></span>
<span data-ttu-id="0a5bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a5bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




