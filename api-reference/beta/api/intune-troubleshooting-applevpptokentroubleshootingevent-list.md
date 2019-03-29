---
title: Listar appleVppTokenTroubleshootingEvents
description: Listar Propriedades e relações dos objetos appleVppTokenTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97d2dc494924f937357787d8c5605e538dceffd9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984608"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="20069-103">Listar appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="20069-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="20069-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20069-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20069-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20069-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20069-106">Listar Propriedades e relações dos objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="20069-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20069-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20069-107">Prerequisites</span></span>
<span data-ttu-id="20069-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20069-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20069-110">Permission type</span></span>|<span data-ttu-id="20069-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20069-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20069-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20069-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20069-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20069-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="20069-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20069-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20069-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20069-115">Not supported.</span></span>|
|<span data-ttu-id="20069-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20069-116">Application</span></span>|<span data-ttu-id="20069-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20069-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20069-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20069-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="20069-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20069-119">Request headers</span></span>
|<span data-ttu-id="20069-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20069-120">Header</span></span>|<span data-ttu-id="20069-121">Valor</span><span class="sxs-lookup"><span data-stu-id="20069-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20069-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20069-122">Authorization</span></span>|<span data-ttu-id="20069-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20069-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20069-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20069-124">Accept</span></span>|<span data-ttu-id="20069-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20069-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20069-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20069-126">Request body</span></span>
<span data-ttu-id="20069-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20069-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20069-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="20069-128">Response</span></span>
<span data-ttu-id="20069-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20069-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20069-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20069-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="20069-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20069-131">Request</span></span>
<span data-ttu-id="20069-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20069-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="20069-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="20069-133">Response</span></span>
<span data-ttu-id="20069-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20069-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




