---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e01927b9447f77ce571bf2e855eb80350ccfce26
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759104"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="4b222-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="4b222-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="4b222-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b222-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b222-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b222-106">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b222-106">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b222-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b222-107">Prerequisites</span></span>
<span data-ttu-id="4b222-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b222-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b222-110">Permission type</span></span>|<span data-ttu-id="4b222-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b222-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b222-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b222-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b222-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b222-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b222-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b222-115">Not supported.</span></span>|
|<span data-ttu-id="4b222-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b222-116">Application</span></span>|<span data-ttu-id="4b222-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b222-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b222-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b222-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4b222-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b222-119">Request headers</span></span>
|<span data-ttu-id="4b222-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b222-120">Header</span></span>|<span data-ttu-id="4b222-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4b222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b222-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b222-122">Authorization</span></span>|<span data-ttu-id="4b222-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b222-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b222-124">Accept</span></span>|<span data-ttu-id="4b222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b222-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b222-126">Request body</span></span>
<span data-ttu-id="4b222-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b222-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b222-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b222-128">Response</span></span>
<span data-ttu-id="4b222-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b222-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b222-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b222-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b222-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b222-131">Request</span></span>
<span data-ttu-id="4b222-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b222-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="4b222-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b222-133">Response</span></span>
<span data-ttu-id="4b222-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b222-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 332

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




