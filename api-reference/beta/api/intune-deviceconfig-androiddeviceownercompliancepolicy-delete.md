---
title: Excluir androidDeviceOwnerCompliancePolicy
description: Exclui androidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fac35c5cba1897078aaa4a91b295ab0098007dcc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242865"
---
# <a name="delete-androiddeviceownercompliancepolicy"></a><span data-ttu-id="a0f50-103">Excluir androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a0f50-103">Delete androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="a0f50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0f50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0f50-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0f50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0f50-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0f50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0f50-107">Exclui [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0f50-107">Deletes a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0f50-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0f50-108">Prerequisites</span></span>
<span data-ttu-id="a0f50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0f50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0f50-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0f50-111">Permission type</span></span>|<span data-ttu-id="a0f50-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0f50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0f50-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0f50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0f50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0f50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0f50-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0f50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0f50-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0f50-116">Not supported.</span></span>|
|<span data-ttu-id="a0f50-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0f50-117">Application</span></span>|<span data-ttu-id="a0f50-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0f50-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0f50-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0f50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a0f50-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f50-120">Request headers</span></span>
|<span data-ttu-id="a0f50-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0f50-121">Header</span></span>|<span data-ttu-id="a0f50-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0f50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0f50-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0f50-123">Authorization</span></span>|<span data-ttu-id="a0f50-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0f50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0f50-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0f50-125">Accept</span></span>|<span data-ttu-id="a0f50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0f50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0f50-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f50-127">Request body</span></span>
<span data-ttu-id="a0f50-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0f50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0f50-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0f50-129">Response</span></span>
<span data-ttu-id="a0f50-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a0f50-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a0f50-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0f50-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0f50-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f50-132">Request</span></span>
<span data-ttu-id="a0f50-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0f50-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a0f50-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0f50-134">Response</span></span>
<span data-ttu-id="a0f50-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0f50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




