---
title: Acessar deviceManagementTroubleshootingEvent
description: Leia as propriedades e as relações do objeto deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4df24a618f71804090b1b4ad5cd8b1c320664be
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732307"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="7596f-103">Acessar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7596f-103">Get deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="7596f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7596f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7596f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7596f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7596f-106">Leia as propriedades e as relações do objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7596f-106">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7596f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7596f-107">Prerequisites</span></span>
<span data-ttu-id="7596f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7596f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7596f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7596f-110">Permission type</span></span>|<span data-ttu-id="7596f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7596f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7596f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7596f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7596f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7596f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7596f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7596f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7596f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7596f-115">Not supported.</span></span>|
|<span data-ttu-id="7596f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7596f-116">Application</span></span>|<span data-ttu-id="7596f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7596f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7596f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7596f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7596f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7596f-119">Optional query parameters</span></span>
<span data-ttu-id="7596f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7596f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7596f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7596f-121">Request headers</span></span>
|<span data-ttu-id="7596f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7596f-122">Header</span></span>|<span data-ttu-id="7596f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7596f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7596f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7596f-124">Authorization</span></span>|<span data-ttu-id="7596f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7596f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7596f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7596f-126">Accept</span></span>|<span data-ttu-id="7596f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7596f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7596f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7596f-128">Request body</span></span>
<span data-ttu-id="7596f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7596f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7596f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7596f-130">Response</span></span>
<span data-ttu-id="7596f-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7596f-131">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7596f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7596f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7596f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7596f-133">Request</span></span>
<span data-ttu-id="7596f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7596f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="7596f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7596f-135">Response</span></span>
<span data-ttu-id="7596f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7596f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









