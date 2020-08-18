---
title: função getComanagedDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44dd46dc5fd48127ed380a50a9d43f98bb2364bb
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792489"
---
# <a name="getcomanageddevicessummary-function"></a><span data-ttu-id="1148f-103">função getComanagedDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="1148f-103">getComanagedDevicesSummary function</span></span>

<span data-ttu-id="1148f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1148f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1148f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1148f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1148f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1148f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1148f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1148f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1148f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1148f-108">Prerequisites</span></span>
<span data-ttu-id="1148f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1148f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1148f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1148f-111">Permission type</span></span>|<span data-ttu-id="1148f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1148f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1148f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1148f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1148f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1148f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1148f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1148f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1148f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1148f-116">Not supported.</span></span>|
|<span data-ttu-id="1148f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1148f-117">Application</span></span>|<span data-ttu-id="1148f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1148f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1148f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1148f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagedDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="1148f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1148f-120">Request headers</span></span>
|<span data-ttu-id="1148f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1148f-121">Header</span></span>|<span data-ttu-id="1148f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1148f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1148f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1148f-123">Authorization</span></span>|<span data-ttu-id="1148f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1148f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1148f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1148f-125">Accept</span></span>|<span data-ttu-id="1148f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1148f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1148f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1148f-127">Request body</span></span>
<span data-ttu-id="1148f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1148f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1148f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1148f-129">Response</span></span>
<span data-ttu-id="1148f-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1148f-130">If successful, this function returns a `200 OK` response code and a [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1148f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1148f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1148f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1148f-132">Request</span></span>
<span data-ttu-id="1148f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1148f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagedDevicesSummary
```

### <a name="response"></a><span data-ttu-id="1148f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1148f-134">Response</span></span>
<span data-ttu-id="1148f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1148f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "microsoft.graph.comanagedDevicesSummary",
    "inventoryCount": 14,
    "compliancePolicyCount": 5,
    "resourceAccessCount": 3,
    "configurationSettingsCount": 10,
    "windowsUpdateForBusinessCount": 13,
    "endpointProtectionCount": 7,
    "modernAppsCount": 15,
    "officeAppsCount": 15,
    "totalComanagedCount": 3
  }
}
```



