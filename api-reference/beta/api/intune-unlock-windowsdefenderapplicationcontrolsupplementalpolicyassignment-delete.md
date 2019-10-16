---
title: Excluir windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Exclui windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c5618c5cdece864ff91b6e64b436e73f08b0f8d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536676"
---
# <a name="delete-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="14455-103">Excluir windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="14455-103">Delete windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="14455-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14455-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14455-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14455-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14455-106">Exclui [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14455-106">Deletes a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14455-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14455-107">Prerequisites</span></span>
<span data-ttu-id="14455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14455-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14455-110">Permission type</span></span>|<span data-ttu-id="14455-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14455-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14455-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14455-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14455-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14455-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="14455-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14455-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14455-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14455-115">Not supported.</span></span>|
|<span data-ttu-id="14455-116">Application</span><span class="sxs-lookup"><span data-stu-id="14455-116">Application</span></span>|<span data-ttu-id="14455-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14455-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14455-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14455-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="14455-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14455-119">Request headers</span></span>
|<span data-ttu-id="14455-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14455-120">Header</span></span>|<span data-ttu-id="14455-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14455-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14455-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14455-122">Authorization</span></span>|<span data-ttu-id="14455-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14455-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14455-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14455-124">Accept</span></span>|<span data-ttu-id="14455-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14455-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14455-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14455-126">Request body</span></span>
<span data-ttu-id="14455-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14455-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14455-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="14455-128">Response</span></span>
<span data-ttu-id="14455-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14455-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14455-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14455-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="14455-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14455-131">Request</span></span>
<span data-ttu-id="14455-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14455-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="14455-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="14455-133">Response</span></span>
<span data-ttu-id="14455-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14455-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






