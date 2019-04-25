---
title: Get targetedManagedAppPolicyAssignment
description: Ler propriedades e relações do objeto targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3abec81ea2d39e088c96d2f5d2650010818e4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529321"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="6ad39-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6ad39-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="6ad39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ad39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ad39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad39-106">Ler propriedades e relações do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ad39-106">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ad39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ad39-107">Prerequisites</span></span>
<span data-ttu-id="6ad39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ad39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ad39-110">Permission type</span></span>|<span data-ttu-id="6ad39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ad39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ad39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ad39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ad39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ad39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6ad39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ad39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ad39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ad39-115">Not supported.</span></span>|
|<span data-ttu-id="6ad39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ad39-116">Application</span></span>|<span data-ttu-id="6ad39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ad39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ad39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ad39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ad39-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ad39-119">Optional query parameters</span></span>
<span data-ttu-id="6ad39-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ad39-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ad39-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad39-121">Request headers</span></span>
|<span data-ttu-id="6ad39-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ad39-122">Header</span></span>|<span data-ttu-id="6ad39-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6ad39-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ad39-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ad39-124">Authorization</span></span>|<span data-ttu-id="6ad39-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ad39-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ad39-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ad39-126">Accept</span></span>|<span data-ttu-id="6ad39-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6ad39-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ad39-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad39-128">Request body</span></span>
<span data-ttu-id="6ad39-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ad39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ad39-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad39-130">Response</span></span>
<span data-ttu-id="6ad39-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ad39-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ad39-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ad39-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ad39-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad39-133">Request</span></span>
<span data-ttu-id="6ad39-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ad39-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6ad39-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad39-135">Response</span></span>
<span data-ttu-id="6ad39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ad39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





