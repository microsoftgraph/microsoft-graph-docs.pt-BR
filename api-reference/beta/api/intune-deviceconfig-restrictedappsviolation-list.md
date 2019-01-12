---
title: Lista restrictedAppsViolations
description: Lista as propriedades e os relacionamentos dos objetos restrictedAppsViolation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecd78f2300461198b31fb94117005995d12892bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950372"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="6cc0c-103">Lista restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="6cc0c-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="6cc0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cc0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cc0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cc0c-107">Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="6cc0c-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cc0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cc0c-108">Prerequisites</span></span>
<span data-ttu-id="6cc0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cc0c-111">Permission type</span></span>|<span data-ttu-id="6cc0c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cc0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc0c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cc0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc0c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cc0c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cc0c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cc0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-116">Not supported.</span></span>|
|<span data-ttu-id="6cc0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc0c-117">Application</span></span>|<span data-ttu-id="6cc0c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="6cc0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc0c-120">Request headers</span></span>
|<span data-ttu-id="6cc0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cc0c-121">Header</span></span>|<span data-ttu-id="6cc0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cc0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cc0c-123">Authorization</span></span>|<span data-ttu-id="6cc0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc0c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cc0c-125">Accept</span></span>|<span data-ttu-id="6cc0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc0c-127">Request body</span></span>
<span data-ttu-id="6cc0c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cc0c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc0c-129">Response</span></span>
<span data-ttu-id="6cc0c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc0c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cc0c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cc0c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc0c-132">Request</span></span>
<span data-ttu-id="6cc0c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="6cc0c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc0c-134">Response</span></span>
<span data-ttu-id="6cc0c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cc0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





