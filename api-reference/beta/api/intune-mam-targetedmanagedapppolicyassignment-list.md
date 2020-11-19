---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbfd52d7b28c54cf46943b98fee41a52cc14d0f1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277453"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="9a4cd-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="9a4cd-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="9a4cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a4cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a4cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a4cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4cd-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9a4cd-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a4cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a4cd-108">Prerequisites</span></span>
<span data-ttu-id="9a4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a4cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a4cd-111">Permission type</span></span>|<span data-ttu-id="9a4cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a4cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a4cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a4cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a4cd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a4cd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9a4cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a4cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a4cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-116">Not supported.</span></span>|
|<span data-ttu-id="9a4cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a4cd-117">Application</span></span>|<span data-ttu-id="9a4cd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a4cd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a4cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a4cd-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9a4cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4cd-120">Request headers</span></span>
|<span data-ttu-id="9a4cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a4cd-121">Header</span></span>|<span data-ttu-id="9a4cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a4cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a4cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a4cd-123">Authorization</span></span>|<span data-ttu-id="9a4cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a4cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a4cd-125">Accept</span></span>|<span data-ttu-id="9a4cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a4cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a4cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4cd-127">Request body</span></span>
<span data-ttu-id="9a4cd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a4cd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a4cd-129">Response</span></span>
<span data-ttu-id="9a4cd-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a4cd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a4cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a4cd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4cd-132">Request</span></span>
<span data-ttu-id="9a4cd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="9a4cd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a4cd-134">Response</span></span>
<span data-ttu-id="9a4cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a4cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




