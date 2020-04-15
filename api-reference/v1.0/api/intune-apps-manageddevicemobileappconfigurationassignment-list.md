---
title: Listar managedDeviceMobileAppConfigurationAssignments
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7db781fd33984f3abe270c30c03d5ee6bdf401ec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446283"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="8359d-103">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8359d-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="8359d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8359d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8359d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8359d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8359d-106">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8359d-106">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8359d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8359d-107">Prerequisites</span></span>
<span data-ttu-id="8359d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8359d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8359d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8359d-110">Permission type</span></span>|<span data-ttu-id="8359d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8359d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8359d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8359d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8359d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8359d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8359d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8359d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8359d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8359d-115">Not supported.</span></span>|
|<span data-ttu-id="8359d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8359d-116">Application</span></span>|<span data-ttu-id="8359d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8359d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8359d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8359d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8359d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8359d-119">Request headers</span></span>
|<span data-ttu-id="8359d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8359d-120">Header</span></span>|<span data-ttu-id="8359d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8359d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8359d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8359d-122">Authorization</span></span>|<span data-ttu-id="8359d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8359d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8359d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8359d-124">Accept</span></span>|<span data-ttu-id="8359d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8359d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8359d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8359d-126">Request body</span></span>
<span data-ttu-id="8359d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8359d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8359d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8359d-128">Response</span></span>
<span data-ttu-id="8359d-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8359d-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8359d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8359d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8359d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8359d-131">Request</span></span>
<span data-ttu-id="8359d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8359d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="8359d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8359d-133">Response</span></span>
<span data-ttu-id="8359d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8359d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






