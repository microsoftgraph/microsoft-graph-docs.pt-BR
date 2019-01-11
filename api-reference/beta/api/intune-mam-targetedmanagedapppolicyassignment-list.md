---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a9ed6fd48467408ba940157530d8b9925515f3d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821998"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="fbc75-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="fbc75-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="fbc75-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbc75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbc75-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbc75-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fbc75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbc75-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fbc75-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbc75-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbc75-108">Prerequisites</span></span>
<span data-ttu-id="fbc75-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc75-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbc75-111">Permission type</span></span>|<span data-ttu-id="fbc75-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbc75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc75-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbc75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc75-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbc75-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fbc75-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbc75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc75-116">Not supported.</span></span>|
|<span data-ttu-id="fbc75-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbc75-117">Application</span></span>|<span data-ttu-id="fbc75-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc75-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc75-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fbc75-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc75-120">Request headers</span></span>
|<span data-ttu-id="fbc75-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbc75-121">Header</span></span>|<span data-ttu-id="fbc75-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbc75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc75-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbc75-123">Authorization</span></span>|<span data-ttu-id="fbc75-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc75-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbc75-125">Accept</span></span>|<span data-ttu-id="fbc75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc75-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc75-127">Request body</span></span>
<span data-ttu-id="fbc75-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbc75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbc75-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc75-129">Response</span></span>
<span data-ttu-id="fbc75-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc75-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc75-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbc75-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbc75-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc75-132">Request</span></span>
<span data-ttu-id="fbc75-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbc75-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="fbc75-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc75-134">Response</span></span>
<span data-ttu-id="fbc75-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbc75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





