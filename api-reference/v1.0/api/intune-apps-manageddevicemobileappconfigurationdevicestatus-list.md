---
title: Listar managedDeviceMobileAppConfigurationDeviceStatuses
description: Listar Propriedades e relações dos objetos managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a97d8ebfed484db6a4762b5a10bc8ab2779495bd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462112"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="e3ecc-103">Listar managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e3ecc-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

<span data-ttu-id="e3ecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3ecc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3ecc-106">Listar Propriedades e relações dos objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e3ecc-106">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3ecc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3ecc-107">Prerequisites</span></span>
<span data-ttu-id="e3ecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ecc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3ecc-110">Permission type</span></span>|<span data-ttu-id="e3ecc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3ecc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3ecc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3ecc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3ecc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ecc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3ecc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3ecc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3ecc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-115">Not supported.</span></span>|
|<span data-ttu-id="e3ecc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3ecc-116">Application</span></span>|<span data-ttu-id="e3ecc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3ecc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ecc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e3ecc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ecc-119">Request headers</span></span>
|<span data-ttu-id="e3ecc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3ecc-120">Header</span></span>|<span data-ttu-id="e3ecc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e3ecc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3ecc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3ecc-122">Authorization</span></span>|<span data-ttu-id="e3ecc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3ecc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3ecc-124">Accept</span></span>|<span data-ttu-id="e3ecc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3ecc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ecc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ecc-126">Request body</span></span>
<span data-ttu-id="e3ecc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ecc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ecc-128">Response</span></span>
<span data-ttu-id="e3ecc-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ecc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3ecc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3ecc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ecc-131">Request</span></span>
<span data-ttu-id="e3ecc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="e3ecc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ecc-133">Response</span></span>
<span data-ttu-id="e3ecc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3ecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```






