---
title: Listar managedDeviceMobileAppConfigurationAssignments
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79d0e741ce9fbcdd691a0bf71cf5c4f3abe97515
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699461"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="a0220-103">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a0220-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="a0220-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0220-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0220-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0220-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0220-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0220-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0220-107">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0220-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0220-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0220-108">Prerequisites</span></span>
<span data-ttu-id="a0220-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0220-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0220-111">Permission type</span></span>|<span data-ttu-id="a0220-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0220-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0220-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0220-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0220-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0220-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0220-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0220-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0220-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0220-116">Not supported.</span></span>|
|<span data-ttu-id="a0220-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0220-117">Application</span></span>|<span data-ttu-id="a0220-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0220-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0220-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0220-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a0220-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-120">Request headers</span></span>
|<span data-ttu-id="a0220-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0220-121">Header</span></span>|<span data-ttu-id="a0220-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0220-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0220-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0220-123">Authorization</span></span>|<span data-ttu-id="a0220-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0220-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0220-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0220-125">Accept</span></span>|<span data-ttu-id="a0220-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0220-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0220-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-127">Request body</span></span>
<span data-ttu-id="a0220-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0220-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0220-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0220-129">Response</span></span>
<span data-ttu-id="a0220-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0220-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0220-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0220-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0220-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-132">Request</span></span>
<span data-ttu-id="a0220-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0220-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="a0220-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0220-134">Response</span></span>
<span data-ttu-id="a0220-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0220-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```





