---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2ddc4d37717ba5fe8d167f2ea79f61df7eee970
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178861"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="c374e-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="c374e-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="c374e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c374e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c374e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c374e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c374e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c374e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c374e-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c374e-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c374e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c374e-108">Prerequisites</span></span>
<span data-ttu-id="c374e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c374e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c374e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c374e-111">Permission type</span></span>|<span data-ttu-id="c374e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c374e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c374e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c374e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c374e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c374e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c374e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c374e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c374e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c374e-116">Not supported.</span></span>|
|<span data-ttu-id="c374e-117">Application</span><span class="sxs-lookup"><span data-stu-id="c374e-117">Application</span></span>|<span data-ttu-id="c374e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c374e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c374e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c374e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c374e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c374e-120">Request headers</span></span>
|<span data-ttu-id="c374e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c374e-121">Header</span></span>|<span data-ttu-id="c374e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c374e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c374e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c374e-123">Authorization</span></span>|<span data-ttu-id="c374e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c374e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c374e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c374e-125">Accept</span></span>|<span data-ttu-id="c374e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c374e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c374e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c374e-127">Request body</span></span>
<span data-ttu-id="c374e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c374e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c374e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c374e-129">Response</span></span>
<span data-ttu-id="c374e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c374e-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c374e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c374e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c374e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c374e-132">Request</span></span>
<span data-ttu-id="c374e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c374e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="c374e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c374e-134">Response</span></span>
<span data-ttu-id="c374e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c374e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



