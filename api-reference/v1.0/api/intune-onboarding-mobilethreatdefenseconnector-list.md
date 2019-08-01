---
title: Listar mobileThreatDefenseConnectors
description: Lista propriedades e relações dos objetos mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9948b6797232c6d21446c9432f9284f8ed298be8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976702"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="73d1e-103">Listar mobileThreatDefenseConnectors</span><span class="sxs-lookup"><span data-stu-id="73d1e-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="73d1e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73d1e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73d1e-105">Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="73d1e-105">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73d1e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73d1e-106">Prerequisites</span></span>
<span data-ttu-id="73d1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73d1e-109">Permission type</span></span>|<span data-ttu-id="73d1e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73d1e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73d1e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73d1e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73d1e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="73d1e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="73d1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73d1e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73d1e-114">Not supported.</span></span>|
|<span data-ttu-id="73d1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73d1e-115">Application</span></span>|<span data-ttu-id="73d1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73d1e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73d1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73d1e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="73d1e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73d1e-118">Request headers</span></span>
|<span data-ttu-id="73d1e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73d1e-119">Header</span></span>|<span data-ttu-id="73d1e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="73d1e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73d1e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="73d1e-121">Authorization</span></span>|<span data-ttu-id="73d1e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73d1e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73d1e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73d1e-123">Accept</span></span>|<span data-ttu-id="73d1e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="73d1e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d1e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73d1e-125">Request body</span></span>
<span data-ttu-id="73d1e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73d1e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d1e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d1e-127">Response</span></span>
<span data-ttu-id="73d1e-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73d1e-128">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d1e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73d1e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="73d1e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73d1e-130">Request</span></span>
<span data-ttu-id="73d1e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73d1e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="73d1e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d1e-132">Response</span></span>
<span data-ttu-id="73d1e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73d1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6
    }
  ]
}
```



