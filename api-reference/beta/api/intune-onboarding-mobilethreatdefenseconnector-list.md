---
title: Listar mobileThreatDefenseConnectors
description: Lista propriedades e relações dos objetos mobileThreatDefenseConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a3a9146e9280651652fefdd3798a842a335a508
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411264"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="b6fa9-103">Listar mobileThreatDefenseConnectors</span><span class="sxs-lookup"><span data-stu-id="b6fa9-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="b6fa9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6fa9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6fa9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6fa9-107">Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b6fa9-107">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6fa9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6fa9-108">Prerequisites</span></span>
<span data-ttu-id="b6fa9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6fa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6fa9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6fa9-111">Permission type</span></span>|<span data-ttu-id="b6fa9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6fa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6fa9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6fa9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6fa9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6fa9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b6fa9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6fa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6fa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-116">Not supported.</span></span>|
|<span data-ttu-id="b6fa9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6fa9-117">Application</span></span>|<span data-ttu-id="b6fa9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6fa9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6fa9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="b6fa9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fa9-120">Request headers</span></span>
|<span data-ttu-id="b6fa9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6fa9-121">Header</span></span>|<span data-ttu-id="b6fa9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6fa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6fa9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6fa9-123">Authorization</span></span>|<span data-ttu-id="b6fa9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6fa9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6fa9-125">Accept</span></span>|<span data-ttu-id="b6fa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6fa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6fa9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fa9-127">Request body</span></span>
<span data-ttu-id="b6fa9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6fa9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6fa9-129">Response</span></span>
<span data-ttu-id="b6fa9-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-130">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6fa9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6fa9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6fa9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6fa9-132">Request</span></span>
<span data-ttu-id="b6fa9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="b6fa9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6fa9-134">Response</span></span>
<span data-ttu-id="b6fa9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6fa9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "windowsEnabled": true,
      "macEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "windowsDeviceBlockedOnMissingPartnerData": true,
      "macDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6,
      "allowPartnerToCollectIOSApplicationMetadata": true
    }
  ]
}
```




