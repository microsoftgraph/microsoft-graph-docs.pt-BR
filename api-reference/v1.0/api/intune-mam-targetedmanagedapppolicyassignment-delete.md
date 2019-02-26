---
title: Excluir targetedManagedAppPolicyAssignment
description: Exclui targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9729cf1d6483dc4f972aa83c760753f1c6197b27
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251283"
---
# <a name="delete-targetedmanagedapppolicyassignment"></a><span data-ttu-id="11b88-103">Excluir targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="11b88-103">Delete targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="11b88-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11b88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b88-105">Exclui [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="11b88-105">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11b88-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11b88-106">Prerequisites</span></span>
<span data-ttu-id="11b88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="11b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="11b88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11b88-109">Permission type</span></span>|<span data-ttu-id="11b88-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11b88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11b88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11b88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11b88-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b88-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11b88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11b88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11b88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b88-114">Not supported.</span></span>|
|<span data-ttu-id="11b88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11b88-115">Application</span></span>|<span data-ttu-id="11b88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11b88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11b88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="11b88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11b88-118">Request headers</span></span>
|<span data-ttu-id="11b88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11b88-119">Header</span></span>|<span data-ttu-id="11b88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="11b88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11b88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11b88-121">Authorization</span></span>|<span data-ttu-id="11b88-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11b88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11b88-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11b88-123">Accept</span></span>|<span data-ttu-id="11b88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11b88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11b88-125">Request body</span></span>
<span data-ttu-id="11b88-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11b88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11b88-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b88-127">Response</span></span>
<span data-ttu-id="11b88-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="11b88-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11b88-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11b88-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="11b88-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11b88-130">Request</span></span>
<span data-ttu-id="11b88-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11b88-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="11b88-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b88-132">Response</span></span>
<span data-ttu-id="11b88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11b88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



