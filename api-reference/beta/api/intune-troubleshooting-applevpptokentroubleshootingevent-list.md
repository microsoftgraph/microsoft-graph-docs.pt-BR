---
title: Listar appleVppTokenTroubleshootingEvents
description: Listar Propriedades e relações dos objetos appleVppTokenTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae9fb48fdae7658ba2c4f8de652b7e2481bb387f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350311"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="3c152-103">Listar appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="3c152-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="3c152-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c152-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c152-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c152-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c152-106">Listar Propriedades e relações dos objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="3c152-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c152-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c152-107">Prerequisites</span></span>
<span data-ttu-id="3c152-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c152-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c152-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c152-110">Permission type</span></span>|<span data-ttu-id="3c152-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c152-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c152-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c152-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c152-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="3c152-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="3c152-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c152-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c152-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c152-115">Not supported.</span></span>|
|<span data-ttu-id="3c152-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c152-116">Application</span></span>|<span data-ttu-id="3c152-117">\* \* TODO: Determine escopos ao apponly \* \*</span><span class="sxs-lookup"><span data-stu-id="3c152-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c152-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c152-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="3c152-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c152-119">Request headers</span></span>
|<span data-ttu-id="3c152-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c152-120">Header</span></span>|<span data-ttu-id="3c152-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3c152-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c152-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c152-122">Authorization</span></span>|<span data-ttu-id="3c152-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c152-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c152-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c152-124">Accept</span></span>|<span data-ttu-id="3c152-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c152-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c152-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c152-126">Request body</span></span>
<span data-ttu-id="3c152-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c152-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c152-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c152-128">Response</span></span>
<span data-ttu-id="3c152-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c152-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c152-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c152-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c152-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c152-131">Request</span></span>
<span data-ttu-id="3c152-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c152-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="3c152-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c152-133">Response</span></span>
<span data-ttu-id="3c152-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c152-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






