---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76391441b068048ffc8e81be2cb1f3f5ac443704
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983335"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="82f72-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="82f72-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="82f72-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82f72-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82f72-105">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82f72-105">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82f72-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82f72-106">Prerequisites</span></span>
<span data-ttu-id="82f72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82f72-109">Permission type</span></span>|<span data-ttu-id="82f72-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82f72-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82f72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82f72-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="82f72-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="82f72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82f72-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82f72-114">Not supported.</span></span>|
|<span data-ttu-id="82f72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82f72-115">Application</span></span>|<span data-ttu-id="82f72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82f72-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f72-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82f72-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="82f72-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82f72-118">Request headers</span></span>
|<span data-ttu-id="82f72-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82f72-119">Header</span></span>|<span data-ttu-id="82f72-120">Valor</span><span class="sxs-lookup"><span data-stu-id="82f72-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82f72-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="82f72-121">Authorization</span></span>|<span data-ttu-id="82f72-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82f72-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82f72-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82f72-123">Accept</span></span>|<span data-ttu-id="82f72-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82f72-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f72-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82f72-125">Request body</span></span>
<span data-ttu-id="82f72-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82f72-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f72-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="82f72-127">Response</span></span>
<span data-ttu-id="82f72-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82f72-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82f72-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82f72-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="82f72-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82f72-130">Request</span></span>
<span data-ttu-id="82f72-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82f72-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="82f72-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="82f72-132">Response</span></span>
<span data-ttu-id="82f72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82f72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



