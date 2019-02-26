---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10b1e91d3f1582988b0a1d18e0962eff50521973
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254594"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="51126-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="51126-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="51126-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51126-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51126-105">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51126-105">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51126-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51126-106">Prerequisites</span></span>
<span data-ttu-id="51126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="51126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51126-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51126-109">Permission type</span></span>|<span data-ttu-id="51126-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51126-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51126-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51126-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51126-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51126-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51126-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51126-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51126-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51126-114">Not supported.</span></span>|
|<span data-ttu-id="51126-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51126-115">Application</span></span>|<span data-ttu-id="51126-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51126-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51126-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51126-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="51126-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51126-118">Request headers</span></span>
|<span data-ttu-id="51126-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51126-119">Header</span></span>|<span data-ttu-id="51126-120">Valor</span><span class="sxs-lookup"><span data-stu-id="51126-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51126-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="51126-121">Authorization</span></span>|<span data-ttu-id="51126-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51126-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51126-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51126-123">Accept</span></span>|<span data-ttu-id="51126-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51126-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51126-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51126-125">Request body</span></span>
<span data-ttu-id="51126-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51126-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51126-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="51126-127">Response</span></span>
<span data-ttu-id="51126-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51126-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51126-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51126-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="51126-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51126-130">Request</span></span>
<span data-ttu-id="51126-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51126-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="51126-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="51126-132">Response</span></span>
<span data-ttu-id="51126-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



