---
title: Acessar deviceManagementTroubleshootingEvent
description: Leia as propriedades e as relações do objeto deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e53af3190d9c1282dbd7eb90908495c3d807906
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361144"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="16b5b-103">Acessar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="16b5b-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="16b5b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16b5b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16b5b-105">Leia as propriedades e as relações do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="16b5b-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16b5b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16b5b-106">Prerequisites</span></span>
<span data-ttu-id="16b5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b5b-109">Permission type</span></span>|<span data-ttu-id="16b5b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16b5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b5b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16b5b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16b5b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="16b5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b5b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b5b-114">Not supported.</span></span>|
|<span data-ttu-id="16b5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16b5b-115">Application</span></span>|<span data-ttu-id="16b5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16b5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16b5b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16b5b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16b5b-118">Optional query parameters</span></span>
<span data-ttu-id="16b5b-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16b5b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b5b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16b5b-120">Request headers</span></span>
|<span data-ttu-id="16b5b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16b5b-121">Header</span></span>|<span data-ttu-id="16b5b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16b5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16b5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16b5b-123">Authorization</span></span>|<span data-ttu-id="16b5b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16b5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16b5b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16b5b-125">Accept</span></span>|<span data-ttu-id="16b5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16b5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16b5b-127">Request body</span></span>
<span data-ttu-id="16b5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16b5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b5b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b5b-129">Response</span></span>
<span data-ttu-id="16b5b-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b5b-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b5b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16b5b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="16b5b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16b5b-132">Request</span></span>
<span data-ttu-id="16b5b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16b5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="16b5b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b5b-134">Response</span></span>
<span data-ttu-id="16b5b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16b5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




