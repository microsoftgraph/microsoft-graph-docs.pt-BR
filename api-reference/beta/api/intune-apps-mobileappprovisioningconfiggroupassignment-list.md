---
title: Listar mobileAppProvisioningConfigGroupAssignments
description: Listar Propriedades e relações dos objetos mobileAppProvisioningConfigGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5946fb2a4f14947f187a64f47cd633a288d185fd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934886"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="90ec3-103">Listar mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="90ec3-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="90ec3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90ec3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ec3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90ec3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ec3-106">Listar Propriedades e relações dos objetos [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="90ec3-106">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ec3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90ec3-107">Prerequisites</span></span>
<span data-ttu-id="90ec3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ec3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ec3-110">Permission type</span></span>|<span data-ttu-id="90ec3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90ec3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ec3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ec3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90ec3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="90ec3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="90ec3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ec3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ec3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ec3-115">Not supported.</span></span>|
|<span data-ttu-id="90ec3-116">Application</span><span class="sxs-lookup"><span data-stu-id="90ec3-116">Application</span></span>|<span data-ttu-id="90ec3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="90ec3-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ec3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ec3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="90ec3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ec3-119">Request headers</span></span>
|<span data-ttu-id="90ec3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90ec3-120">Header</span></span>|<span data-ttu-id="90ec3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90ec3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ec3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ec3-122">Authorization</span></span>|<span data-ttu-id="90ec3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ec3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ec3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90ec3-124">Accept</span></span>|<span data-ttu-id="90ec3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90ec3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ec3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ec3-126">Request body</span></span>
<span data-ttu-id="90ec3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90ec3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ec3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ec3-128">Response</span></span>
<span data-ttu-id="90ec3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ec3-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ec3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90ec3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ec3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ec3-131">Request</span></span>
<span data-ttu-id="90ec3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ec3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="90ec3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ec3-133">Response</span></span>
<span data-ttu-id="90ec3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ec3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```





