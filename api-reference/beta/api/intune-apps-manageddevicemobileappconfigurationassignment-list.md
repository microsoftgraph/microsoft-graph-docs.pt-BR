---
title: Listar managedDeviceMobileAppConfigurationAssignments
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb8b92de608a5402f0386321dd0916a0bfa627c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961627"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="5ee07-103">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="5ee07-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="5ee07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ee07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ee07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee07-106">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ee07-106">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ee07-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ee07-107">Prerequisites</span></span>
<span data-ttu-id="5ee07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee07-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee07-110">Permission type</span></span>|<span data-ttu-id="5ee07-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ee07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee07-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee07-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ee07-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5ee07-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee07-115">Not supported.</span></span>|
|<span data-ttu-id="5ee07-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee07-116">Application</span></span>|<span data-ttu-id="5ee07-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee07-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5ee07-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee07-119">Request headers</span></span>
|<span data-ttu-id="5ee07-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ee07-120">Header</span></span>|<span data-ttu-id="5ee07-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ee07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee07-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee07-122">Authorization</span></span>|<span data-ttu-id="5ee07-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee07-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ee07-124">Accept</span></span>|<span data-ttu-id="5ee07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee07-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee07-126">Request body</span></span>
<span data-ttu-id="5ee07-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ee07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee07-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee07-128">Response</span></span>
<span data-ttu-id="5ee07-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee07-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee07-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ee07-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ee07-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee07-131">Request</span></span>
<span data-ttu-id="5ee07-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee07-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="5ee07-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee07-133">Response</span></span>
<span data-ttu-id="5ee07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





