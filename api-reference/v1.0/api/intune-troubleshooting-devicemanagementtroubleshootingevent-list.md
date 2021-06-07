---
title: Listar deviceManagementTroubleshootingEvents
description: Listar propriedades e relações de objetos de deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78ac4f5d2c5eb076745f90d45143b7b7a683cca5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732287"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="091d4-103">Listar deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="091d4-103">List deviceManagementTroubleshootingEvents</span></span>

<span data-ttu-id="091d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="091d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="091d4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="091d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="091d4-106">Listar propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="091d4-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="091d4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="091d4-107">Prerequisites</span></span>
<span data-ttu-id="091d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="091d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="091d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="091d4-110">Permission type</span></span>|<span data-ttu-id="091d4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="091d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="091d4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="091d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="091d4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="091d4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="091d4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="091d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="091d4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="091d4-115">Not supported.</span></span>|
|<span data-ttu-id="091d4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="091d4-116">Application</span></span>|<span data-ttu-id="091d4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="091d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="091d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="091d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="091d4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="091d4-119">Request headers</span></span>
|<span data-ttu-id="091d4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="091d4-120">Header</span></span>|<span data-ttu-id="091d4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="091d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="091d4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="091d4-122">Authorization</span></span>|<span data-ttu-id="091d4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="091d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="091d4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="091d4-124">Accept</span></span>|<span data-ttu-id="091d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="091d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="091d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="091d4-126">Request body</span></span>
<span data-ttu-id="091d4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="091d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="091d4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="091d4-128">Response</span></span>
<span data-ttu-id="091d4-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="091d4-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="091d4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="091d4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="091d4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="091d4-131">Request</span></span>
<span data-ttu-id="091d4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="091d4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="091d4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="091d4-133">Response</span></span>
<span data-ttu-id="091d4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="091d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```









