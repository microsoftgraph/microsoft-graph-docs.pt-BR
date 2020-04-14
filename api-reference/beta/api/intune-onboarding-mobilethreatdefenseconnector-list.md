---
title: Listar mobileThreatDefenseConnectors
description: Lista propriedades e relações dos objetos mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73423c1e14fc00dfdfb14d8ee7b2fdf3c4611062
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377725"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="62d08-103">Listar mobileThreatDefenseConnectors</span><span class="sxs-lookup"><span data-stu-id="62d08-103">List mobileThreatDefenseConnectors</span></span>

<span data-ttu-id="62d08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62d08-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62d08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62d08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d08-107">Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="62d08-107">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62d08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62d08-108">Prerequisites</span></span>
<span data-ttu-id="62d08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62d08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62d08-111">Permission type</span></span>|<span data-ttu-id="62d08-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62d08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62d08-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62d08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62d08-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="62d08-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="62d08-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62d08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62d08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d08-116">Not supported.</span></span>|
|<span data-ttu-id="62d08-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62d08-117">Application</span></span>|<span data-ttu-id="62d08-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="62d08-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62d08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62d08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="62d08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62d08-120">Request headers</span></span>
|<span data-ttu-id="62d08-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62d08-121">Header</span></span>|<span data-ttu-id="62d08-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62d08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62d08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62d08-123">Authorization</span></span>|<span data-ttu-id="62d08-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62d08-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62d08-125">Accept</span></span>|<span data-ttu-id="62d08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62d08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62d08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62d08-127">Request body</span></span>
<span data-ttu-id="62d08-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62d08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62d08-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d08-129">Response</span></span>
<span data-ttu-id="62d08-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62d08-130">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d08-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62d08-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="62d08-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62d08-132">Request</span></span>
<span data-ttu-id="62d08-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62d08-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="62d08-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d08-134">Response</span></span>
<span data-ttu-id="62d08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62d08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



