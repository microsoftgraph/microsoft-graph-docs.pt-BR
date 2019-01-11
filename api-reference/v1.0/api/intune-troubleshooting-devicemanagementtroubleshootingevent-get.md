---
title: Acessar deviceManagementTroubleshootingEvent
description: Leia as propriedades e as relações do objeto deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1704536a527e78d3a49e577e487e2f5f417c7514
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839680"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="a7d03-103">Acessar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7d03-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="a7d03-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7d03-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7d03-105">Leia as propriedades e as relações do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a7d03-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7d03-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7d03-106">Prerequisites</span></span>
<span data-ttu-id="a7d03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7d03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7d03-109">Permission type</span></span>|<span data-ttu-id="a7d03-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7d03-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7d03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7d03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7d03-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7d03-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a7d03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7d03-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7d03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7d03-114">Not supported.</span></span>|
|<span data-ttu-id="a7d03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7d03-115">Application</span></span>|<span data-ttu-id="a7d03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7d03-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7d03-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d03-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7d03-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7d03-118">Optional query parameters</span></span>
<span data-ttu-id="a7d03-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7d03-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a7d03-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d03-120">Request headers</span></span>
|<span data-ttu-id="a7d03-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7d03-121">Header</span></span>|<span data-ttu-id="a7d03-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7d03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7d03-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7d03-123">Authorization</span></span>|<span data-ttu-id="a7d03-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7d03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7d03-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7d03-125">Accept</span></span>|<span data-ttu-id="a7d03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7d03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7d03-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d03-127">Request body</span></span>
<span data-ttu-id="a7d03-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7d03-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d03-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7d03-129">Response</span></span>
<span data-ttu-id="a7d03-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7d03-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7d03-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7d03-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7d03-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d03-132">Request</span></span>
<span data-ttu-id="a7d03-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7d03-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="a7d03-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7d03-134">Response</span></span>
<span data-ttu-id="a7d03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7d03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```



