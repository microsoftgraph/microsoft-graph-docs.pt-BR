---
title: Obter appleVppTokenTroubleshootingEvent
description: Leia as propriedades e os relacionamentos do objeto appleVppTokenTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fce083d7a29f8cf0e69c0fb81d0c0cc13f8e58dd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429092"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="b9758-103">Obter appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b9758-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="b9758-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9758-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b9758-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9758-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9758-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b9758-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9758-107">Leia as propriedades e os relacionamentos do objeto [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="b9758-107">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9758-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9758-108">Prerequisites</span></span>
<span data-ttu-id="b9758-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9758-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9758-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9758-111">Permission type</span></span>|<span data-ttu-id="b9758-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9758-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9758-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9758-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9758-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9758-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b9758-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9758-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9758-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9758-116">Not supported.</span></span>|
|<span data-ttu-id="b9758-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9758-117">Application</span></span>|<span data-ttu-id="b9758-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9758-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9758-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9758-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9758-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9758-120">Optional query parameters</span></span>
<span data-ttu-id="b9758-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9758-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9758-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9758-122">Request headers</span></span>
|<span data-ttu-id="b9758-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9758-123">Header</span></span>|<span data-ttu-id="b9758-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9758-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9758-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9758-125">Authorization</span></span>|<span data-ttu-id="b9758-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9758-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9758-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9758-127">Accept</span></span>|<span data-ttu-id="b9758-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9758-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9758-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9758-129">Request body</span></span>
<span data-ttu-id="b9758-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9758-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9758-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9758-131">Response</span></span>
<span data-ttu-id="b9758-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9758-132">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9758-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9758-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9758-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9758-134">Request</span></span>
<span data-ttu-id="b9758-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9758-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="b9758-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9758-136">Response</span></span>
<span data-ttu-id="b9758-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9758-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




