---
title: Listar appleVppTokenTroubleshootingEvents
description: Listar Propriedades e relações dos objetos appleVppTokenTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1f6c2bca6b29974dc22b819967f5a077cf31f9c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939054"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="48193-103">Listar appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="48193-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="48193-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48193-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48193-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48193-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48193-106">Listar Propriedades e relações dos objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="48193-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48193-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48193-107">Prerequisites</span></span>
<span data-ttu-id="48193-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48193-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48193-110">Permission type</span></span>|<span data-ttu-id="48193-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48193-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48193-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48193-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48193-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48193-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="48193-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48193-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48193-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48193-115">Not supported.</span></span>|
|<span data-ttu-id="48193-116">Application</span><span class="sxs-lookup"><span data-stu-id="48193-116">Application</span></span>|<span data-ttu-id="48193-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48193-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48193-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48193-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="48193-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48193-119">Request headers</span></span>
|<span data-ttu-id="48193-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48193-120">Header</span></span>|<span data-ttu-id="48193-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48193-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48193-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48193-122">Authorization</span></span>|<span data-ttu-id="48193-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48193-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48193-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48193-124">Accept</span></span>|<span data-ttu-id="48193-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48193-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48193-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48193-126">Request body</span></span>
<span data-ttu-id="48193-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48193-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48193-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="48193-128">Response</span></span>
<span data-ttu-id="48193-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48193-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48193-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48193-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="48193-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48193-131">Request</span></span>
<span data-ttu-id="48193-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48193-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="48193-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="48193-133">Response</span></span>
<span data-ttu-id="48193-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48193-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





