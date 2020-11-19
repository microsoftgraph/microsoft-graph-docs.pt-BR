---
title: função getManagedDevicesWithFailedOrPendingApps
description: Recupera a lista de dispositivos com aplicativos com falha ou pendentes
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea4f3746c34f0aeed39892aaf0d1b67a9ee16427
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223197"
---
# <a name="getmanageddeviceswithfailedorpendingapps-function"></a><span data-ttu-id="f05e7-103">função getManagedDevicesWithFailedOrPendingApps</span><span class="sxs-lookup"><span data-stu-id="f05e7-103">getManagedDevicesWithFailedOrPendingApps function</span></span>

<span data-ttu-id="f05e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f05e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f05e7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f05e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f05e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f05e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f05e7-107">Recupera a lista de dispositivos com aplicativos com falha ou pendentes</span><span class="sxs-lookup"><span data-stu-id="f05e7-107">Retrieves the list of devices with failed or pending apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f05e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f05e7-108">Prerequisites</span></span>
<span data-ttu-id="f05e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f05e7-111">Permission type</span></span>|<span data-ttu-id="f05e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f05e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f05e7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f05e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f05e7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f05e7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f05e7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f05e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f05e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05e7-116">Not supported.</span></span>|
|<span data-ttu-id="f05e7-117">Application</span><span class="sxs-lookup"><span data-stu-id="f05e7-117">Application</span></span>|<span data-ttu-id="f05e7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f05e7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f05e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f05e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

## <a name="request-headers"></a><span data-ttu-id="f05e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f05e7-120">Request headers</span></span>
|<span data-ttu-id="f05e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f05e7-121">Header</span></span>|<span data-ttu-id="f05e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f05e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f05e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f05e7-123">Authorization</span></span>|<span data-ttu-id="f05e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f05e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f05e7-125">Accept</span></span>|<span data-ttu-id="f05e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f05e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f05e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f05e7-127">Request body</span></span>
<span data-ttu-id="f05e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f05e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f05e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05e7-129">Response</span></span>
<span data-ttu-id="f05e7-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f05e7-130">If successful, this function returns a `200 OK` response code and a [managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f05e7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f05e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f05e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f05e7-132">Request</span></span>
<span data-ttu-id="f05e7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f05e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

### <a name="response"></a><span data-ttu-id="f05e7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05e7-134">Response</span></span>
<span data-ttu-id="f05e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f05e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 187

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState",
      "summarizedAppState": "success",
      "deviceId": "Device Id value"
    }
  ]
}
```




