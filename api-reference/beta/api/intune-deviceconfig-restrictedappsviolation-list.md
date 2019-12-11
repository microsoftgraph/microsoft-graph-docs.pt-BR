---
title: Listar restrictedAppsViolations
description: Listar Propriedades e relações dos objetos restrictedAppsViolation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 136736c07302bc1741084662dfa33539b77ef587
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947831"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="9c655-103">Listar restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="9c655-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="9c655-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c655-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c655-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c655-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c655-106">Listar Propriedades e relações dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="9c655-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c655-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c655-107">Prerequisites</span></span>
<span data-ttu-id="9c655-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c655-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c655-110">Permission type</span></span>|<span data-ttu-id="9c655-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c655-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c655-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c655-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c655-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c655-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9c655-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c655-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c655-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c655-115">Not supported.</span></span>|
|<span data-ttu-id="9c655-116">Application</span><span class="sxs-lookup"><span data-stu-id="9c655-116">Application</span></span>|<span data-ttu-id="9c655-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c655-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c655-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c655-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="9c655-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c655-119">Request headers</span></span>
|<span data-ttu-id="9c655-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c655-120">Header</span></span>|<span data-ttu-id="9c655-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9c655-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c655-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c655-122">Authorization</span></span>|<span data-ttu-id="9c655-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c655-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c655-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c655-124">Accept</span></span>|<span data-ttu-id="9c655-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c655-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c655-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c655-126">Request body</span></span>
<span data-ttu-id="9c655-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c655-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c655-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c655-128">Response</span></span>
<span data-ttu-id="9c655-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c655-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c655-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c655-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c655-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c655-131">Request</span></span>
<span data-ttu-id="9c655-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c655-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="9c655-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c655-133">Response</span></span>
<span data-ttu-id="9c655-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c655-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





