---
title: Listar restrictedAppsViolations
description: Listar Propriedades e relações dos objetos restrictedAppsViolation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24b5096ea6003a15dd014336e9059bd2922370ff
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976320"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="127c6-103">Listar restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="127c6-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="127c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="127c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="127c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="127c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127c6-106">Listar Propriedades e relações dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="127c6-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="127c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="127c6-107">Prerequisites</span></span>
<span data-ttu-id="127c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="127c6-110">Permission type</span></span>|<span data-ttu-id="127c6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="127c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="127c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="127c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="127c6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="127c6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="127c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="127c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="127c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="127c6-115">Not supported.</span></span>|
|<span data-ttu-id="127c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="127c6-116">Application</span></span>|<span data-ttu-id="127c6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="127c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="127c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="127c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="127c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="127c6-119">Request headers</span></span>
|<span data-ttu-id="127c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="127c6-120">Header</span></span>|<span data-ttu-id="127c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="127c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="127c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="127c6-122">Authorization</span></span>|<span data-ttu-id="127c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="127c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="127c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="127c6-124">Accept</span></span>|<span data-ttu-id="127c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="127c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="127c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="127c6-126">Request body</span></span>
<span data-ttu-id="127c6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="127c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="127c6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="127c6-128">Response</span></span>
<span data-ttu-id="127c6-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="127c6-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="127c6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="127c6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="127c6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="127c6-131">Request</span></span>
<span data-ttu-id="127c6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="127c6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="127c6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="127c6-133">Response</span></span>
<span data-ttu-id="127c6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="127c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





