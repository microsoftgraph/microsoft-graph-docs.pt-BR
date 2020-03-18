---
title: Excluir targetedManagedAppPolicyAssignment
description: Exclui targetedManagedAppPolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42a8cb9af1a1eba9b54cea74ca45bb64500bd6da
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803432"
---
# <a name="delete-targetedmanagedapppolicyassignment"></a><span data-ttu-id="09bca-103">Excluir targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="09bca-103">Delete targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="09bca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09bca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09bca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09bca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09bca-106">Exclui [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09bca-106">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09bca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09bca-107">Prerequisites</span></span>
<span data-ttu-id="09bca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09bca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09bca-110">Permission type</span></span>|<span data-ttu-id="09bca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09bca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09bca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09bca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09bca-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bca-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09bca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09bca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09bca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09bca-115">Not supported.</span></span>|
|<span data-ttu-id="09bca-116">Application</span><span class="sxs-lookup"><span data-stu-id="09bca-116">Application</span></span>|<span data-ttu-id="09bca-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bca-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09bca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09bca-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="09bca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09bca-119">Request headers</span></span>
|<span data-ttu-id="09bca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09bca-120">Header</span></span>|<span data-ttu-id="09bca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="09bca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09bca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09bca-122">Authorization</span></span>|<span data-ttu-id="09bca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09bca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09bca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09bca-124">Accept</span></span>|<span data-ttu-id="09bca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09bca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09bca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09bca-126">Request body</span></span>
<span data-ttu-id="09bca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09bca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09bca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="09bca-128">Response</span></span>
<span data-ttu-id="09bca-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09bca-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09bca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09bca-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09bca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09bca-131">Request</span></span>
<span data-ttu-id="09bca-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09bca-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="09bca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="09bca-133">Response</span></span>
<span data-ttu-id="09bca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09bca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




