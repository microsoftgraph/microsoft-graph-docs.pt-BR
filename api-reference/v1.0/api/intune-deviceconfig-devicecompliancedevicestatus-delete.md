---
title: Excluir deviceComplianceDeviceStatus
description: Exclui deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5be7d2e7bdd63190867ed5803aebe8c32f6c687
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43400301"
---
# <a name="delete-devicecompliancedevicestatus"></a><span data-ttu-id="27198-103">Excluir deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="27198-103">Delete deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="27198-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27198-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27198-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27198-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27198-106">Exclui [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="27198-106">Deletes a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27198-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27198-107">Prerequisites</span></span>
<span data-ttu-id="27198-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27198-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27198-110">Permission type</span></span>|<span data-ttu-id="27198-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27198-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27198-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27198-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27198-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27198-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27198-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27198-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27198-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27198-115">Not supported.</span></span>|
|<span data-ttu-id="27198-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27198-116">Application</span></span>|<span data-ttu-id="27198-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27198-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27198-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27198-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="27198-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27198-119">Request headers</span></span>
|<span data-ttu-id="27198-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27198-120">Header</span></span>|<span data-ttu-id="27198-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27198-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27198-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27198-122">Authorization</span></span>|<span data-ttu-id="27198-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27198-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27198-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27198-124">Accept</span></span>|<span data-ttu-id="27198-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27198-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27198-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27198-126">Request body</span></span>
<span data-ttu-id="27198-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27198-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27198-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="27198-128">Response</span></span>
<span data-ttu-id="27198-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27198-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27198-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27198-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="27198-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27198-131">Request</span></span>
<span data-ttu-id="27198-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27198-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="27198-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27198-133">Response</span></span>
<span data-ttu-id="27198-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27198-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






