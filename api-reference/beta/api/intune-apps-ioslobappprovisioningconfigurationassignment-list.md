---
title: Listar iosLobAppProvisioningConfigurationAssignments
description: Listar Propriedades e relações dos objetos iosLobAppProvisioningConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f2bbb86d3f939d8bb162b527b01f9195b66ee5f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793385"
---
# <a name="list-ioslobappprovisioningconfigurationassignments"></a><span data-ttu-id="bad92-103">Listar iosLobAppProvisioningConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="bad92-103">List iosLobAppProvisioningConfigurationAssignments</span></span>

<span data-ttu-id="bad92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bad92-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bad92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bad92-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bad92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bad92-107">Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bad92-107">List properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bad92-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bad92-108">Prerequisites</span></span>
<span data-ttu-id="bad92-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bad92-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bad92-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bad92-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bad92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bad92-111">Permission type</span></span>|<span data-ttu-id="bad92-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bad92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bad92-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bad92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bad92-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bad92-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bad92-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bad92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bad92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bad92-116">Not supported.</span></span>|
|<span data-ttu-id="bad92-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bad92-117">Application</span></span>|<span data-ttu-id="bad92-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bad92-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bad92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bad92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bad92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bad92-120">Request headers</span></span>
|<span data-ttu-id="bad92-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bad92-121">Header</span></span>|<span data-ttu-id="bad92-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bad92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bad92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bad92-123">Authorization</span></span>|<span data-ttu-id="bad92-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bad92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bad92-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bad92-125">Accept</span></span>|<span data-ttu-id="bad92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bad92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bad92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bad92-127">Request body</span></span>
<span data-ttu-id="bad92-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bad92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bad92-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bad92-129">Response</span></span>
<span data-ttu-id="bad92-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bad92-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bad92-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bad92-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bad92-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bad92-132">Request</span></span>
<span data-ttu-id="bad92-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bad92-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="bad92-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bad92-134">Response</span></span>
<span data-ttu-id="bad92-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="bad92-135">Here is an example of the response.</span></span> <span data-ttu-id="bad92-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="bad92-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bad92-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bad92-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 461

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



