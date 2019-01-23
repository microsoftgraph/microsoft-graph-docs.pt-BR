---
title: Lista restrictedAppsViolations
description: Lista as propriedades e os relacionamentos dos objetos restrictedAppsViolation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 284eeac8ca2220058ac1233540d3d845b55d1bd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410179"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="feded-103">Lista restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="feded-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="feded-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="feded-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="feded-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="feded-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="feded-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="feded-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feded-107">Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="feded-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feded-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="feded-108">Prerequisites</span></span>
<span data-ttu-id="feded-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="feded-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="feded-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feded-111">Permission type</span></span>|<span data-ttu-id="feded-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="feded-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feded-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feded-113">Delegated (work or school account)</span></span>|<span data-ttu-id="feded-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="feded-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="feded-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feded-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feded-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feded-116">Not supported.</span></span>|
|<span data-ttu-id="feded-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feded-117">Application</span></span>|<span data-ttu-id="feded-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feded-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feded-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feded-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="feded-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feded-120">Request headers</span></span>
|<span data-ttu-id="feded-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="feded-121">Header</span></span>|<span data-ttu-id="feded-122">Valor</span><span class="sxs-lookup"><span data-stu-id="feded-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feded-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="feded-123">Authorization</span></span>|<span data-ttu-id="feded-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feded-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feded-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="feded-125">Accept</span></span>|<span data-ttu-id="feded-126">application/json</span><span class="sxs-lookup"><span data-stu-id="feded-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feded-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feded-127">Request body</span></span>
<span data-ttu-id="feded-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="feded-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="feded-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="feded-129">Response</span></span>
<span data-ttu-id="feded-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="feded-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feded-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feded-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="feded-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feded-132">Request</span></span>
<span data-ttu-id="feded-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feded-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="feded-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="feded-134">Response</span></span>
<span data-ttu-id="feded-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="feded-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




