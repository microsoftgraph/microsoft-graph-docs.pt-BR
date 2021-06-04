---
title: Get enrollmentTroubleshootingEvent
description: Propriedades de leitura e relações do objeto enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c62ed979c9693340a69b38cb4bb5c81c5badf379
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732303"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="55876-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="55876-103">Get enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="55876-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55876-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55876-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55876-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55876-106">Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="55876-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55876-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55876-107">Prerequisites</span></span>
<span data-ttu-id="55876-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55876-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55876-110">Permission type</span></span>|<span data-ttu-id="55876-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55876-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55876-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55876-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55876-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="55876-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="55876-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55876-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55876-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55876-115">Not supported.</span></span>|
|<span data-ttu-id="55876-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55876-116">Application</span></span>|<span data-ttu-id="55876-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55876-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55876-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55876-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55876-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55876-119">Optional query parameters</span></span>
<span data-ttu-id="55876-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55876-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55876-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55876-121">Request headers</span></span>
|<span data-ttu-id="55876-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55876-122">Header</span></span>|<span data-ttu-id="55876-123">Valor</span><span class="sxs-lookup"><span data-stu-id="55876-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55876-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55876-124">Authorization</span></span>|<span data-ttu-id="55876-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55876-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55876-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55876-126">Accept</span></span>|<span data-ttu-id="55876-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55876-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55876-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55876-128">Request body</span></span>
<span data-ttu-id="55876-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55876-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55876-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="55876-130">Response</span></span>
<span data-ttu-id="55876-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55876-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55876-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55876-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="55876-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55876-133">Request</span></span>
<span data-ttu-id="55876-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55876-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="55876-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="55876-135">Response</span></span>
<span data-ttu-id="55876-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55876-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "operatingSystem": "Operating System value",
    "osVersion": "Os Version value",
    "userId": "User Id value",
    "deviceId": "Device Id value",
    "enrollmentType": "userEnrollment",
    "failureCategory": "authentication",
    "failureReason": "Failure Reason value"
  }
}
```









