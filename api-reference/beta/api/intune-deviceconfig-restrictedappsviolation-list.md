---
title: Listar restrictedAppsViolations
description: Listar Propriedades e relações dos objetos restrictedAppsViolation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad33582abce305845b2b8903829902f01530150c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42483676"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="bff1e-103">Listar restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="bff1e-103">List restrictedAppsViolations</span></span>

<span data-ttu-id="bff1e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bff1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bff1e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bff1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bff1e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bff1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bff1e-107">Listar Propriedades e relações dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="bff1e-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bff1e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bff1e-108">Prerequisites</span></span>
<span data-ttu-id="bff1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bff1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bff1e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bff1e-111">Permission type</span></span>|<span data-ttu-id="bff1e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bff1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bff1e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bff1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bff1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bff1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bff1e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bff1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bff1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bff1e-116">Not supported.</span></span>|
|<span data-ttu-id="bff1e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bff1e-117">Application</span></span>|<span data-ttu-id="bff1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bff1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bff1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bff1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="bff1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bff1e-120">Request headers</span></span>
|<span data-ttu-id="bff1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bff1e-121">Header</span></span>|<span data-ttu-id="bff1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bff1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bff1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bff1e-123">Authorization</span></span>|<span data-ttu-id="bff1e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bff1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bff1e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bff1e-125">Accept</span></span>|<span data-ttu-id="bff1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bff1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bff1e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bff1e-127">Request body</span></span>
<span data-ttu-id="bff1e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bff1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bff1e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff1e-129">Response</span></span>
<span data-ttu-id="bff1e-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bff1e-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bff1e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bff1e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bff1e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bff1e-132">Request</span></span>
<span data-ttu-id="bff1e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bff1e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="bff1e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff1e-134">Response</span></span>
<span data-ttu-id="bff1e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bff1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





