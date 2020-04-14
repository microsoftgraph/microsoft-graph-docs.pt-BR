---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89331e8874e6d9cbef172e5f1b121ddb85f97bdd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43360895"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="22f06-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="22f06-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="22f06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22f06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22f06-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22f06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22f06-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f06-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="22f06-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f06-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22f06-108">Prerequisites</span></span>
<span data-ttu-id="22f06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22f06-111">Permission type</span></span>|<span data-ttu-id="22f06-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22f06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f06-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22f06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22f06-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f06-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="22f06-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22f06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f06-116">Not supported.</span></span>|
|<span data-ttu-id="22f06-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22f06-117">Application</span></span>|<span data-ttu-id="22f06-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f06-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22f06-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="22f06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22f06-120">Request headers</span></span>
|<span data-ttu-id="22f06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22f06-121">Header</span></span>|<span data-ttu-id="22f06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22f06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22f06-123">Authorization</span></span>|<span data-ttu-id="22f06-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22f06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f06-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22f06-125">Accept</span></span>|<span data-ttu-id="22f06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22f06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22f06-127">Request body</span></span>
<span data-ttu-id="22f06-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22f06-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22f06-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f06-129">Response</span></span>
<span data-ttu-id="22f06-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22f06-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f06-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22f06-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f06-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22f06-132">Request</span></span>
<span data-ttu-id="22f06-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22f06-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="22f06-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f06-134">Response</span></span>
<span data-ttu-id="22f06-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



