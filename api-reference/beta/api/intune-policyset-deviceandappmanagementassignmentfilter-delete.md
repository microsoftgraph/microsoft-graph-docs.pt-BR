---
title: Excluir deviceAndAppManagementAssignmentFilter
description: Exclui deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 509fa93280cfa534194af3fcf85006f9c5ba6db2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233149"
---
# <a name="delete-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="e557b-103">Excluir deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="e557b-103">Delete deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="e557b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e557b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e557b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e557b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e557b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e557b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e557b-107">Exclui [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="e557b-107">Deletes a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e557b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e557b-108">Prerequisites</span></span>
<span data-ttu-id="e557b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e557b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e557b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e557b-111">Permission type</span></span>|<span data-ttu-id="e557b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e557b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e557b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e557b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e557b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e557b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e557b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e557b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e557b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e557b-116">Not supported.</span></span>|
|<span data-ttu-id="e557b-117">Application</span><span class="sxs-lookup"><span data-stu-id="e557b-117">Application</span></span>|<span data-ttu-id="e557b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e557b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e557b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e557b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="e557b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e557b-120">Request headers</span></span>
|<span data-ttu-id="e557b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e557b-121">Header</span></span>|<span data-ttu-id="e557b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e557b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e557b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e557b-123">Authorization</span></span>|<span data-ttu-id="e557b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e557b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e557b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e557b-125">Accept</span></span>|<span data-ttu-id="e557b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e557b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e557b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e557b-127">Request body</span></span>
<span data-ttu-id="e557b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e557b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e557b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e557b-129">Response</span></span>
<span data-ttu-id="e557b-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e557b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e557b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e557b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e557b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e557b-132">Request</span></span>
<span data-ttu-id="e557b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e557b-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

### <a name="response"></a><span data-ttu-id="e557b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e557b-134">Response</span></span>
<span data-ttu-id="e557b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e557b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




