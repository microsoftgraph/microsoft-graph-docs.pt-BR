---
title: Listar mobileAppAssignments
description: Listar propriedades e relações dos objetos mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a6c5e4b14698b5bbce1e84af94cf0491fd67439
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793322"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="ca694-103">Listar mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="ca694-103">List mobileAppAssignments</span></span>

<span data-ttu-id="ca694-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca694-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca694-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca694-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca694-107">Listar propriedades e relações dos objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ca694-107">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca694-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca694-108">Prerequisites</span></span>
<span data-ttu-id="ca694-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ca694-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ca694-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca694-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca694-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca694-111">Permission type</span></span>|<span data-ttu-id="ca694-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca694-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca694-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca694-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca694-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca694-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ca694-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca694-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca694-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca694-116">Not supported.</span></span>|
|<span data-ttu-id="ca694-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca694-117">Application</span></span>|<span data-ttu-id="ca694-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca694-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca694-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca694-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ca694-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca694-120">Request headers</span></span>
|<span data-ttu-id="ca694-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca694-121">Header</span></span>|<span data-ttu-id="ca694-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca694-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca694-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca694-123">Authorization</span></span>|<span data-ttu-id="ca694-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca694-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca694-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca694-125">Accept</span></span>|<span data-ttu-id="ca694-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca694-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca694-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca694-127">Request body</span></span>
<span data-ttu-id="ca694-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca694-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca694-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca694-129">Response</span></span>
<span data-ttu-id="ca694-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca694-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca694-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca694-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca694-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca694-132">Request</span></span>
<span data-ttu-id="ca694-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca694-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="ca694-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca694-134">Response</span></span>
<span data-ttu-id="ca694-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ca694-135">Here is an example of the response.</span></span> <span data-ttu-id="ca694-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ca694-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ca694-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ca694-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 733

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "settings": {
        "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
        "vpnConfigurationId": "Vpn Configuration Id value",
        "uninstallOnDeviceRemoval": true
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



