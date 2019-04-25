---
title: Listar settingStateDeviceSummaries
description: Listar propriedades e relações dos objetos settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89fc1df7d1951650e36df2f8e2a367654a6c96d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572588"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="92890-103">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="92890-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="92890-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92890-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92890-105">Listar propriedades e relações dos objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="92890-105">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92890-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92890-106">Prerequisites</span></span>
<span data-ttu-id="92890-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92890-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92890-109">Permission type</span></span>|<span data-ttu-id="92890-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92890-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92890-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92890-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92890-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92890-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92890-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92890-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92890-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92890-114">Not supported.</span></span>|
|<span data-ttu-id="92890-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92890-115">Application</span></span>|<span data-ttu-id="92890-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92890-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92890-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92890-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="92890-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92890-118">Request headers</span></span>
|<span data-ttu-id="92890-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92890-119">Header</span></span>|<span data-ttu-id="92890-120">Valor</span><span class="sxs-lookup"><span data-stu-id="92890-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92890-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="92890-121">Authorization</span></span>|<span data-ttu-id="92890-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92890-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92890-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92890-123">Accept</span></span>|<span data-ttu-id="92890-124">application/json</span><span class="sxs-lookup"><span data-stu-id="92890-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92890-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92890-125">Request body</span></span>
<span data-ttu-id="92890-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92890-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92890-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="92890-127">Response</span></span>
<span data-ttu-id="92890-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92890-128">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92890-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92890-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="92890-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92890-130">Request</span></span>
<span data-ttu-id="92890-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92890-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="92890-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="92890-132">Response</span></span>
<span data-ttu-id="92890-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92890-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```



