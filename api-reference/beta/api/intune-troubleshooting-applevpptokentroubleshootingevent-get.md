---
title: Obter appleVppTokenTroubleshootingEvent
description: Leia as propriedades e as relações do objeto appleVppTokenTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 983de8437eacd0e57fa6f2b683ac40f53237dd28
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537759"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="e9ab8-103">Obter appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e9ab8-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="e9ab8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9ab8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9ab8-106">Leia as propriedades e as relações do objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e9ab8-106">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9ab8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9ab8-107">Prerequisites</span></span>
<span data-ttu-id="e9ab8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9ab8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9ab8-110">Permission type</span></span>|<span data-ttu-id="e9ab8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9ab8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9ab8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9ab8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9ab8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ab8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e9ab8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9ab8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9ab8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-115">Not supported.</span></span>|
|<span data-ttu-id="e9ab8-116">Application</span><span class="sxs-lookup"><span data-stu-id="e9ab8-116">Application</span></span>|<span data-ttu-id="e9ab8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ab8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9ab8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ab8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9ab8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9ab8-119">Optional query parameters</span></span>
<span data-ttu-id="e9ab8-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9ab8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ab8-121">Request headers</span></span>
|<span data-ttu-id="e9ab8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9ab8-122">Header</span></span>|<span data-ttu-id="e9ab8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e9ab8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9ab8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9ab8-124">Authorization</span></span>|<span data-ttu-id="e9ab8-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9ab8-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9ab8-126">Accept</span></span>|<span data-ttu-id="e9ab8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9ab8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9ab8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ab8-128">Request body</span></span>
<span data-ttu-id="e9ab8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9ab8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ab8-130">Response</span></span>
<span data-ttu-id="e9ab8-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-131">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9ab8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9ab8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9ab8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ab8-133">Request</span></span>
<span data-ttu-id="e9ab8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e9ab8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ab8-135">Response</span></span>
<span data-ttu-id="e9ab8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9ab8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1003

{
  "value": {
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
}
```






