---
title: Listar mobileThreatDefenseConnectors
description: Lista propriedades e relações dos objetos mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d4203121e3b50f6700daafbd012cee476a6eeac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224274"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="f377a-103">Listar mobileThreatDefenseConnectors</span><span class="sxs-lookup"><span data-stu-id="f377a-103">List mobileThreatDefenseConnectors</span></span>

<span data-ttu-id="f377a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f377a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f377a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f377a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f377a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f377a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f377a-107">Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f377a-107">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f377a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f377a-108">Prerequisites</span></span>
<span data-ttu-id="f377a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f377a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f377a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f377a-111">Permission type</span></span>|<span data-ttu-id="f377a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f377a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f377a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f377a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f377a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f377a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f377a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f377a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f377a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f377a-116">Not supported.</span></span>|
|<span data-ttu-id="f377a-117">Application</span><span class="sxs-lookup"><span data-stu-id="f377a-117">Application</span></span>|<span data-ttu-id="f377a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f377a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f377a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f377a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f377a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f377a-120">Request headers</span></span>
|<span data-ttu-id="f377a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f377a-121">Header</span></span>|<span data-ttu-id="f377a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f377a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f377a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f377a-123">Authorization</span></span>|<span data-ttu-id="f377a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f377a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f377a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f377a-125">Accept</span></span>|<span data-ttu-id="f377a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f377a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f377a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f377a-127">Request body</span></span>
<span data-ttu-id="f377a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f377a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f377a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f377a-129">Response</span></span>
<span data-ttu-id="f377a-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f377a-130">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f377a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f377a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f377a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f377a-132">Request</span></span>
<span data-ttu-id="f377a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f377a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="f377a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f377a-134">Response</span></span>
<span data-ttu-id="f377a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f377a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 876

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidMobileApplicationManagementEnabled": true,
      "iosMobileApplicationManagementEnabled": true,
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




