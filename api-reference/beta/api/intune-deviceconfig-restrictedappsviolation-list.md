---
title: Listar restrictedAppsViolations
description: Listar propriedades e relações dos objetos restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8617c15fdb23de0833ea467c3794fb09321d2561
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132475"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="aa40e-103">Listar restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="aa40e-103">List restrictedAppsViolations</span></span>

<span data-ttu-id="aa40e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa40e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa40e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa40e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa40e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa40e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa40e-107">Listar propriedades e relações dos objetos [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="aa40e-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa40e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa40e-108">Prerequisites</span></span>
<span data-ttu-id="aa40e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa40e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa40e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa40e-111">Permission type</span></span>|<span data-ttu-id="aa40e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa40e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa40e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa40e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa40e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa40e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa40e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa40e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa40e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa40e-116">Not supported.</span></span>|
|<span data-ttu-id="aa40e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa40e-117">Application</span></span>|<span data-ttu-id="aa40e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa40e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa40e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa40e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="aa40e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa40e-120">Request headers</span></span>
|<span data-ttu-id="aa40e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa40e-121">Header</span></span>|<span data-ttu-id="aa40e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aa40e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa40e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa40e-123">Authorization</span></span>|<span data-ttu-id="aa40e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa40e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa40e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa40e-125">Accept</span></span>|<span data-ttu-id="aa40e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa40e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa40e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa40e-127">Request body</span></span>
<span data-ttu-id="aa40e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa40e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa40e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa40e-129">Response</span></span>
<span data-ttu-id="aa40e-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa40e-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa40e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa40e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa40e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa40e-132">Request</span></span>
<span data-ttu-id="aa40e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa40e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="aa40e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa40e-134">Response</span></span>
<span data-ttu-id="aa40e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa40e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




