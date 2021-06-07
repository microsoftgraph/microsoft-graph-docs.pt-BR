---
title: Excluir deviceComplianceDeviceStatus
description: Exclui deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e6b8a2f0d95145ca892168d761d2884a5c4f8ec
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756628"
---
# <a name="delete-devicecompliancedevicestatus"></a><span data-ttu-id="8d6cf-103">Excluir deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8d6cf-103">Delete deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="8d6cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d6cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d6cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d6cf-106">Exclui [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8d6cf-106">Deletes a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d6cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d6cf-107">Prerequisites</span></span>
<span data-ttu-id="8d6cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d6cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d6cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d6cf-110">Permission type</span></span>|<span data-ttu-id="8d6cf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d6cf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d6cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d6cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d6cf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6cf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d6cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d6cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d6cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-115">Not supported.</span></span>|
|<span data-ttu-id="8d6cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d6cf-116">Application</span></span>|<span data-ttu-id="8d6cf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6cf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d6cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d6cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8d6cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d6cf-119">Request headers</span></span>
|<span data-ttu-id="8d6cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d6cf-120">Header</span></span>|<span data-ttu-id="8d6cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8d6cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d6cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d6cf-122">Authorization</span></span>|<span data-ttu-id="8d6cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d6cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d6cf-124">Accept</span></span>|<span data-ttu-id="8d6cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d6cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d6cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d6cf-126">Request body</span></span>
<span data-ttu-id="8d6cf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d6cf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d6cf-128">Response</span></span>
<span data-ttu-id="8d6cf-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d6cf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d6cf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d6cf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d6cf-131">Request</span></span>
<span data-ttu-id="8d6cf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8d6cf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d6cf-133">Response</span></span>
<span data-ttu-id="8d6cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d6cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




